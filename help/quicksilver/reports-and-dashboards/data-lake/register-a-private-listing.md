---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Registrar uma lista privada para o Workfront Data Connect
description: Registre uma lista privada do Snowflake para compartilhar os dados do Workfront Data Connect diretamente com a conta da Snowflake de sua organização.
author: Courtney
feature: Reports and Dashboards
exl-id:
last-update: 2026-09-15T00:00:00.000Z
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: ed31fce397f9e99e7049d4f55eaca94f43dfcf5c
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 3%
---
# Registrar uma lista privada para o Workfront Data Connect

Você pode compartilhar os dados do Workfront Data Connect diretamente com a conta da Snowflake de sua organização registrando uma lista privada. Esse método de conexão usa o recurso de listagem privada da Snowflake para compartilhar dados com segurança entre organizações sem expô-los publicamente, e funciona em regiões e plataformas de hospedagem.

Uma lista privada é útil quando você deseja unir seus dados do Workfront a outros dados no data warehouse da empresa. Como os dados chegam à sua própria conta do Snowflake, você pode consultá-los junto com o restante dos dados.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td><p>Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Padrão</p>
   <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

Você também precisa de uma conta do Snowflake com permissões para aceitar listagens e criar bancos de dados, além de um direito do Workfront Data Connect.

## O que uma listagem privada compartilha

Uma lista privada oferece acesso ao seguinte:

* Mais de 100 visualizações de dados para objetos do Workfront. Para obter descrições de cada exibição, consulte o [dicionário de dados do Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md).
* As `*_event` visualizações de dados, que contêm cada transação de alteração entregue aos pipelines de dados da Conexão de Dados.
* Valores de dados personalizados para objetos extensíveis de dados. Para ver um exemplo, consulte o exemplo de consulta de dados personalizada em [exemplos de consulta da Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/basic-query-examples.md).

## Diferenças de uma conexão de conta de leitor

Uma lista privada compartilha um conjunto diferente de visualizações do que uma conexão de conta de leitor, e os dados chegam em uma programação diferente. Lembre-se das seguintes diferenças:

* Uma listagem privada compartilha somente as visualizações `*_event`. As exibições `*_current` e `*_daily_history` estão disponíveis por meio de uma conta de leitor, mas não por meio de uma lista privada. Você pode criá-los em sua própria conta da Snowflake. Para obter mais informações, consulte [Configurar exibições de Histórico Atual e Diário](#set-up-current-and-daily-history-views) neste artigo.
* Uma lista privada pode não incluir todas as visualizações disponíveis por meio de uma conta de leitor. Exemplos de exibições que não são compartilhadas incluem objetos do Workfront Planning, `MONITORING_DATA_REFRESHES`, `BOOKINGS` e `CLASSIFIER`. Esta lista não é exaustiva.
* O Data Connect carrega eventos de alteração a cada 4 horas. Como uma lista privada requer uma etapa de replicação adicional para exibir os dados, espera-se que os dados demorem cerca de 1 hora a mais para serem recebidos do que por meio de uma conta de leitor.
* A replicação de dados é executada às 01:01, 05:01, 09:01, 13:01, 17:01 e 21:01 UTC. Normalmente, os dados estão disponíveis em cerca de 10 minutos após cada execução.
* As exibições `MONITORING_DATA_REFRESHES` e `JOB_HISTORY` não refletem o momento em que os dados são disponibilizados por meio de uma lista privada. Embora a visualização `JOB_HISTORY` seja compartilhada por meio da lista privada, recomendamos lê-la por meio de uma conta de leitor para identificar trabalhos com falha mais rapidamente.

## Registrar uma lista privada

Para registrar uma lista privada, primeiro colete os detalhes da conta do Snowflake e adicione a lista no Workfront.

### Colete os detalhes da sua conta da Snowflake

O Workfront usa os detalhes da sua conta do Snowflake para direcionar a lista para sua conta. Obtenha os seguintes detalhes:

* Endereço da conta
* URL da conta
* Organização da conta
* Nome da conta

Cada um desses valores está disponível no modal Detalhes da conta no Snowflake.

Para localizar os detalhes da sua conta:

1. Enquanto estiver conectado na sua conta do Snowflake, clique no menu de usuário no canto inferior esquerdo.

1. Selecione sua conta na seção **Conta** do menu.

1. Clique em **Exibir detalhes da conta**.

1. Registre cada um dos valores listados acima.

Além disso, decida sobre o nome do banco de dados pelo qual você deseja acessar seus dados vinculados do Workfront. Insira esse nome ao registrar a lista.

### Adicionar a lista privada no Workfront

Registre a lista privada por meio da interface do Adobe Workfront.

>[!IMPORTANT]
>
>Você pode criar apenas uma lista privada por localizador de conta.

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Instalação**.

1. No painel esquerdo, clique em **Sistema** > **Conexão de Dados**.

1. Clique na guia **Conexões do Snowflake**.

1. Clique em **Adicionar lista privada**.

1. Preencha o formulário com os detalhes da conta coletados, incluindo o nome do banco de dados de sua preferência.

1. Clique em **Adicionar lista privada**.

### Conectar-se à lista no Snowflake

Na sua conta do Snowflake, estabeleça uma conexão com a lista privada como uma fonte de dados externa. Em seguida, você pode consultar os dados do Workfront junto com o restante dos dados.

## Configurar exibições do histórico atual e diário

Uma conexão de conta de leitor fornece três visualizações de dados para cada tabela de objetos:

* **Atual** — uma representação de baixa latência dos dados como eles existem atualmente no aplicativo de origem.
* **Histórico Diário** — uma representação dos dados como eram às 23:59 UTC para cada dia.
* **Evento** — cada transação de alteração entregue aos pipelines de dados da Conexão de Dados.

Uma listagem privada compartilha somente a visualização Evento. Esta seção fornece o SQL para criar as exibições Atual, Histórico diário e Evento na sua própria conta do Snowflake.

Todas as exibições de eventos incluídas na lista têm os campos necessários para a lógica de exibição abaixo. Esses exemplos assumem que você criou um novo banco de dados e esquema de sua escolha na conta do Snowflake de destino e usam a exibição `projects_event`. Em cada exemplo, substitua `<listing_db>` e `<listing_schema>` por seus próprios valores.

>[!TIP]
>
>Recomendamos que você substitua `select *` por uma lista das colunas usadas na análise. Se você usar `select *` e colunas forem adicionadas posteriormente ao modo de exibição de evento da lista, será necessário recriar o modo de exibição para habilitar as novas colunas.

### Exibições atuais

A exibição Atual de um objeto é o último registro de evento de alteração armazenado na Conexão de dados. Se o último registro estiver em um estado excluído, ele será omitido da exibição Atual. Todas as exibições de eventos têm a mesma estrutura.

```sql
create or replace view projects_current copy grants
as
select *
from <listing_db>.<listing_schema>.projects_event
where end_effective_timestamp = '2300-01-01'::timestamp_ntz
 and nvl(deleted, 0) != 1;
```

As colunas `deleted` e `end_effective_timestamp` não são necessárias na exibição Atual. A exibição filtra os dados em um único valor e remove o registro completamente se o registro for excluído.

### Exibições do histórico diário

A exibição Histórico Diário identifica o registro de evento de alteração que estava ativo às 23:59:59 de uma determinada data, para que você possa direcionar o estado do registro ao longo do tempo. O exemplo a seguir fornece o estado de um registro de projeto no final de cada dia.

```sql
create or replace view projects_daily_history copy grants
as
select d.calendardate as
 , p.*
from <listing_db>.<listing_schema>.calendar_dates d
join <listing_db>.<listing_schema>.projects_event p
 on p.begin_effective_timestamp <= d.calendareodtimestamp
and d.calendareodtimestamp < p.end_effective_timestamp
where d.calendareodtimestamp < current_date() - 1
 and nvl(deleted, 0) != 1;
```

### Visualizações de evento

Para fins de consistência, recomendamos que você crie uma cópia da visualização de eventos no banco de dados de listagem e a coloque no mesmo schema das visualizações Histórico atual e diário.

```sql
create or replace view projects_event copy grants
as
select *
from <listing_db>.<listing_schema>.projects_event;
```
