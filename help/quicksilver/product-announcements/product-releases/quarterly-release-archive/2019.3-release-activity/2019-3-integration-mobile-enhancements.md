---
product-previous: mobile
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: Integração 2019.3 e melhorias móveis
description: Esta página descreve todas as alterações, integração e aprimoramentos móveis feitos na versão 2019.3. Ele será disponibilizado no ambiente de Produção na semana de 19 de agosto de 2019.
author: Luke
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 15e03405-63ff-48ea-b873-cf44f1f46282
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Integração 2019.3 e melhorias móveis

Esta página descreve todas as alterações, integração e aprimoramentos móveis feitos na versão 2019.3. Ele será disponibilizado no ambiente de Produção na semana de 19 de agosto de 2019.

Para obter uma lista de todas as alterações feitas em 2019.3, consulte a [visão geral da atividade da versão 2019.3](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md).

## Suporte a itens compartilhados na integração com o MS OneDrive

Agora você pode vincular seus arquivos e pastas compartilhados do OneDrive a objetos do Workfront. Por outro lado, você pode carregar arquivos no Workfront para pastas compartilhadas no OneDrive.

Para obter mais informações, consulte as seções [Vincular um documento externo ao Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents), [Vincular uma ou mais pastas externas](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-a-folder) e [Atualizar e vincular um documento do Workfront a um provedor de nuvem externo](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) no artigo [Vincular documentos de aplicativos externos](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Para obter informações, consulte a seção [Vincular um documento externo ao Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) no artigo [Vincular documentos de aplicativos externos](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Especificação de domínio necessária para todos os logons da Workfront

Todos os logons do Workfront agora exigem que o usuário especifique o domínio se ele ainda não estiver especificado no URL do Workfront. Solicitar essas informações torna sua instância do Workfront mais segura. Além disso, se a sua implementação do Workfront tiver várias instâncias, esse aprimoramento permitirá adicionar o mesmo usuário a cada instância do Workfront na implementação.

Essa alteração pode afetar os logons de usuário e as integrações da API:

* **Logons de usuário**

  Se o domínio da sua empresa não estiver incluído no URL do Workfront, você verá um novo campo Domínio na tela de logon, além dos campos Nome de usuário e Senha.

  Para a maioria dos clientes, nenhuma alteração é necessária porque as informações de domínio já estão incluídas no URL do Workfront. Por exemplo, &quot;*domínio*.my.workfront.com.&quot;

* **Integrações de API**

  Se você tiver qualquer código API indo para um endereço que não inclui seu nome de domínio, esse código API não funcionará mais.

Para obter mais informações, consulte [Fazer logon no Adobe Workfront](../../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/log-in-to-workfront.md).

## Converter tarefas e problemas em projetos usando o aplicativo móvel no iOS

Agora você pode converter tarefas e problemas individuais em projetos no aplicativo móvel do Workfront no iOS.

## Faça logon no aplicativo móvel com impressão digital ou ID facial

Dependendo do dispositivo, você pode optar por fazer logon no aplicativo móvel do Workfront usando a tecnologia de impressão digital ou ID facial. Ao fazer logon no aplicativo móvel, ele perguntará se você deseja fazer logon usando o método de autenticação compatível com seu telefone.

Para obter mais informações sobre como gerenciar este recurso, consulte [Adobe Workfront para iOS](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md) ou [Adobe Workfront para Android](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md).

## Nova configuração para desconectar usuários automaticamente em dispositivos móveis

Para tornar o aplicativo móvel Workfront mais seguro para você e sua empresa, os usuários serão desconectados automaticamente após 15 dias de inatividade. Os administradores do Workfront podem personalizar esse limite de tempo no aplicativo web em Configurar > Sistema > Preferências.

Para obter mais informações, consulte [Configurar preferências de segurança do sistema](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## O Aplicativo Móvel Exige Um Domínio Ao Fazer Logon

Como melhoria de segurança, o aplicativo móvel do Workfront agora exige que você forneça seu domínio se não fizer logon com credenciais de Logon único.

>[!NOTE]
>
>Disponibilidade do iOS: 12 de junho de 2019
>
>Disponibilidade de produção: 17 de junho de 2019

## Excluir objetos usando o aplicativo para dispositivos móveis no iOS

>[!NOTE]
>
>Esse recurso foi disponibilizado nas lojas de aplicativos para o iOS na semana de 19 de agosto de 2019.

Agora você pode excluir objetos como tarefas, problemas e folhas de horas no aplicativo móvel do iOS. Você deve ter as permissões corretas no objeto para excluí-lo.

## Filtrar por projetos inativos no aplicativo móvel

>[!NOTE]
>
>Esse recurso estará disponível nas lojas de aplicativos para iOS e Android na semana de 19 de agosto de 2019.

Adicionamos Projetos mortos como opção de filtro na guia Projetos do aplicativo móvel.

## Redefina sua senha usando o aplicativo móvel

Você pode usar o aplicativo Workfront Mobile para redefinir sua senha caso a tenha esquecido. Toque em Esqueceu a senha? e siga as instruções na tela. Não é possível redefinir a senha do SSO no aplicativo móvel.

## Nova aparência para dispositivos móveis

Adicionamos as seguintes melhorias de aparência para aprimorar sua experiência no aplicativo móvel do Workfront.

* Os itens a seguir foram movidos da barra superior da página Detalhes para áreas mais proeminentes da tela:

   * O ícone de adição agora está no canto inferior esquerdo da tela
   * A marca de seleção para começar a trabalhar em um item agora é um botão Trabalhar nisso na parte superior central da tela

* Agora é possível exibir os formulários personalizados anexados tocando em Mostrar mais na parte inferior da página Detalhes.
* Alteração da aparência das páginas usadas para enviar tarefas, problemas e solicitações.

