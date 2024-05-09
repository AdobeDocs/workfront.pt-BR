---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Instale o Visualizador de provas de desktop na sua organização
description: O Desktop Proofing Viewer, projetado principalmente para revisar conteúdo interativo, é um aplicativo que deve ser instalado no computador local de cada usuário. Como administrador do Adobe Workfront ou administrador do Workfront Proof, você pode executar essa instalação.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: c89b21c6-fe70-4f46-aebd-5b82a667db72
source-git-commit: 5cc1acffff12d78e48228f3ae223514c0ff379ef
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Instale o Visualizador de provas de desktop na sua organização

<!--Audited: 05/2024-->

O Desktop Proofing Viewer, projetado principalmente para revisar conteúdo interativo, é um aplicativo que deve ser instalado no computador local de cada usuário. Como administrador do Adobe Workfront ou administrador do Workfront Proof, você pode executar essa instalação.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Plano atual: Pro ou Superior</p> <p>ou</p> <p>Plano herdado: Premium ou Select</p> <p>Para obter mais informações sobre acesso de prova com os diferentes planos, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de prova no Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Plano atual: Trabalho ou Plano</p> <p>Plano herdado: Qualquer um (Você deve ter a prova ativada para o usuário)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>É necessário ter Administrador selecionado no seu Perfil de permissão de prova. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configurar o acesso à prova de um usuário</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Requisitos do sistema

O Desktop Proofing Viewer é suportado nos seguintes sistemas operacionais:

* Windows 7 e posterior, 32 bits e 64 bits
* Mac OS X 10.9 e posterior, 64 bits

## Pré-requisitos

Para permitir que os usuários usem o Desktop Proofing Viewer, você deve configurar o sistema para iniciar o Desktop Proofing Viewer como a visualização padrão para provas interativas antes da instalação.

## Configure o Visualizador de provas de desktop como padrão para provas interativas

Depois de instalar o Visualizador de provas de desktop na sua organização, você pode defini-lo como o visualizador padrão para provas interativas.

{{step1-to-proofing}}

1. Clique em **Configurações da conta** próximo ao canto superior direito do Workfront Proof e clique na guia **Configurações** guia.

1. Em **Padrões de prova**, no final do **Visualizador de provas de desktop para provas interativas** clique em **Configuração**.

   ![Padrões de prova](assets/proof-defaults.png)

1. Clique em **Ativado e padrão** e, em seguida, clique em **Salvar**.

## Instalação do Visualizador de provas de desktop para seus usuários

* [Instalação do Visualizador de provas de desktop no Mac](#installing-the-desktop-proofing-viewer-on-mac)
* [Instalação do Visualizador de provas de desktop no Windows](#installing-the-desktop-proofing-viewer-on-windows)

### Instalação do Visualizador de provas de desktop no Mac {#installing-the-desktop-proofing-viewer-on-mac}

1. No computador do usuário, siga um destes procedimentos para baixar o aplicativo:

   * Se estiver usando o ambiente de Produção, clique em [Download de produção do Mac para o visualizador de provas de desktop](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof-2.1.19.pkg).
   * Se estiver usando o ambiente de Pré-visualização, clique em [Download da visualização do Mac para o visualizador de provas de desktop](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview-2.1.19.pkg).

1. Abra o arquivo que acabou de baixar para iniciar a instalação.
1. Na caixa de instalação exibida, clique em **Continuar** e, em seguida, clique em **Instalar**.

   ![Caixa de instalação](assets/install-wf-proof-box.png)

1. Certifique-se de que cada usuário conclua a instalação abrindo uma prova interativa na área Documentos do Workfront.

### Instalação do Visualizador de provas de desktop no Windows {#installing-the-desktop-proofing-viewer-on-windows}

1. No computador do usuário, siga um destes procedimentos para baixar o aplicativo:

   * No ambiente de Produção, clique em [Download de Produção do Windows para o Visualizador de Revisão de Texto para Desktop](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Setup+2.1.19.exe).
   * No ambiente de Pré-visualização, clique em [Download da Visualização do Windows para o Visualizador de Revisores de Texto para Desktop](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview+Setup+2.1.19.exe).

1. Abra o arquivo que acabou de baixar para iniciar a instalação.
1. Na caixa de aviso de segurança exibida, clique em **Executar**.

   ![Screen_Shot_2018-05-02_at_10.56.55_AM.png](assets/screen-shot-2018-05-02-at-10.56.55-am-350x271.png)

   O Desktop Proofing Viewer instala e executa.

1. (Condicional) Se você instalar o aplicativo usando o Internet Explorer, atualize a página de inicialização no navegador depois que o aplicativo for instalado.
1. Certifique-se de que cada usuário conclua a instalação abrindo uma prova interativa na área Documentos do Workfront.
