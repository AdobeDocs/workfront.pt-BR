---
product-area: documents
navigation-topic: approvals
title: Configurar marcas para o Revisor do AI
description: Configurar marcas para o Revisor do AI
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
source-git-commit: cf1d4bfeedb94e8607dad47177d804169254ee85
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 5%

---

# Configurar marcas para o Revisor do AI

>[!IMPORTANT]
>
>No momento, esse recurso está na versão beta.

O Revisor da IA usa diretrizes da marca para avaliar o conteúdo durante o processo de revisão. Você pode criar marcas no Workfront fazendo upload de arquivos PDF que contêm as diretrizes da marca ou inserindo manualmente os elementos da marca.

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
   <td role="rowheader">Permissões do Admin Console</td> 
   <td> <p>Você deve ter o GenStudio Brand Manager.</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Pré-requisitos

* Sua organização deve ter migrado para o Adobe IMS (Identity Management System).
* Sua instância do Workfront deve ter as Aprovações unificadas habilitadas.
  <!--* Your organization must have GenStudio Foundation.-->
* A Adobe deve ter um contrato de API Gen da Adobe assinado no arquivo.
Para obter mais informações sobre como assinar o contrato, consulte [Assinar o contrato da Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).

## Criar uma marca usando uma PDF

{{step-1-to-setup}}

1. No painel esquerdo, vá para **Análise e Aprovação** > **Marcas**.
1. Clique em **Adicionar marca** no canto superior direito da tela.
1. Dê um nome à marca.
1. Clique em Fazer upload de PDFs para fazer upload de arquivos de marca.
   ![carregar pdfs de marca](assets/upload-PDF.png)
1. Clique em **Continuar**.
1. Carregue um ou mais arquivos PDF que contenham as diretrizes da sua marca, em seguida, clique em **Adicionar marca**.
1. Depois que os arquivos forem carregados, analise os elementos de marca extraídos para garantir que eles estejam alinhados às diretrizes da sua marca.

   >[!IMPORTANT]
   >
   >As diretrizes são geradas usando seus arquivos e a tecnologia de IA gerativa e podem ser imprecisas. Revise as diretrizes extraídas para ver detalhes ausentes ou incorretos e edite-os antes de publicar esta marca.

1. Quando terminar, clique em **Publicar** para disponibilizar a marca para o Revisor da IA.

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
        <td>logotipos</td>
        <td>Incluir os logotipos oficiais associados à marca.</td>
    </tr>
    <tr>
        <td>Cores</td>
        <td>Especificar a paleta de cores da marca.</td>
    </tr>
    </table>

   ![adicionar elementos de marca manualmente](assets/brand-elements.png)


1. Quando terminar, clique em **Publicar** para disponibilizar a marca para o Revisor da IA.
