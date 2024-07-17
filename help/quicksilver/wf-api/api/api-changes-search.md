---
filename: api-changes-search
content-type: api
keywords: objeto,status,pesquisa,melhor,prática,resposta
navigation-topic: api-navigation-topic
title: "Alterações na API principal: respostas de pesquisa de status"
description: Alterações na forma como o Workfront armazena objetos de status.
feature: Workfront API
role: Developer
exl-id: 322f1525-d1d5-4845-a590-e34eb94ccdc2
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 0%

---

# Alterações na API principal: respostas da pesquisa de status

Foram feitas alterações no modo como o Workfront armazena objetos de status. Essas alterações não afetam como as solicitações de pesquisa de status são feitas, mas afetarão a resposta retornada pelas solicitações de API que incluem uma pesquisa por objetos de status retornando uma lista incompleta de status de grupo.

## Práticas recomendadas

Para obter de maneira confiável a lista completa de status disponíveis para um grupo, as solicitações a seguir são consideradas práticas recomendadas.

>[!NOTE]
>
>Essas estruturas de solicitação são recomendadas para todos os usuários independentemente de as alterações na pesquisa de status terem ou não sido feitas no cluster.

Para Status do Grupo de Projeto:

>**Exemplo:**

```
/attask/api/<VERSION>/CSTEM/projectGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Para Status do Grupo de Tarefas:

>**Exemplo:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Para Status do Grupo de Problemas:

>**Exemplo:**

```
/attask/api/<VERSION>/CSTEM/opTaskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Todos esses três pontos de extremidade aceitam o parâmetro **includeHidden=true** para buscar os status ocultos de projeto/tarefa/problema de um determinado grupo. Modelar as consultas de pesquisa de status após esses exemplos de práticas recomendadas garantirá que todas as informações de status do grupo sejam incluídas em cada resposta.

Este é um exemplo de uma consulta de pesquisa de status sendo feita a um grupo de tarefas que inclui um status bloqueado no nível do sistema **Custom_1** e um status desbloqueado **Custom_2**:

>**Exemplo:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d286d000004fc8f53942de697a868
```

Usar esse formato garante que sua resposta inclua todos os itens a seguir:

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

## Noções básicas sobre as alterações feitas na consulta de pesquisa de status herdada

No sistema herdado, uma consulta de pesquisa de status copiaria todos os status de sistema disponíveis para todos os grupos incluídos em uma consulta. A resposta herdada incluiria todos os status do sistema e os status de nível de grupo disponíveis para cada grupo na consulta.

Por exemplo, esta consulta (que não segue as práticas recomendadas atuais):

>**Exemplo:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

Teria a seguinte resposta no sistema herdado, que inclui todos os status de objeto:

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

No entanto, após as atualizações feitas no modo como os status são armazenados e usados, os status não são copiados para grupos e são herdados por cada grupo no nível do sistema. Como resultado, a consulta da API de pesquisa lê apenas os status que estão diretamente associados a um grupo específico, portanto, a resposta inclui status bloqueados e desbloqueados pelo sistema, mas apenas para os grupos que foram criados após a adição do status em questão.

Falha ao usar os métodos de práticas recomendadas atualizadas para fazer consultas de pesquisa de status após a atualização do sistema herdado resultará em uma lista incompleta de status de grupo retornados na resposta.

Este é um exemplo do que essa estrutura de solicitação desatualizada retorna após a atualização do sistema herdado:

>**Exemplo:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

Observe que essa resposta inclui apenas status específicos do grupo e deixa de fora os status que foram declarados no nível do sistema:

```
{
  "data": [
    {
      "color": "8BC34A",
      "equatesWith": "NEW",
      "groupID": "602d286d000004fc8f53942de697a868",
      "label": "Custom_2",
      "objCode": "CSTEM",
      "value": "MMI"
    }
  ]
}
```
