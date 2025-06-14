---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: Introdução à integração do GenStudio for Performance Marketing e do Workfront Proof
description: Introdução à integração do GenStudio for Performance Marketing e do Workfront Proof
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 9905a522-9913-49c0-8c80-a8b46221fcbb
source-git-commit: 4b0ba0112138b91b12e10f4770ecab3db4e3fddb
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Introdução à integração do GenStudio for Performance Marketing e do Workfront Proof

Com a integração entre o GenStudio for Performance Marketing e o Workfront Proof, você pode

* Usar modelos de prova do Workfront para definir workflows de revisão e aprovação

* Revisar e aprovar o conteúdo de rascunho do GenStudio for Performance Marketing no visualizador de provas do Workfront

* Exibir decisões de revisão no GenStudio for Performance Marketing para aprovação final e publicação

Para obter mais informações sobre revisão e aprovação no GenStudio for Performance Marketing, consulte [Integração do Workfront Proof com o GenStudio for Performance Marketing](https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/approve/proof-integration).


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> 
   <p>Qualquer</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Atual: Padrão </p> 
   <p>Herdados: plano </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td> 
   <p> Você deve ter o GenStudio for Performance Marketing e ser adicionado ao produto como um usuário no Admin Console. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a projetos</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Requisitos de integração

* O Workfront e o GenStudio for Performance Marketing devem ser implantados na mesma Organização IMS.

* Os usuários podem pertencer a apenas uma instância do Workfront na organização IMS.

* A instância do Workfront deve ser ativada na Adobe Unified Experience.

* A integração deve ser habilitada na área Configuração do Workfront.


## Habilitar a integração no Workfront

Você deve ser um administrador do sistema para habilitar essa integração.

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique no ícone **[!UICONTROL Instalação]** ![Instalação](/help/_includes/assets/gear-icon-setup.png).
1. No painel esquerdo, clique em **Revisar e aprovar** > **Adobe GenStudio**.
1. Habilitar **Usar aprovações de prova**.
   ![habilitar revisão de texto para a configuração do GenStudio](assets/enable-proofing-gs.png)

## Usar modelos de prova do Workfront para definir workflows de aprovação

Se o processo de revisão de conteúdo de sua organização for repetido com frequência ou revisado pelas mesmas pessoas, você poderá usar modelos de prova para automatizar os fluxos de trabalho de revisão e aprovação.

### Criar um modelo de prova no Workfront

É possível criar modelos simples, de estágio único, para apenas um ou dois revisores, ou criar modelos automatizados, de vários estágios para revisões complexas com muitos estágios e dependências.

Para obter mais informações sobre como criar workflows e modelos automatizados no Workfront, consulte

* [Visão geral do fluxo de trabalho automatizado](/help/quicksilver/review-and-approve-work/proofing/proofing-overview/automated-workflow.md)
* [Criar e gerenciar modelos de fluxo de trabalho automatizado](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md)

### Escolher ou modificar o modelo no GenStudio for Performance Marketing

Quando um usuário inicia uma revisão no GenStudio for Performance Marketing, ele simplesmente escolhe o modelo necessário. Os usuários podem alterar facilmente qualquer modelo de fluxo de trabalho de prova, adicionando ou removendo revisores e estágios, a qualquer momento.

Para obter mais informações, consulte [Solicitar revisão e aprovação](https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/approve/request-review).

## Revisar e aprovar o conteúdo de rascunho do GenStudio for Performance Marketing no visualizador de provas do Workfront

Você pode revisar e aprovar o conteúdo de rascunho diretamente no GenStudio for Performance Marketing no visualizador de provas do Workfront.

Com o revisor de provas, você pode

* Deixar comentários
* Marcar rascunho para mostrar o que precisa ser alterado
* Tomar uma decisão

Para obter mais informações, consulte [Revisar e editar conteúdo](https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/approve/review-and-edit).


>[!IMPORTANT]
>
>Os usuários devem instalar o [Revisar conteúdo interativo com a ferramenta de revisão do Adobe Workfront](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-proof-in-web-viewer-extension.md) antes de começar a revisar rascunhos no GenStudio for Performance Marketing.


## Exibir decisões de revisão no GenStudio for Performance Marketing para aprovação final e publicação

Depois que o ativo tiver passado pelo processo de revisão e aprovação, você poderá visualizar a decisão de revisão e publicar o conteúdo diretamente do GenStudio for Performance Marketing.

Para obter mais informações, consulte [Publicar conteúdo aprovado](https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/approve/publish-content).
