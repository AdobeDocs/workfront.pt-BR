---
title: Introdução ao Adobe Workfront Planning Designer
description: Usando o Adobe Planning Designer, você pode gerar um novo espaço de trabalho, completo com tipos de registro e campos no Workfront Planning, adicionar objetos a um espaço de trabalho ou exibir o histórico de alterações em registros.
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 866b237db5d109b0a435145119a6412e41d960ab
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 1%

---


<!--add these at release to the metadata:

author: Alina, Becky
feature: Workfront Planning
role: User, Admin -->

# Introdução ao Adobe Workfront Planning Designer

{{planning-important-intro}}

Você pode usar o Adobe Planning Designer viabilizado pela IA para gerar um novo espaço de trabalho, adicionar objetos a um espaço de trabalho (tipos de registro, registros, exibições ou campos) ou exibir o histórico de alterações nos registros.

>[!IMPORTANT]
>
>No momento, o Planning Designer está disponível apenas para usuários que participam do programa Closed Beta.

Para obter informações sobre o Workfront Planning, consulte os seguintes artigos:

* [Informações gerais sobre o Adobe Workfront Planning](/help/quicksilver/planning/planning-information.md)
* [Introdução ao Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)
* [Visão geral do acesso ao Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md)


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacotes Adobe Workfront</p></td> 
   <td> 
<p>Qualquer pacote do Workfront e do Planning</p>
<p>Qualquer pacote de Fluxo de Trabalho e Planejamento</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Padrão</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Inscrevendo-se no programa Beta Fechado para o Designer de Planejamento

<!--edit this Or create a new article under Beta programs?? -->

Atualmente, você pode solicitar a participação no programa Beta Fechado para o Designer de Planejamento.

## Considerações sobre o Planning Designer

* Para usar o Designer do Planning, sua organização deve atender aos requisitos para usar o Assistente de IA da Workfront.

  Para obter detalhes, consulte [Pré-requisitos do Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

* Para usar o Planning Designer, um administrador do sistema deve habilitá-lo na área Preferências do Sistema da sua Configuração.

* Você pode usar prompts para criar objetos do Planning usando o Assistente do Workfront AI na área do Planning ou usando o Planning Designer.

* As ações executadas pelo Assistente de IA na área de Planejamento ou aquelas executadas pelo Planning Designer estão no contexto das suas permissões do Workfront Planning e do seu nível de acesso ao Workfront.

  Para obter informações, consulte os seguintes artigos:

   * [Visão geral das permissões de compartilhamento no Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Visão geral do tipo de licença ao usar o Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* As alterações feitas pelo Planning Designer em nome do usuário são rastreadas no painel de histórico do registro.

* Você pode usar comandos para desfazer suas ações. Por exemplo, você pode digitar &quot;Desfazer a última alteração&quot; para reverter a alteração.

* Ao criar, atualizar ou excluir um objeto por meio do Planning Designer, ele exibe as ações desejadas e solicita uma confirmação. Você pode confirmar ou cancelar as ações.

* Quando você cria espaços de trabalho e tipos de registro usando o Planning Designer, as exibições e os campos também são criados automaticamente.

## Funcionalidade atualmente disponível para o Planning Designer

Você pode usar o Planning Designer ou o Assistente de IA para executar qualquer uma das seguintes ações:

* Criar e configurar espaços de trabalho

* Criar tipos de registro

* Criar campos ou campos de fórmula

* Criar, excluir, duplicar e restaurar registros

* Editar, atualizar, anexar um campo em um registro

* Vincular registros a outros registros

* Acessar histórico de alterações de registro

* Criar exibições personalizadas

* Criar registros importando um documento.

  A criação de registros a partir de um documento importado está disponível somente no Planning Designer, e não no AI Assistant.

  Para obter informações sobre os tipos e tamanhos de arquivo aceitos, consulte a seção &quot;Medidas de proteção de documentos&quot; no artigo [Usar Preenchimento de Formulário fornecido pela IA para preencher uma solicitação usando prompts ou documentos](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).

  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Ativar o Designer de planejamento para sua organização

Como administrador do Workfront, você deve primeiro habilitar o Planning Designer para sua organização.

<!--add steps here-->

1. Faça logon no Workfront como Administrador do sistema.
1. Clique em **Menu principal** ![Ícone do menu principal](assets/main-menu-shell.png) no canto superior esquerdo da tela e em **Instalação**.
1. Clique em **Sistema** > no painel esquerdo e vá para a área **Preferências de IA**.
1. Ative as seguintes configurações:
   * **Habilitar IA**
   * **Aceitar Betas de IA**
   * **Designer do Planning**

   ![Configuração do Planning Designer nas Preferências do Sistema](assets/planning-designer-toggle-in-system-preferences.png)
1. Clique em **Salvar**.

   Todos os usuários do sistema que possuem uma licença Standard agora podem ver o botão **Design com IA** na página principal Espaços de trabalho na área do Planning. <!--check screen shot-->

   ![Botão Criar com IA na página Espaços de Trabalho](assets/design-with-ai-button-on-workspaces-page.png)

   Todos os usuários agora podem iniciar e usar o Planning Designer para criar e atualizar objetos do Workfront Planning.

## Criar ou atualizar objetos usando o Planning Designer

Você pode criar ou atualizar objetos no Workfront Planning usando o Planning Designer ou o Assistente de IA, a menos que especificado de outra forma.

1. Faça logon no Workfront e clique no ícone **Menu principal** ![Menu principal Linhas](assets/lines-main-menu.png), no canto superior esquerdo.

1. Clique em **Planning**. A área Planejamento é aberta.

1. Clique em **Design com IA**.

   A janela **Planning Designer** é aberta.

   ![Janela do Planning Designer](assets/planning-designer-window.png)

1. No espaço fornecido, comece a digitar comandos para o Assistente de IA e, em seguida, clique em Inserir quando terminar.

   <!--add screen shot-->

   Por exemplo, você pode digitar uma solicitação semelhante às seguintes:

   * Crie e configure um espaço de trabalho com cinco tipos de registro para gerenciar campanhas

   * Criar campanhas de marketing para cada mês do ano atual

   * Adicionar um campo de campanha para o Status do espaço de trabalho de Design de marketing

   * Excluir todos os registros em um Status de Obsoleto

   * Atualizar todas as campanhas do Planning para um status Ativo

   * Conectar campanhas a personalidades no espaço de trabalho de Design de marketing

   * Exibir o histórico de alterações para a campanha &quot;Dia dos namorados&quot;

   * Crie uma exibição de linha do tempo para campanhas no espaço de trabalho de Design de marketing

   * Criar registros importando um documento. A criação de registros a partir de um documento importado está disponível somente no Planning Designer, e não no AI Assistant.

   <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

1. Depois de receber uma resposta bem-sucedida, siga os links fornecidos na área de prompt para criar, atualizar ou revisar o objeto de sua solicitação.

   Quando você concorda em criar os objetos, as alterações são exibidas à direita da área de prompt.

   Você pode revisar espaços de trabalho, tipos de registro, campos, exibições e registros na área de visualização à direita do prompt.
1. (Opcional) Digite prompts adicionais para editar ainda mais seus objetos.
1. (Opcional) Clique no **ícone Alternar a tela de visualização do espaço de trabalho do AI** ![Ícone Ocultar ou mostrar tela de visualização](assets/hide-show-preview-screen-in-planning-designer.png) para abrir ou fechar a tela de visualização à direita.
1. Clique no **ícone Abrir espaço de trabalho em nova guia** ![ícone Abrir espaço de trabalho em nova guia](assets/open-workspace-on-new-tab-icon.png) para abrir o espaço de trabalho que você está atualizando em uma nova guia.
1. Clique no ícone **Fechar** **X** para fechar o Planning Designer e abrir a área Espaços de Trabalho.
1. Abra o espaço de trabalho editado usando o Planning Designer e faça mais alterações em seus objetos.




