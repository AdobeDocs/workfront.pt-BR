---
title: Personalizar página inicial e resumo usando um modelo de layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Você pode usar um Modelo de layout para configurar o que os usuários veem ao clicar em uma tarefa ou problema na Página inicial e no Resumo. Cada configuração feita usando as etapas abaixo afeta a área inicial e o painel Resumo da mesma maneira. Essas personalizações não se aplicam ao painel Resumo do documento.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 2%

---

# Personalizar página inicial e resumo usando um modelo de layout

Você pode usar um Modelo de layout para configurar o que os usuários veem ao clicar em uma tarefa ou problema na Página inicial e no Resumo. Cada configuração feita usando as etapas abaixo afeta a área inicial e o painel Resumo da mesma maneira. Essas personalizações não se aplicam ao painel Resumo do documento.

Você pode configurar:

* Quais campos são exibidos para uma tarefa ou problema na área Detalhes e em que ordem
* Se atualizações, tempo registrado, documentos anexados e carimbos de data e hora são exibidos para uma tarefa ou problema selecionado

Também é possível personalizar os campos que os usuários veem na área inicial quando clicam em aprovação de projeto, aprovação de documento ou aprovação de versão de documento atribuída a eles.

Para obter informações sobre a área inicial, consulte [Usar a área Início](../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md). Para obter informações sobre o painel Resumo, consulte [Visão geral do resumo](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Para executar essas etapas no nível do sistema, é necessário o nível de acesso Administrador do sistema.
Para executá-los para um grupo, você deve ser um gerente desse grupo.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizar página inicial e resumo usando um modelo de layout

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Clique na seta para baixo ![](assets/dropdown-arrow.png) under **Personalize o que os usuários veem**, depois clique em **Início e resumo**.

1. Na lista exibida à esquerda, clique no tipo de objeto (**Tarefas**, **Problemas**, **Projetos**, **Documentos** ou **Versões do documento**) que você deseja personalizar em Início e Resumo.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tarefas</td> 
      <td> <p>Na página inicial, a configuração dessa configuração afeta a área à direita de uma tarefa quando um usuário clica na tarefa. E, em uma lista de tarefas, afeta o painel Resumo que é exibido no lado direito da página quando um usuário seleciona uma tarefa e clica no ícone Abrir resumo <img src="assets/summary-panel-icon.png">.</p> <p>Por exemplo, você pode determinar quais campos os usuários veem na área Detalhes quando os usuários selecionam tarefas na Página inicial:</p> <p><img src="assets/home-details-adobe branding.jpg"></p> <p>E quando selecionam uma tarefa no Resumo:</p> <p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Problemas</td> 
      <td> <p>Na Página inicial, a configuração dessa configuração afeta a área à direita de um problema quando um usuário clica no problema.</p> <p>Em uma lista de problemas, essa configuração afeta o painel Resumo , que é exibido no lado direito da página quando um usuário seleciona um problema e clica no ícone Abrir resumo <img src="assets/summary-panel-icon.png">.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Projetos</td> 
      <td>Na Página inicial, quando um usuário clica em uma aprovação de projeto atribuída a ele, a configuração dessa configuração afeta a área à direita da aprovação.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td>Na Página inicial, quando um usuário clica em uma aprovação de documento atribuída a ele, a configuração dessa configuração afeta a área à direita da aprovação.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Versões do documento</td> 
      <td>Na Página inicial, quando um usuário clica em uma aprovação atribuída a ele para uma versão específica de um documento, sua configuração para essa configuração afeta a área à direita da aprovação.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >Se uma tarefa não for atribuída, o usuário atribuído ao modelo de layout não visualizará as personalizações de campo no Resumo.

1. (Condicional) Se você clicou em Tarefas ou Problemas na etapa anterior, selecione a categoria de tarefa ou problema que deseja personalizar.

   ![](assets/choose-cat-cstmz-nwe-adobe-branding.png)

1. (Condicional) Se a variável **Botão Definir ação primária** será exibido o menu suspenso (se você selecionar **Tarefas** ou **Problemas** na lista à esquerda), clique na ação principal (**Concluído** ou **Status**) que você deseja disponibilizar para os usuários na área inicial e no painel Resumo quando eles visualizarem uma tarefa ou um problema.

   ![](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)

1. Adicionar ![](assets/add-item-plus-in-circle-blue.png) ou ocultar ![](assets/close-or-hide---x.png) campos para o tipo de objeto selecionado.

   ![](assets/lt-home-add-hide-fields-adobe-branding.png)

1. Repita as etapas 3 a 6 para personalizar a área inicial e o painel Resumo para qualquer outro tipo de objeto.
1. Clique em **Configurações globais**, próximo ao canto inferior esquerdo, ative ou desative qualquer uma das seguintes opções relacionadas a objetos do Adobe Workfront em Início e Resumo:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Exibir atualizações do trabalho</td> 
      <td>Exibe as atualizações feitas em uma tarefa ou problema selecionado em Início ou Resumo. Isso inclui atualizações do sistema e atualizações feitas por um usuário. Os usuários ainda podem filtrar as atualizações do sistema, conforme descrito em <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref">Ativar ou desativar atualizações do sistema</a> em <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Atualizar trabalho</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Registar horas em relação a trabalho</td> 
      <td>Exibe a opção Log time against work quando uma tarefa ou problema é selecionado, permitindo que os usuários façam logon nos itens de trabalho diretamente das áreas Home e Summary .</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exibir documentos associados ao trabalho</td> 
      <td>Exibe uma área Documentos em Início e Resumo quando uma tarefa ou problema é selecionado, listando quaisquer documentos anexados à tarefa ou problema. Os usuários podem clicar em documentos para exibi-los em uma janela de pré-visualização.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ocultar carimbo de data e hora</td> 
      <td>Oculta os carimbos de data e hora dos seguintes campos de data em Início e Resumo:
       <ul>
        <li>Data de conclusão planejada</li>
        <li>Data de confirmação</li>
        <li><p>Data de envio</p></li>
       </ul><p><b>OBSERVAÇÃO</b>: Quando esta opção está ativada, os itens de trabalho que se tornam vencidos são movidos para o Agrupamento tardio na Lista de Trabalho Inicial com base apenas em data, não em hora.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Continue personalizando o modelo de layout.

   Ou

   Se tiver terminado de personalizar, clique em **Salvar**.

Para obter mais informações sobre modelos de layout, consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
