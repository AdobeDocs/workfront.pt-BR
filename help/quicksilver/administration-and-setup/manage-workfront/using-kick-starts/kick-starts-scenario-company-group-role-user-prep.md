---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: "Cenário de início: preparação da empresa, do grupo, da função e do usuário"
description: Ao implementar o Adobe Workfront, em vez de inserir dados manualmente, você pode importar a lista de clientes, os departamentos internos, as funções de trabalho e as informações do usuário.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b83e2e35-dd9d-4d98-b8d4-2f8718b3c6c1
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '1100'
ht-degree: 2%

---

# Cenário de lançamentos: empresa, grupo, função e preparação de lançamentos do usuário

Ao implementar o Adobe Workfront, em vez de inserir dados manualmente, você pode importar a lista de clientes, os departamentos internos, as funções de trabalho e as informações do usuário.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## O que pode ser importado

A tabela a seguir exibe as empresas, grupos e funções a serem importados:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Empresas</strong> </th> 
   <th><strong>Grupos</strong> </th> 
   <th><strong>Funções</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td valign="top"> <p>Acme, Co</p> <p>Workfront, Inc.</p> <p><em>Sua Empresa</em> </p> <p>XYZ, Inc.</p> </td> 
   <td valign="top"> <p valign="top" rowspan="7">Finanças</p> <p valign="top" rowspan="7">IT </p> <p valign="top" rowspan="7">Marketing </p> <p valign="top" rowspan="7">Vendas</p> </td> 
   <td valign="top"> <p valign="top">Analista de negócios</p> <p valign="top">Creative do controlador</p> <p valign="top">Designer</p> <p valign="top">Gerenciador de Recursos</p> <p valign="top">Scrum Master</p> <p valign="top">Redator técnico</p> <p valign="top">Desenvolvedor da Web</p> </td> 
  </tr> 
 </tbody> 
</table>

Os nomes das funções devem ser exclusivos. As funções de trabalho existentes não podem ser importadas.

As tabelas a seguir exibem os usuários a serem importados e vários atributos de usuário para cada um:

### Usuário 1

| **Nome** | Chris |
|---|---|
| **Sobrenome** | Tripulação |
| **Nome de Usuário/Email** | mailto:cmanning@foo.com |
| **Senha** | updateMe |
| **Acesso** | Integrante da Equipe |
| **Empresa** | &lt;*Sua Empresa>* |
| **Grupo Padrão** | Marketing |
| **Função** | Analista de negócios |

{style="table-layout:auto"}

### Usuário 2

| **Nome** | Jennifer |
|---|---|
| **Sobrenome** | Campbell |
| **Nome de Usuário/Email** | jcampbell@foo.com |
| **Senha** | updateMe |
| **Acesso** | Gerente de projeto |
| **Empresa** | &lt;*Sua Empresa>* |
| **Grupo Padrão** | Marketing |
| **Função** | Gerente de projeto |

{style="table-layout:auto"}

### Usuário 3

| **Nome** | Jill |
|---|---|
| **Sobrenome** | Sullivan |
| **Nome de Usuário/Email** | jsullivan@foo.com |
| **Senha** | updateMe |
| **Acesso** | Help Desk |
| **Empresa** | &lt;*Sua Empresa>* |
| **Grupo Padrão** | Vendas |
| **Função** | Representante de Vendas |

{style="table-layout:auto"}

### Usuário 4

| **Nome** | Marc |
|---|---|
| **Sobrenome** | Lewis |
| **Nome de Usuário/Email** | mlewis@foo.com |
| **Senha** | updateMe |
| **Acesso** | Gerente de Portfólio |
| **Empresa** | &lt;*Sua Empresa>* |
| **Grupo Padrão** | Finanças |
| **Função** | Controlador |

{style="table-layout:auto"}

### Usuário 5

| **Nome** | Pam |
|---|---|
| **Sobrenome** | Reynolds |
| **Nome de Usuário/Email** | preynolds@foo.com |
| **Senha** | updateMe |
| **Acesso** | Gerente de projeto |
| **Empresa** | *Sua Empresa>* |
| **Grupo Padrão** | Marketing |
| **Função** | IT |

{style="table-layout:auto"}

### Usuário 6

| **Nome** | Ray |
|---|---|
| **Sobrenome** | Andrews |
| **Nome de Usuário/Email** | randrews@foo.com |
| **Senha** | updateMe |
| **Acesso** | Administrador |
| **Empresa** | *Sua Empresa>* |
| **Grupo Padrão** | Gerenciador de Recursos |
| **Função** | nenhum |

{style="table-layout:auto"}

## Baixar um modelo de início

{{step-1-to-setup}}

1. Clique em **Sistema** > **Kick-Starts** > **Importar Dados.**

1. Clique em **Mais Opções** para ver a lista completa de opções de importação.
1. Selecione os objetos Nível de Acesso, Empresa, Grupo, Função de Trabalho e Usuário que você deseja importar.

## Inserir informações da empresa

1. Abra o arquivo **Workfront.xlsx** que você acabou de baixar.

   >[!TIP]
   >
   >Ao trabalhar com folhas de dados muito amplas, você pode usar a ferramenta Congelar painel do editor de planilhas (ou equivalente) para facilitar o trabalho com a planilha.

1. Vá para a folha &#39;Empresa CMPY&#39;.

   Deve ficar em branco, a menos que as empresas já estejam no sistema. ![](assets/cmpysheet-350x16.png)

   ![](assets/companyid--1--350x78.png)

1. Especifique VERDADEIRO na coluna **isNew**.
1. Repita essa ação para cada empresa que está sendo adicionada. (Neste exemplo, conclua esta ação para as linhas 3-6, pois quatro empresas estão sendo adicionadas.)

   ![](assets/cmpyisnew-350x86.png)

1. Especifique um identificador exclusivo.

   Isso deve ser feito para cada linha da coluna ID. Números inteiros iniciando em 1 funcionam bem ao criar novos registros.

   ![](assets/cmpyisnew-350x86.png)

1. Defina um Nome.

   Especifique os nomes de cada cliente na coluna **setName**.

   ![](assets/companyid-350x78.png)

1. Vá para a planilha Grupo.

   A menos que você já tenha criado grupos no Workfront, esta planilha deve exibir somente o Grupo padrão provisionado com cada conta do Workfront.

   ![](assets/groupsheet-350x15.png) ![](assets/emptygroupsheet-350x85.png)

1. Defina a coluna **isNew**. De acordo com o cenário, 4 grupos serão importados, portanto, especifique TRUE nas linhas 4 a 7 para a coluna &#39;isNew&#39;.
1. Especifique um identificador exclusivo.

   Isso deve ser feito para cada linha da coluna ID. Números inteiros iniciando em 1 funcionam bem ao criar novos registros.

   ![](assets/groupids-350x85.png)

1. Defina um Nome.

   Especifique os nomes de cada departamento na coluna **setName**.

   ![](assets/groupnames-350x85.png)

   Especifique as informações da função. Vá para a planilha Função.

1. A menos que você já tenha criado ou excluído funções em sua conta, esta planilha deve exibir 8 funções provisionadas com cada conta do Workfront.

   ![](assets/groupnames-350x85.png)

1. Definir instrução True.

   Sete funções de trabalho estão importando, insira TRUE nas linhas 12 a 18 da coluna &quot;isNew&quot;.

   ![](assets/roleisnew-350x104.png)

1. Especifique um identificador exclusivo.

   Isso deve ser feito para cada linha da coluna ID. Números inteiros iniciando em 1 funcionam bem ao criar novos registros.

   ![](assets/usersheet-350x16.png)

   ![](assets/roleisnew--1--350x104.png)

1. Forneça nomes para cada função digitando-a na coluna setName.

   ![](assets/roleisnew-350x104.png)

1. Forneça detalhes adicionais, conforme necessário.

   Inclua taxas de faturamento, taxas de custo e descrições para as Funções que você está criando, conforme necessário.

1. Vá para a planilha Usuário para inserir Informações do Usuário.

   A menos que você já tenha criado usuários em sua conta, esta planilha deve exibir somente o Usuário administrador que é provisionado com cada conta do Workfront.

   ![](assets/rolenames-350x104.png) ![](assets/emptyusersheet-350x52.png)

1. Defina o valor Verdadeiro especificando TRUE nas linhas 4 a 9 para a coluna &#39;isNew&#39;, já que 6 usuários estão sendo importados.

   ![](assets/userisnew-350x52.png)

1. Defina um identificador exclusivo especificando um identificador exclusivo em cada linha para a coluna de ID. Normalmente, números inteiros começando em 1 funcionam bem para novos registros.

   ![](assets/userisnew-350x52.png)

1. Insira os nomes de cada usuário nas colunas &#39;setFirstName&#39; e &#39;setLastName&#39;.

   ![](assets/usernames-350x52.png)

1. Defina valores detalhados especificando valores nas colunas &#39;setEmail&#39;, &#39;setPassword&#39; e &#39;setUsername&#39;.

   ![](assets/usercredentials-350x52.png)

1. Especifique os valores de Nível de Acesso.

   Por exemplo, Chris Manning, que é um Integrante da equipe, procure a ID na folha Nível de acesso ACSLVL para o nível de acesso do Integrante da equipe. Copie a ID na área de transferência e, na planilha USUÁRIO, cole-a na coluna **setAccessLevelID** da linha de Chris.

   Repita essa etapa para cada usuário e nível de acesso.

   ![](assets/copyalid-350x171.png) ![](assets/pastealid-350x59.png)

1. Especificar detalhes do Grupo Padrão.

   De acordo com o cenário, Chris Manning pertence ao grupo Marketing. Na planilha Grupo, localize a ID do grupo de Marketing, copie-a para a área de transferência e, na planilha USUÁRIO, cole-a na coluna **setHomeGroupID** da linha de Chris. &#x200B;Repita essa etapa para cada atribuição de usuário e grupo.

   ![](assets/copygroupid-1-350x133.png) ![](assets/pastegroupid-350x59.png)

1. Especifique Detalhes da empresa.

   Todos os usuários neste cenário pertencem à mesma empresa. Na planilha CÓPIA da empresa, localize a ID da *Sua própria empresa *empresa, copie a ID na área de transferência e, na guia USUÁRIO, cole esse valor em cada linha da coluna &#39;setCompanyID&#39;.&#x200B;

   Repita essa etapa para cada atribuição de usuário e grupo.

   ![](assets/companyid--1--350x78.png)

   ![](assets/pastecompanyid-350x84.png)

1. Especifique os detalhes da Função.

   De acordo com o cenário, Chris Manning terá a função de Analista de negócios. Na planilha Função Função, localize a ID da função Analista de negócios, copie-a para a área de transferência e, na planilha Usuário, cole-a na coluna &quot;setRoleID&quot; na linha de Chris. &#x200B;Repita essa etapa para cada atribuição de usuário e grupo.

   ![](assets/copyroleid-350x149.png)

   ![](assets/pasteroleid-350x95.png)

1. Preencha outros detalhes do usuário, conforme necessário, e salve o arquivo.
1. Importe o arquivo do Excel.

   Siga as instruções fornecidas em [Importar dados para o Adobe Workfront usando um modelo de Kick-Start](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
