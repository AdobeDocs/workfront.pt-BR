---
product-area: projects
navigation-topic: financials
title: Alterar a moeda do projeto
description: Como Gerente de projetos, você pode configurar um projeto para usar uma moeda diferente da moeda padrão do seu sistema Adobe Workfront. Isso permite exibir informações financeiras sobre o projeto na moeda desejada ao calcular custos e receita de mão de obra.
author: Alina
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# Alterar a moeda do projeto

Como Gerente de projetos, você pode configurar um projeto para usar uma moeda diferente da moeda padrão do seu sistema Adobe Workfront. Isso permite exibir informações financeiras sobre o projeto na moeda desejada ao calcular custos e receita de mão de obra.

Antes que você possa usar moedas alternativas conforme descrito nesta seção, o administrador do Workfront deve primeiro habilitar e configurar várias moedas, conforme descrito no artigo [Configurar taxas de câmbio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a projetos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Considerações ao alterar a moeda de um projeto no Workfront

* Não é possível alterar a moeda de um projeto se houver informações financeiras no projeto.
* As taxas são usadas para Custos de Mão-de-Obra; cálculos de receita e são usadas no futuro para fins de relatório.
* Se você não especificar uma moeda diferente para um projeto, a Workfront presume que a moeda do projeto é a moeda padrão do sistema. Para obter informações sobre a moeda padrão em nível de sistema, consulte [Configurar taxas de câmbio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* Por padrão, todos os usuários com licença completa têm acesso para exibir moedas e taxas de câmbio. O administrador do Workfront precisa conceder acesso administrativo adicional a **Taxas de câmbio** para permitir que os usuários definam taxas específicas em projetos.
* As taxas de câmbio no Workfront não são dinâmicas. O valor é definido por um administrador e deve ser atualizado quando ocorrerem alterações nas taxas de câmbio.
* Ao criar um relatório para refletir a moeda em um projeto, por padrão, todos os relatórios são agrupados pela moeda padrão do projeto. Se você criar um relatório com vários projetos com taxas de câmbio diferentes, quaisquer agrupamentos aplicados ao projeto refletirão a taxa de câmbio padrão no nível do sistema. Para obter mais informações, consulte o artigo [Criar relatórios de dados financeiros com taxas de câmbio exclusivas](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

## Configurar a moeda para um projeto

1. Vá para o projeto no qual deseja alterar a moeda padrão.

   >[!TIP]
   >
   >Certifique-se de que o projeto ainda não tenha nenhuma informação financeira. Por exemplo, verifique se não há Custos planejados ou reais associados ao projeto.

1. Clique em **Detalhes do projeto** no painel esquerdo e vá para a área **Finanças**.
1. Clique em **Adicionar** no campo **Moeda** e selecione a moeda que deseja usar como moeda padrão para o projeto. Todas as moedas que o administrador do Workfront definiu para a instância do Workfront são exibidas.

   ![](assets/currency-on-project-expanded-nwe.png)

1. (Condicional) Se você selecionar uma moeda diferente da moeda padrão definida para o sistema Workfront, especifique a taxa da moeda selecionada, pois ela está relacionada à moeda definida como a moeda base no sistema.
1. Clique em **Salvar alterações**.
