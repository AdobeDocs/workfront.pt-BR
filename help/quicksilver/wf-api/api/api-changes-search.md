---
filename: api-changes-search
content-type: api
keywords: objeto,status,pesquisa,melhor,prática,resposta
navigation-topic: api-navigation-topic
title: "Alterações na API principal: Respostas de pesquisa de status"
description: Alterações na maneira como o Workfront armazena objetos de status.
exl-id: 322f1525-d1d5-4845-a590-e34eb94ccdc2
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 1%

---

# Alterações na API principal: Respostas de pesquisa de status

Foram feitas alterações na maneira como o Workfront armazena objetos de status. Essas alterações não afetam como as solicitações de pesquisa de status são feitas, mas afetarão a resposta retornada pelas solicitações de API que incluem uma pesquisa por objetos de status retornando uma lista incompleta de status de grupo.

## Práticas recomendadas

Para obter com confiança a lista completa de status disponíveis para um grupo, as seguintes solicitações são consideradas práticas recomendadas.

>[!NOTE]
>
>Essas estruturas de solicitação são recomendadas para todos os usuários, independentemente de as alterações de pesquisa de status terem ou não sido feitas no cluster.

Para Status do Grupo de Projetos:

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

Todos os três pontos finais aceitam o **includeHidden=true** para buscar os status ocultos do projeto/tarefa/emissão de um determinado grupo. Modelar suas consultas de pesquisa de status após esses exemplos de práticas recomendadas garantirá que todas as informações de status do grupo sejam incluídas com cada resposta.

Este é um exemplo de uma consulta de pesquisa de status sendo feita para um grupo de tarefas que inclui um status bloqueado no nível do sistema **Personalizado_1** e um status desbloqueado **Personalizado_2**:

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

## Noções básicas das alterações feitas na consulta de pesquisa de status herdada

No sistema herdado, uma consulta de pesquisa de status copiaria todos os status do sistema disponíveis para todos os grupos incluídos em uma consulta. A resposta herdada incluiria todos os status do sistema e status de nível de grupo disponíveis para cada grupo na query.

Por exemplo, esta query (que não segue as práticas recomendadas atuais):

>**Exemplo:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

Teria a seguinte resposta sob o sistema herdado, que inclui todos os status de objeto:

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

No entanto, após as atualizações feitas na maneira como os status são armazenados e usados, os status não são copiados para grupos e são herdados por cada grupo no nível do sistema. Como resultado, a consulta da API de pesquisa lê apenas os status que estão diretamente associados a um grupo específico, de modo que a resposta inclui os status bloqueados e desbloqueados do sistema, mas somente para os grupos que foram criados após a adição do status em questão.

Se os métodos de práticas recomendadas atualizados não forem usados para fazer consultas de pesquisa de status depois que o sistema herdado tiver sido atualizado, uma lista incompleta de status de grupo será retornada na resposta.

Este é um exemplo do que essa estrutura de solicitação desatualizada retorna depois que o sistema herdado é atualizado:

>**Exemplo:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

Observe que essa resposta inclui apenas status específicos do grupo e exclui os status que foram declarados no nível do sistema:

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
