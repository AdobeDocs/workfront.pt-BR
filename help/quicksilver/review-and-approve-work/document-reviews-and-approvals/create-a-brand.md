---
product-area: documents
navigation-topic: approvals
title: Criar e gerenciar marcas para o Revisor de conteúdo
description: Criar e gerenciar marcas para o Revisor de conteúdo
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b2788f3f-43d2-46f3-8502-bb833f8a0970
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 2b3e2ac00126facab9cc45ba8fb193d8951a37ec
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 9%

---

# Criar e gerenciar marcas para o Revisor de conteúdo

{{highlighted-preview-article-level}}

O Revisor de conteúdo usa diretrizes de marca para avaliar o conteúdo durante o processo de revisão. Você pode criar marcas no Workfront fazendo upload de arquivos PDF que contêm as diretrizes da marca ou inserindo manualmente os elementos da marca.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Padrão</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do sistema.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões do Admin Console*</td> 
   <td> <p>Você deve ser um Gerente de marca da GenStudio.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos

* Sua instância do Workfront deve ter as Aprovações unificadas habilitadas.

* Sua organização deve ter o GenStudio Foundation.
   * O Revisor de conteúdo no Workfront fornece a funcionalidade disponível no GenStudio Foundation para revisão de ativos e fluxos de trabalho de aprovação. Não é necessário acessar o GenStudio Foundation diretamente para concluir o trabalho. Seu acesso à funcionalidade do GenStudio Foundation por meio do Revisor de conteúdo se enquadra nos termos de seu contrato com a Workfront.
* A Adobe deve ter um contrato de API Gen da Adobe assinado no arquivo.
Para obter mais informações sobre como assinar o contrato, consulte [Assinar o contrato da Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).


## Pré-requisitos

1. Você deve conceder acesso às permissões de marca nos níveis de acesso da Admin Console e da Workfront antes de criar marcas. Para obter instruções, consulte [Conceder acesso às permissões de marca](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md).


## Criar uma marca usando uma PDF

{{step-1-to-setup}}

1. No painel esquerdo, vá para **Análise e Aprovação** > **Marcas**.
1. Clique em **Adicionar marca** no canto superior direito da tela.
1. Dê um nome à marca.
1. Clique em **Carregar PDFs** para carregar arquivos de marca.
   ![carregar pdfs de marca](assets/upload-PDF.png)
1. Clique em **Continuar**.
1. Carregue um ou mais arquivos PDF que contenham as diretrizes da sua marca, em seguida, clique em **Adicionar marca**.
1. Depois que os arquivos forem carregados, analise os elementos de marca extraídos para garantir que eles estejam alinhados às diretrizes da sua marca.

   >[!IMPORTANT]
   >
   >As diretrizes são geradas usando seus arquivos e a tecnologia de IA gerativa e podem ser imprecisas. Revise as diretrizes extraídas para ver detalhes ausentes ou incorretos e edite-os antes de publicar esta marca.

1. Quando terminar, clique em **Publicar** para disponibilizar a marca para o Revisor de Conteúdo.

## Criar uma marca manualmente

{{step-1-to-setup}}

1. No painel esquerdo, vá para **Análise e Aprovação** > **Marcas**.
1. Clique em **Adicionar marca** no canto superior direito da tela.
1. Dê um nome à marca.
1. Clique em **Adicionar manualmente** para criar uma marca com elementos individuais.
1. Preencha os detalhes da marca conforme necessário. Você pode adicionar os seguintes elementos:

   <table>
    <tr>
        <td>Quando usar</td>
        <td>Informe aos profissionais de marketing quando usar essa marca.</td>
    </tr>
    <tr>
        <td>Diretrizes de voz</td>
        <td>Forneça orientação sobre o tom e o estilo da voz da marca.</td>
    </tr>
    <tr>
        <td>Diretrizes de imagem</td>
        <td>Especifique os tipos de imagens que se alinham com a identidade da marca.</td>
    </tr>
    <tr>
        <td>Diretrizes do canal</td>
        <td>Descreva os canais apropriados para a comunicação da marca.</td>
    </tr>
    <tr>
        <td>Logotipos</td>
        <td>Incluir os logotipos oficiais associados à marca.</td>
    </tr>
    <tr>
        <td>Cores</td>
        <td>Especificar a paleta de cores da marca.</td>
    </tr>
    </table>

   ![adicionar elementos de marca manualmente](assets/brand-elements.png)


1. Quando terminar, clique em **Publicar** para disponibilizar a marca para o Revisor de Conteúdo.
