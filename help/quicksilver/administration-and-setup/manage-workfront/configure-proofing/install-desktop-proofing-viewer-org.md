---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Instale o Desktop Proofing Viewer para sua organização
description: O Desktop Proofing Viewer, desenvolvido principalmente para verificar conteúdo interativo, é um aplicativo que deve ser instalado na máquina local de cada usuário. Como administrador do Adobe Workfront ou administrador do Workfront Proof, você pode executar essa instalação.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: c89b21c6-fe70-4f46-aebd-5b82a667db72
source-git-commit: 58f976d9f4245e528a4ddf23d39b92d9fa405311
workflow-type: tm+mt
source-wordcount: '591'
ht-degree: 0%

---

# Instale o Desktop Proofing Viewer para sua organização

O Desktop Proofing Viewer, desenvolvido principalmente para verificar conteúdo interativo, é um aplicativo que deve ser instalado na máquina local de cada usuário. Como administrador do Adobe Workfront ou administrador do Workfront Proof, você pode executar essa instalação.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Plano atual: Pro ou superior</p> <p>ou</p> <p>Plano herdado: Premium ou Selecionar</p> <p>Para obter mais informações sobre como revisar o acesso com os diferentes planos, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de prova no Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano atual: Trabalho ou Plano</p> <p>Plano herdado: Qualquer (É necessário ter a prova ativada para o usuário)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ter o Administrador selecionado em seu Perfil de permissão de prova. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configurar o acesso à prova de um usuário</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Requisitos do sistema

O Desktop Proofing Viewer é compatível com os seguintes sistemas operacionais:

* Windows 7 e posterior, 32 bits e 64 bits
* Mac OS X 10.9 e posterior, 64 bits

## Pré-requisitos

Para permitir que os usuários usem o Desktop Proofing Viewer, você deve

* Configure o sistema para iniciar o Desktop Proofing Viewer como a exibição padrão para provas interativas antes da instalação.

## Configure o Desktop Proofing Viewer como padrão para provas interativas

Depois de instalar o Desktop Proofing Viewer para sua organização, você pode defini-lo como visualizador padrão para provas interativas.

1. No Workfront, clique no Menu principal ![](assets/main-menu-icon.png)e, em seguida, clique em Verificação ![](assets/proofing-in-main-menu.png) para acessar o Workfront Proof.

1. Clique em **Configurações da conta** próximo ao canto superior direito da Workfront Proof, clique no botão **Configurações** guia .

1. Em **Padrões de prova** no final do **Visualizador de prova de desktop para prova interativa** , clique em **Configuração**.

   ![](assets/proof-defaults-350x265.png)

1. Clique em **Ativado e padrão**, depois clique em **Salvar**.

## Instalar o visualizador de prova de desktop para seus usuários

* [Instalar o visualizador de prova de desktop no Mac](#installing-the-desktop-proofing-viewer-on-mac)
* [Instalar o visualizador de prova de Desktop no Windows](#installing-the-desktop-proofing-viewer-on-windows)

### Instalar o visualizador de prova de desktop no Mac {#installing-the-desktop-proofing-viewer-on-mac}

1. Na máquina do usuário, execute um dos seguintes procedimentos para baixar o aplicativo:

   * Se você estiver usando o ambiente de Produção, clique em  [Download de produção do Mac para o visualizador de prova de desktop.](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof-2.1.19.pkg)
   * Se estiver usando o ambiente de Visualização, clique em  [Download da visualização do Mac para o visualizador de prova de desktop.](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview-2.1.19.pkg)
)

1. Abra o arquivo que acabou de baixar para iniciar a instalação.
1. Na caixa de instalação exibida, clique em **Continuar**, depois clique em **Instalar**.

   ![00000776.png](assets/00000776-350x244.png)

1. Certifique-se de que cada usuário conclua a instalação abrindo uma prova interativa da área Documents no Workfront.

### Instalar o visualizador de prova de Desktop no Windows {#installing-the-desktop-proofing-viewer-on-windows}

1. Na máquina do usuário, execute um dos seguintes procedimentos para baixar o aplicativo:

   * No ambiente Produção, clique em [Download de produção do Windows para o Visualizador de Verificação de Verificação de Verificação de Verificação de Desktop.](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Setup+2.1.19.exe)
   * No ambiente de Visualização, clique em [Download da Visualização do Windows para o Visualizador de Verificação Linguística da Área de Trabalho](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview+Setup+2.1.19.exe).

1. Abra o arquivo que acabou de baixar para iniciar a instalação.
1. Na caixa de aviso de segurança exibida, clique em **Executar**.

   ![Screen_Shot_2018-05-02_at_10.56.55_AM.png](assets/screen-shot-2018-05-02-at-10.56.55-am-350x271.png)

   O Desktop Proofing Viewer instala e executa.

1. (Condicional) Se você instalar o aplicativo usando o Internet Explorer, atualize a página de inicialização no navegador após a instalação do aplicativo.
1. Certifique-se de que cada usuário conclua a instalação abrindo uma prova interativa da área Documents no Workfront.
