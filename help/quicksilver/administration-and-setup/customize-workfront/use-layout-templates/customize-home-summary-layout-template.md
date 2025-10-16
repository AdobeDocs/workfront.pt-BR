---
title: Personalizar o painel de resumo usando um modelo de layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Você pode usar um Modelo de layout para configurar o que os usuários veem quando clicam em uma tarefa ou problema no Resumo. Cada configuração feita usando as etapas abaixo afeta o painel Resumo. Essas personalizações não se aplicam ao painel Resumo do documento.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: 76e32fa6b87583d2b8c296045da731afdb6d1f9a
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 2%

---

# Personalizar o painel Resumo usando um modelo de layout

<!--Audited: 11/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>   -->


Você pode usar um Modelo de layout para configurar o que os usuários veem no painel Resumo quando clicam em uma tarefa ou problema. Cada configuração feita usando as etapas abaixo afeta o painel Resumo. Essas personalizações não se aplicam ao painel Resumo do documento.

Você pode configurar:

* Quais campos são exibidos para uma tarefa ou problema na área Detalhes e em que ordem
* Se atualizações, tempo registrado, documentos anexados e carimbos de data e hora são exibidos para uma tarefa ou problema selecionado

Você também pode personalizar os campos que os usuários veem na área Página inicial quando eles clicam em uma aprovação de projeto, aprovação de documento ou aprovação de versão de documento atribuída a eles.

Para obter informações sobre o painel Resumo, consulte [Visão geral do resumo](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

Para obter informações sobre como criar modelos de layout, consulte [Criar e gerenciar modelos de layout](../use-layout-templates/create-and-manage-layout-templates.md).

Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Após configurar um modelo de layout, você deve atribuí-lo aos usuários para que as alterações feitas fiquem visíveis para outros usuários. Para obter informações sobre como atribuir um modelo de layout aos usuários, consulte [Atribuir usuários a um modelo de layout](../use-layout-templates/assign-users-to-layout-template.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Para executar essas etapas no nível do sistema, você precisa do nível de acesso Administrador do sistema.</p>
        <p>Para executá-las para um grupo, você deve ser um gerente desse grupo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizar o painel Resumo usando um modelo de layout

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Clique na seta para baixo ![Seta para baixo](assets/dropdown-arrow.png) em **Personalize o que os usuários veem** e clique em **Painel de resumo**.

1. Na lista exibida abaixo, clique no tipo de objeto para o qual você deseja personalizar o Painel de resumo.

   A tabela abaixo explica o que pode ser personalizado para cada objeto

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tarefas</td> 
      <td> <p>Em uma lista de tarefas, essa configuração afeta o painel Resumo exibido no lado direito da página quando um usuário seleciona uma tarefa e clica no ícone Abrir Resumo <img src="assets/summary-panel-icon.png">.</p>

   <p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Problemas</td> 
      <td><p>Em uma lista de problemas, essa configuração afeta o painel Resumo que é exibido no lado direito da página quando um usuário seleciona um problema e clica no ícone Abrir Resumo <img src="assets/summary-panel-icon.png">.</p> </td> 
     </tr> 
    </tbody> 
   </table>

<!--These were removed with the new Home: 

<tr> 
      <td role="rowheader">Projects</td> 
      <td><ul><li><p>In Home, when a user clicks a project approval assigned to them, your configuration for this setting affects the area to the right of the approval.</p>
      <p><b>IMPORTANT:</b> </p><p>This is a deprecated feature. Any changes you make to this area are related to a feature that Workfront has removed. This option will be removed from Workfront with a later maintenance update.</p></li>
      </ul> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documents</td> 
      <td>
     <ul><li><p>In Home, when a user clicks a document approval assigned to them, your configuration for this setting affects the area to the right of the approval.</p>
      <p><b>IMPORTANT:</b> </p><p> This is a deprecated feature. Any changes you make to this area are related to a feature that Workfront has removed. This option will be removed from Workfront with a later maintenance update.</p></li>
      </ul>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Document Versions</td> 
      <td><ul><li><p>In Home, when a user clicks an approval assigned to them for a particular version of a document, your configuration for this setting affects the area to the right of the approval.</p>
      <p><p><b>IMPORTANT:</b></p> This is a deprecated feature. Any changes you make to this area are related to a feature that Workfront has removed. This option will be removed from Workfront with a later maintenance update.</p></li>
      </ul>
      </td> 
     </tr> -->


>[!IMPORTANT]
>
>Se uma tarefa não estiver atribuída, o usuário atribuído ao modelo de layout não verá as personalizações de campo no Resumo.

1. (Condicional) Se você clicou em Tarefas ou Problemas na etapa anterior, selecione a categoria da tarefa ou problema que deseja personalizar.

   ![Escolher categoria para personalizar](assets/choose-cat-cstmz-nwe-adobe-branding.png)

1. (Condicional) Se o menu suspenso **Definir botão de ação principal** for exibido (se você selecionar **Tarefas** ou **Problemas** na lista à esquerda), clique na ação principal (**Concluído** ou **Status**) que você deseja disponibilizar para os usuários no Painel de resumo quando eles visualizarem uma tarefa ou um problema.

   ![Definir ação principal](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)

1. Adicionar ![Adicionar item](assets/add-item-plus-in-circle-blue.png) ou ocultar campos ![Ocultar item](assets/close-or-hide---x.png) para o tipo de objeto selecionado.

   ![Adicionar e ocultar campos](assets/lt-home-add-hide-fields-adobe-branding.png)

1. Repita as etapas 3 a 6 para personalizar o painel Resumo para qualquer outro tipo de objeto.
1. Clique em **Configurações globais**, próximo ao canto inferior esquerdo, e habilite ou desabilite qualquer uma das seguintes opções relacionadas a objetos do Adobe Workfront no Resumo:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Exibir atualizações do trabalho</td> 
      <td>Exibe todas as atualizações feitas em uma tarefa ou problema selecionado no painel Resumo. Isso inclui atualizações do sistema e atualizações feitas por um usuário. Os usuários ainda podem filtrar atualizações do sistema, conforme descrito em <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref">Habilitar ou desabilitar atualizações do sistema</a> em <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Trabalho de atualização</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Registar horas em relação a trabalho</td> 
      <td>Exibe a opção Registrar tempo no trabalho quando uma tarefa ou problema é selecionado, permitindo que os usuários registrem tempo nos itens de trabalho diretamente das áreas Início e Resumo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exibir documentos associados ao trabalho</td> 
      <td>Exibe uma área Documentos no painel Resumo quando uma tarefa ou problema é selecionado, listando todos os documentos anexados à tarefa ou problema. Os usuários podem clicar em documentos para exibi-los em uma janela de pré-visualização.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ocultar carimbo de data e hora</td> 
      <td>Oculta carimbos de data e hora para os seguintes campos de data no painel Resumo:
       <ul>
        <li>Data de conclusão planejada</li>
        <li>Data de confirmação</li>
        <li>Data de Envio</li>
       </ul></td> 
     </tr> 
    </tbody> 
   </table>

1. Continue personalizando o modelo de layout.

   Ou

   Se tiver terminado de personalizar, clique em **Salvar**.

Para obter mais informações sobre modelos de layout, consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
