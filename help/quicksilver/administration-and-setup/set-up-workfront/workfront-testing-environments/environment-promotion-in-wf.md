---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Mover objetos de um ambiente para outro no Workfront
description: O recurso de Promoção do ambiente tem como objetivo fornecer a capacidade de mover objetos relacionados à configuração de um ambiente para outro. Ela não oferece suporte à capacidade de mover objetos transacionais (com exceções limitadas).
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: b44c83314a06592e21ab3c4316e2574b75e85715
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 1%

---

# Visão geral da movimentação de objetos entre ambientes do Workfront (promoção de ambiente)

O recurso de promoção de ambiente tem como objetivo fornecer a capacidade de mover objetos de um ambiente do Workfront para outro. Por exemplo, você pode criar um modelo e configurá-lo no ambiente de sandbox, sabendo que qualquer teste que você fizer não afetará os dados reais da sua organização. Depois que o modelo for configurado e testado, você poderá movê-lo para o ambiente de produção, pronto para uso.

Esse processo é chamado de &quot;promoção do ambiente&quot;.

Você pode executar esse processo no Workfront criando um pacote de objetos para mover e instalando esse pacote no novo ambiente.

* Para obter instruções específicas sobre como executar esse processo no Workfront, consulte:

   * [Criar ou editar um pacote de promoção de ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
   * [Instalar um pacote de promoção de ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

* Para obter instruções sobre como executar esse processo por meio da API do Workfront, consulte [Mover objetos entre [!DNL Workfront] ambientes que usam o [!DNL Workfront] API](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion.md).

## Objetos compatíveis com a promoção do ambiente

O recurso de Promoção do ambiente tem como objetivo fornecer a capacidade de mover objetos relacionados à configuração de um ambiente para outro. Ela não oferece suporte à capacidade de mover objetos transacionais (com exceções limitadas).

* [Objetos de trabalho](#work-objects)
* [Objetos de relatório](#reporting-objects)
* [Objetos de dados personalizados](#custom-data-objects)
* [Objetos da organização](#organization-objects)
* [Outros objetos de configuração](#other-configuration-objects)


### Objetos de trabalho

| Objeto promovível | Sub-objetos promovíveis incluídos |
| --- | --- |
| Projeto (PROJ) | Projeto<br>Tarefa<br>Atribuição<br>Predecessora<br>Empresa<br>Taxa de substituição<br>Grupo<br>Função<br>Equipe<br>Processo de aprovação<br>Caminho de aprovação<br>Etapa de aprovação<br>Aprovador da etapa<br>Agendar<br>Dia Não Útil<br>Definição da fila<br>Grupo de Tópicos de Fila<br>Enfileirar tópico<br>Regra de Encaminhamento<br>Caminho de Etapas<br>Etapa<br>Tipo de Hora<br>Conjunto de recursos<br>Categoria<br>Parâmetro da categoria<br>Parâmetro<br>Grupo de Parâmetros<br>Opção de parâmetro<br>Lógica de exibição da categoria |
| Modelo (TMPL) | Modelo<br>Modelo de Tarefa<br>Atribuição de Modelo de Tarefa<br>Predecessora da Tarefa de Modelo<br>Empresa<br>Taxa de substituição<br>Grupo<br>Função<br>Equipe<br>Processo de aprovação<br>Caminho de aprovação<br>Etapa de aprovação<br>Aprovador da etapa<br>Agendar<br>Dia Não Útil<br>Definição da fila<br>Grupo de Tópicos de Fila<br>Enfileirar tópico<br>Regra de Encaminhamento<br>Caminho de Etapas<br>Etapa<br>Tipo de Hora<br>Conjunto de recursos<br>Categoria<br>Parâmetro da categoria<br>Parâmetro<br>Grupo de Parâmetros<br>Opção de parâmetro<br>Lógica de exibição da categoria |

### Objetos de relatório

| Objeto promovível | Sub-objetos promovíveis incluídos |
| --- | --- |
| Modelo de layout (UITMPL) | Modelo de layout<br>Painel<br>Calendário<br>Seção de calendário<br>Página externa<br>Relatório<br>Filtro<br>Agrupamento<br>Exibir<br>Parâmetro |
| Painel (PTLTAB) | Painel<br>Calendário<br>Seção de calendário<br>Página externa<br>Relatório<br>Filtro<br>Agrupamento<br>Exibir<br>Parâmetro |
| Calendário (CALEND) | Calendário<br>Seção de calendário |
| Página externa (EXTSEC) | Página Externa |
| Relatório (PTLSEC) | Relatório<br>Filtro<br>Agrupamento<br>Exibir<br>Parâmetro |
| Filtro (UIFT) | Filtro<br>Parâmetro |
| Agrupamento (UIGB) | Agrupamento<br>Parâmetro |
| Visualização (UIVW) | Exibir<br>Parâmetro |

### Objetos de dados personalizados

| Objeto promovível | Sub-objetos promovíveis incluídos |
| --- | --- |
| Categoria (CTGY) | Categoria<br>Parâmetro da categoria<br>Parâmetro<br>Grupo de Parâmetros<br>Opção de parâmetro<br>Lógica de exibição da categoria<br>Grupo |
| Parâmetro (PARAM) | Parâmetro<br>Opção de parâmetro |
| Grupo de Parâmetros (PGRP) | Grupo de Parâmetros |

### Objetos da organização

| Objeto promovível | Sub-objetos promovíveis incluídos |
| --- | --- |
| Grupo (GRUPO) | Grupo <br>Subgrupos (até 5 níveis) *<br>Categoria<br>Parâmetro da categoria<br>Parâmetro<br>Grupo de Parâmetros<br>Opção de parâmetro<br>Lógica de exibição da categoria |
| Função (ROLE) | Função |
| Equipe (TEAM) | Equipe<br>Grupo |
| Empresa (CMPY) | Empresa<br>Taxa de substituição<br>Categoria<br>Parâmetro da categoria<br>Parâmetro<br>Grupo de Parâmetros<br>Parâmetro <br>Lógica de exibição da categoria<br>Grupo |
| Portfolio (PORTA) | Portfolio<br>Programa<br>Grupo<br>Categoria<br>Parâmetro da categoria<br>Parâmetro<br>Grupo de Parâmetros<br>Opção de parâmetro<br>Lógica de exibição da categoria |
| Programa (PRGM) | Programa<br>Portfolio<br>Grupo<br>Categoria<br>Parâmetro da categoria<br>Parâmetro<br>Grupo de Parâmetros<br>Opção de parâmetro<br>Lógica de exibição da categoria |

### Outros objetos de configuração

| Objeto promovível | Sub-objetos promovíveis incluídos |
| --- | --- |
| Processo de aprovação (ARVPRC) | Processo de aprovação<br>Caminho de aprovação<br>Etapa de aprovação<br>Aprovador da etapa<br>Função<br>Equipe<br>Grupo |
| Agendamento (SCHED) | Agendar<br>Dia Não Útil<br>Grupo |
| Caminho de Etapas (MPATH) | Caminho de Etapas<br>Etapa |
| Perfil da planilha de horas (TSPRO) | Perfil da Planilha de Horas<br>Tipo de Hora |
| Tipo de Hora (HOURT) | Tipo de hora |
| Tipo de Despesa (EXPTYP) | Tipo de Despesa |
| Tipo de Risco (RSKTYP) | Tipo de Risco |
| Conjunto de Recursos (RSPL) | Conjunto de Recursos |

\* Não disponível no momento


## Status de promoção do ambiente

Os pacotes de promoção de ambiente passam por vários status à medida que são criados e preparados para se moverem entre ambientes. Você pode ver esses status na lista de pacotes dentro do Workfront ou nas respostas da API, se estiver usando a API do Workfront.

Esses status incluem o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>MONTAGEM</td> 
   <td><p>Esse status é atribuído automaticamente enquanto os objetos estão sendo montados. </p><p>Montagem refere-se ao processo automatizado de identificação de objetos e subobjetos a serem incluídos em um pacote e adição desses objetos e seus dados ao pacote.</p><p>Este status não pode ser definido diretamente por um cliente.</p></td> 
  </tr> 
  <tr> 
   <td>RASCUNHO</td> 
   <td><p>Esse status é atribuído na conclusão de um processo de montagem ou ao criar um pacote de promoção vazio.</p><p>É possível que um cliente mova o pacote promocional de volta para esse status.</p><p>Enquanto estiver nesse status, o pacote de promoção não poderá ser instalado em nenhum ambiente.</p></td> 
  </tr> 
  <tr> 
   <td>TESTE</td> 
   <td><p>Esse status permite que um pacote de promoção seja instalado em qualquer sandbox de Pré-visualização ou Atualização personalizada. Enquanto estiver nesse status, o pacote não poderá ser instalado na Produção.</p></td> 
  </tr> 
  <tr> 
   <td>ATIVO</td> 
   <td><p>Esse status permite que um pacote de promoção seja instalado em qualquer ambiente, incluindo Produção.</p><p>Quando o status de um pacote é definido como ATIVO, a variável <code>publishedAt</code> A data é automaticamente definida para o carimbo de data e hora atual da solicitação.</p></td> 
  </tr> 
  <tr> 
   <td>DESATIVADO</td> 
   <td><p>Esse status será usado para ocultar pacotes de promoção usados anteriormente que não serão instalados em nenhum ambiente no futuro.</p><p>Quando um pacote está nesse status, ele não pode ser instalado em nenhum ambiente.</p><p>Quando o status de um pacote é definido como DESATIVADO, a variável <code>retiredAt</code> A data é automaticamente definida para o carimbo de data e hora atual da solicitação.</p><p>O uso deste status é recomendado em vez do uso de<code>DELETE /package</code> endpoint porque ele é recuperável e o histórico de instalação é retido para todas as implantações feitas com esse pacote.</p></td> 
  </tr> 
  <tr> 
   <td>FALHA_NA_MONTAGEM</td> 
   <td><p>O pacote promocional será colocado automaticamente nesse status se a etapa MONTAGEM falhar.</p><p>Para retornar o pacote para a etapa MONTAGEM, acione o processo de extração novamente.</p></td> 
  </tr> 
  </tbody> 
</table>


