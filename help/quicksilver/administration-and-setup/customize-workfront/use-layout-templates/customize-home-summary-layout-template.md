---
title: Personalizar Início e Resumo Usando um Modelo de Layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Você pode usar um Modelo de layout para configurar o que os usuários veem quando clicam em uma tarefa ou problema na Página inicial e no Resumo. Cada configuração feita usando as etapas abaixo afeta a área Página inicial e o Painel de resumo da mesma maneira. Essas personalizações não se aplicam ao painel Resumo do documento.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: 115757a829b92c13cb684369120e26602b9a1782
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 2%

---

# Personalizar Início e Resumo usando um modelo de layout

<span class="preview">Este artigo será renomeado para &quot;Personalizar o painel de resumo usando um modelo de layout&quot; quando a Página Inicial Herdada for removida do Workfront com a versão do quarto trimestre em 17 de outubro. 2024.</span>

Você pode usar um Modelo de layout para configurar o que os usuários veem quando clicam em uma tarefa ou problema na Página inicial e no Resumo. Cada configuração feita usando as etapas abaixo afeta a área Página inicial e o Painel de resumo da mesma maneira. Essas personalizações não se aplicam ao painel Resumo do documento.

Você pode configurar:

* Quais campos são exibidos para uma tarefa ou problema na área Detalhes e em que ordem
* Se atualizações, tempo registrado, documentos anexados e carimbos de data e hora são exibidos para uma tarefa ou problema selecionado

Você também pode personalizar os campos que os usuários veem na área Página inicial quando eles clicam em uma aprovação de projeto, aprovação de documento ou aprovação de versão de documento atribuída a eles.

Para obter informações sobre a área Página Inicial, consulte [Usar a área Página Inicial](../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md). Para obter informações sobre o painel Resumo, consulte [Visão geral do resumo](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

Para obter informações sobre como criar modelos de layout, consulte [Criar e gerenciar modelos de layout](../use-layout-templates/create-and-manage-layout-templates.md).

Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Após configurar um modelo de layout, você deve atribuí-lo aos usuários para que as alterações feitas fiquem visíveis para outros usuários. Para obter informações sobre como atribuir um modelo de layout aos usuários, consulte [Atribuir usuários a um modelo de layout](../use-layout-templates/assign-users-to-layout-template.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td><p>Novo: Padrão</p>
  <p> Atual: Plano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Para executar essas etapas no nível do sistema, você precisa do nível de acesso Administrador do sistema.
Para executá-las para um grupo, você deve ser um gerente desse grupo.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizar Início e Resumo usando um modelo de layout

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Clique na seta para baixo ![](assets/dropdown-arrow.png) em **Personalize o que os usuários veem** e clique em **Página Inicial e Resumo**.

1. Na lista à esquerda, clique no tipo de objeto (**Tarefas**, **Problemas**, **Projetos**, **Documentos** ou **Versões de Documentos**) que você deseja personalizar na Página Inicial e no Resumo.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tarefas</td> 
      <td> <p>Na Página inicial, a configuração dessa configuração afeta a área à direita de uma tarefa quando um usuário clica na tarefa. E, em uma lista de tarefas, isso afeta o painel Resumo que é exibido no lado direito da página quando um usuário seleciona uma tarefa e clica no ícone Abrir Resumo <img src="assets/summary-panel-icon.png">.</p> <p>Por exemplo, você pode determinar quais campos os usuários veem na área Detalhes quando os usuários selecionam tarefas na Página inicial:</p> <p><img src="assets/home-details-adobe branding.jpg"></p> <p>E quando selecionam uma tarefa no Resumo:</p> <p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Problemas</td> 
      <td> <p>Na Página inicial, a configuração dessa configuração afeta a área à direita de um problema quando um usuário clica nele.</p> <p>Em uma lista de problemas, essa configuração afeta o painel Resumo que é exibido no lado direito da página quando um usuário seleciona um problema e clica no ícone Abrir Resumo <img src="assets/summary-panel-icon.png">.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Projetos</td> 
      <td>Na Página inicial, quando um usuário clica em uma aprovação de projeto atribuída a ele, sua configuração para essa configuração afeta a área à direita da aprovação.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td>Na Página inicial, quando um usuário clica em uma aprovação de documento atribuída a ele, sua configuração para essa configuração afeta a área à direita da aprovação.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Versões do documento</td> 
      <td>Na Página inicial, quando um usuário clica em uma aprovação atribuída a ele para uma versão específica de um documento, sua configuração para essa configuração afeta a área à direita da aprovação.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >Se uma tarefa não estiver atribuída, o usuário atribuído ao modelo de layout não verá as personalizações de campo no Resumo.

1. (Condicional) Se você clicou em Tarefas ou Problemas na etapa anterior, selecione a categoria da tarefa ou problema que deseja personalizar.

   ![](assets/choose-cat-cstmz-nwe-adobe-branding.png)

1. (Condicional) Se o menu suspenso **Definir botão de ação principal** for exibido (se você selecionar **Tarefas** ou **Problemas** na lista à esquerda), clique na ação principal (**Concluído** ou **Status**) que você deseja disponibilizar para os usuários na área Página inicial e no painel Resumo quando eles visualizarem uma tarefa ou um problema.

   ![](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)

1. Adicionar ![](assets/add-item-plus-in-circle-blue.png) ou ocultar ![](assets/close-or-hide---x.png) campos para o tipo de objeto selecionado.

   ![](assets/lt-home-add-hide-fields-adobe-branding.png)

1. Repita as etapas 3 a 6 para personalizar a área Início e o painel Resumo para qualquer outro tipo de objeto.
1. Clique em **Configurações globais**, próximo ao canto inferior esquerdo, e habilite ou desabilite qualquer uma das seguintes opções relacionadas a objetos do Adobe Workfront na Página Inicial e em Resumo:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Exibir atualizações do trabalho</td> 
      <td>Exibe todas as atualizações feitas em uma tarefa ou problema selecionado na Página inicial ou em Resumo. Isso inclui atualizações do sistema e atualizações feitas por um usuário. Os usuários ainda podem filtrar atualizações do sistema, conforme descrito em <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref">Habilitar ou desabilitar atualizações do sistema</a> em <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Trabalho de atualização</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Registar horas em relação a trabalho</td> 
      <td>Exibe a opção Registrar tempo no trabalho quando uma tarefa ou problema é selecionado, permitindo que os usuários registrem tempo nos itens de trabalho diretamente das áreas Início e Resumo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exibir documentos associados ao trabalho</td> 
      <td>Exibe uma área Documentos na Página inicial e em Resumo quando uma tarefa ou problema é selecionado, listando todos os documentos anexados à tarefa ou problema. Os usuários podem clicar em documentos para exibi-los em uma janela de pré-visualização.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ocultar carimbo de data e hora</td> 
      <td>Oculta carimbos de data e hora para os seguintes campos de data na Página inicial e no Resumo:
       <ul>
        <li>Data de conclusão planejada</li>
        <li>Data de confirmação</li>
        <li>Data de Envio</li>
       </ul><p><b>NOTA</b>:</p> <p> Quando esta opção está habilitada, os itens de trabalho vencidos são movidos para o agrupamento Atrasado na Lista de trabalho da página inicial com base somente na data, não na hora.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Continue personalizando o modelo de layout.

   Ou

   Se tiver terminado de personalizar, clique em **Salvar**.

Para obter mais informações sobre modelos de layout, consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
