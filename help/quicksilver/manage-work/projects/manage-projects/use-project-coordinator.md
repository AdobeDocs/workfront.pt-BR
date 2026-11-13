---
title: Usar o colaborador do Coordenador de projetos
content-type: reference
description: Saiba como usar o Coordenador de projetos, um colaborador de IA pronto para uso que monitora o status do projeto e acompanha tarefas vencidas.
author: Becky
feature: Work Management, Projects
source-git-commit: 13403cc11448a0611ad0996ed21e1745277e9c05
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 6%

---
# Usar o colaborador do Coordenador de projetos

{{highlighted-preview-article-level}}

O Coordenador de projetos é um colaborador de IA pronto para uso que monitora o projeto e notifica as partes interessadas sobre informações importantes de status.

O uso de um Coordenador de projetos não requer que você configure um agente fora do Workfront.

Para obter instruções sobre como configurar um Coordenador de projetos, consulte [Configurar um Coordenador de projetos](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-project-coordinator) no artigo Configurar colaboradores de IA.

Para obter informações sobre o AI Collaborators em geral, consulte [Configurar o AI Collaborators](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacote</td> 
   <td><p>Select, Prime ou Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licença</td> 
   <td><p>[!UICONTROL Padrão]</p></td>
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td>Você deve ter a permissão Gerenciar para que os projetos atribuam um Coordenador de projetos.</td> 
  </tr>
  </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visão geral do coordenador de projetos

O Coordenador de projetos monitora seu projeto e ajuda a manter o trabalho no caminho certo. Quando atribuído a um projeto, ele envia atualizações de projeto em um agendamento que o administrador configura. As atualizações podem incluir:

* Um resumo do progresso
* Integridade do projeto
* Tarefas ou aprovações atrasadas ou em risco
* Campos ou atribuições ausentes

O coordenador do projeto também pode comentar sobre o projeto e suas tarefas.

O administrador configura a frequência com que as atualizações são enviadas, a hora em que são enviadas e quem as recebe.

Você também pode executar o coordenador de projetos sob demanda, mencionando-o em uma atualização do projeto. O Coordenador de projetos é executado quando mencionado, mesmo que não esteja agendado para execução nesse momento.

>[!NOTE]
>
>O comportamento do coordenador de projetos pode mudar antes da disponibilidade geral.

## Adicionar o coordenador de projetos a um projeto

Um administrador deve primeiro criar o Coordenador de projetos e adicionar o campo **Coordenador de projetos** ao cabeçalho do projeto no seu modelo de layout. Em seguida, o campo aparece no cabeçalho do projeto.

Para obter mais informações, consulte [Personalizar cabeçalhos de objetos usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

Para atribuir um Coordenador de projetos a um projeto:

1. Vá para o projeto ao qual deseja atribuir um Coordenador de projeto.
1. No cabeçalho do projeto, clique no campo **Coordenador de projetos**.
1. Selecione o Coordenador de projetos que deseja atribuir.

   A janela exibe uma descrição do Coordenador de projetos selecionado, bem como as ações que o Coordenador de projetos realiza.
1. Clique em **Aplicar**.

## Executar o coordenador de projetos mencionando-o

Além das atualizações agendadas, você pode acionar o Coordenador de projetos a qualquer momento, @mentioning-o em uma atualização do projeto. O coordenador de projetos é executado assim que é mencionado, mesmo que não esteja agendado para execução nesse momento.

Para mencionar o coordenador de projetos:

1. Vá para o projeto que tem o coordenador de projeto atribuído.
1. Abra a área **Atualizações** do projeto.
1. No campo de atualização, digite **@** e selecione o Coordenador de projetos.
1. Adicione a mensagem e publique a atualização.

   O coordenador de projetos executa e publica sua resposta.

>[!NOTE]
>
>O Coordenador de projetos deve ser atribuído ao projeto antes que você possa acioná-lo com um @mention.

## Configurar o coordenador de projetos

Para obter instruções sobre como configurar o Coordenador de projetos, consulte [Configurar o Coordenador de projetos](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-project-coordinator) no artigo Configurar colaboradores de IA.
