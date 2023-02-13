---
product-area: projects
navigation-topic: financials
title: Alterar a moeda do projeto
description: Como um Gerenciador de projetos, você pode configurar um projeto para usar uma moeda diferente da padrão para seu sistema Adobe Workfront. Isso permite que você exiba informações financeiras sobre o seu projeto na moeda desejada ao calcular custos de mão de obra e receita.
author: Alina
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# Alterar a moeda do projeto

Como um Gerenciador de projetos, você pode configurar um projeto para usar uma moeda diferente da padrão para seu sistema Adobe Workfront. Isso permite que você exiba informações financeiras sobre o seu projeto na moeda desejada ao calcular custos de mão de obra e receita.

Antes de usar moedas alternativas, conforme descrito nesta seção, o administrador do Workfront deve primeiro habilitar e configurar várias moedas, conforme descrito no artigo [Configurar taxas de câmbio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Considerações ao alterar a moeda de um projeto no Workfront

* Não é possível alterar a moeda de um projeto se houver informações financeiras no projeto.
* As taxas são utilizadas para os custos da mão de obra; Cálculos de receita e são usados no futuro para fins de relatório.
* Se você não especificar uma moeda diferente para um projeto, a Workfront partirá do princípio de que a moeda do projeto é a moeda padrão do sistema. Para obter informações sobre a moeda padrão no nível do sistema, consulte [Configurar taxas de câmbio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* Por padrão, todos os usuários da licença completa têm acesso para visualizar moedas e taxas de câmbio. O administrador do Workfront precisa conceder acesso administrativo adicional para **Taxas de câmbio** para permitir que os usuários definam taxas específicas em projetos.
* As taxas de câmbio no Workfront não são dinâmicas. O valor é definido por um administrador e deve ser atualizado quando ocorrerem alterações nas taxas de câmbio.
* Ao criar um relatório para refletir a moeda em um projeto, por padrão, todos os relatórios são agrupados pela moeda padrão do projeto. Se você criar um relatório com vários projetos com taxas de câmbio diferentes, quaisquer agrupamentos aplicados ao projeto refletirão a taxa de câmbio padrão no nível do sistema. Para obter mais informações, consulte o artigo [Criar relatórios de dados financeiros com taxas de câmbio exclusivas](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

## Configurar a moeda de um projeto

1. Vá para o projeto onde deseja alterar a moeda padrão.

   >[!TIP]
   >
   >Garantir que o projeto ainda não tenha informações financeiras. Por exemplo, verifique se não há Custos Planejados ou Reais associados ao projeto.

1. Clique em **Detalhes do projeto** no painel esquerdo, em seguida, vá para o **Finanças** área.
1. Clique em **Adicionar** no **Moeda** e selecione a moeda que deseja usar como a moeda padrão do projeto. Todas as moedas que o administrador do Workfront definiu para a instância do Workfront são exibidas.

   ![](assets/currency-on-project-expanded-nwe.png)

1. (Condicional) Se você selecionar uma moeda diferente da padrão definida para seu sistema Workfront, especifique a taxa para a moeda selecionada, pois ela se relaciona à moeda definida como a moeda base no sistema.
1. Clique em **Salvar alterações**.
