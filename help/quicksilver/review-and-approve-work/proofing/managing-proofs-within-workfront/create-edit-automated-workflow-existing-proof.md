---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Criar ou editar um fluxo de trabalho automatizado para uma prova existente
description: Os fluxos de trabalho automatizados facilitam o gerenciamento do processo de revisão se o seu processo for complexo ou se você enviar conteúdo regularmente para revisão para os mesmos grupos de pessoas. Ao criar uma prova com um Fluxo de trabalho automatizado, a prova é movida de estágio para estágio até aprovação final. Os participantes são notificados quando é sua vez de revisar o documento.
author: Courtney
feature: Digital Content and Documents
exl-id: 852f960f-1b57-4a8a-a928-407ad52418e6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1225'
ht-degree: 1%

---

# Criar ou editar um fluxo de trabalho automatizado para uma prova existente

Os fluxos de trabalho automatizados facilitam o gerenciamento do processo de revisão se o seu processo for complexo ou se você enviar conteúdo regularmente para revisão para os mesmos grupos de pessoas. Ao criar uma prova com um Fluxo de trabalho automatizado, a prova é movida de estágio para estágio até aprovação final. Os participantes são notificados quando é sua vez de revisar o documento.

Para obter informações sobre como criar um Fluxo de trabalho automatizado para uma nova prova, consulte [Criar uma prova avançada com um fluxo de trabalho Automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Plano atual: Pro ou superior</p> <p>ou</p> <p>Plano herdado: Premium</p> <p>Para obter mais informações sobre como revisar o acesso com os diferentes planos, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de prova no Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano atual: Trabalho ou Plano</p> <p>Plano herdado: Qualquer (É necessário ter a prova ativada para o usuário)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de Permissões de Prova </td> 
   <td>Gerente ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, função ou Perfil de permissão de prova você possui, entre em contato com o administrador da Workfront ou da Workfront Proof.

## Crie ou edite um Fluxo de trabalho automatizado para uma prova existente:

1. Passe o mouse sobre o documento na área Documents e clique em Proofing Workflow.

   Ou

   Se você estiver revisando a prova no visualizador de prova, clique em **Fluxo de trabalho** ![](assets/workflow-icon-proofing-viewer.png) no painel esquerdo, em seguida, clique no ícone Editar ![](assets/edit-icon-proofing-viewer.png) para abrir as configurações do Fluxo de trabalho automatizado da prova.

1. (Condicional) Se a prova estiver usando atualmente um fluxo de trabalho básico (sem estágios), clique em **Converter em fluxo de trabalho automatizado** na tela exibida.

   >[!NOTE]
   >
   >Você não pode editar o primeiro estágio ao converter de um fluxo de trabalho básico em um Fluxo de trabalho automatizado, mas pode adicionar e configurar novos estágios.

1. Condicional) Para usar um modelo de Fluxo de trabalho automatizado que o administrador do Adobe Workfront criou e compartilhou com você, clique em **Adicionar modelo**, selecione o modelo na caixa exibida e clique em **Adicionar modelo**.

   Para obter mais informações, consulte [Sobre o uso de modelos de Fluxo de trabalho automatizado](#about-using-automated-workflow-templates) neste artigo.

1. Adicione um estágio ao Fluxo de trabalho automatizado:

   1. Clique em **Nova etapa** próximo ao canto superior direito.
   1. Na caixa exibida, digite um **Nome** para o palco.
   1. (Opcional) Defina um prazo para o estágio.
   1. No **Ativar estágio** escolha como deseja ativar o estágio:


      <table>
      <tbody>
      <tr>
      <td><strong>Na criação da prova</strong></td>
      <td>O estágio fica ativo automaticamente porque a prova já foi criada.</td>
      </tr>
      <tr>
      <td><strong>Quando o prazo final do estágio anterior passar</strong></td>
      <td>Clique na etapa anterior no <strong>Fase principal</strong> lista suspensa .</td>
      </tr>
      <tr>
      <td><strong>Em uma data e hora específicas</strong></td>
      <td>Clique no botão <strong>Ligado</strong> para selecionar a data, clique na caixa à direita para selecionar a hora.</td>
      </tr>
      <tr>
      <td><strong>Todas as decisões são Aprovadas ou Aprovadas com alterações no estágio pai</strong></td>
      <td>Clique no estágio principal na <strong>Fase principal</strong> lista suspensa.</td>
      </tr>
      <tr>
      <td><strong>Todas as decisões são Aprovadas no estágio principal</strong></td>
      <td>Clique no estágio principal na <strong>Fase principal</strong> lista suspensa.</td>
      </tr>
      <tr>
      <td><strong>Todas as decisões são tomadas</strong></td>
      <td>Clique no estágio principal na <strong>Fase principal</strong> lista suspensa.</td>
      </tr>
      </tbody>
      </table>


   1. Insira um nome de contato ou endereço de email e defina as configurações para revisores para o estágio.

      Para obter informações sobre como adicionar revisores, consulte [Sobre como adicionar revisores a um estágio](#about-adding-reviewers-to-a-stage) neste artigo.

   1. Use qualquer uma das seguintes opções para configurar ainda mais o estágio:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader"><strong>Opções de prazo final</strong> </td>
         <td><p>Para definir um prazo para o estágio, clique em uma opção no <strong>Opções de prazo</strong> lista suspensa. Em seguida, em <strong>Prazo</strong>, execute um dos seguintes procedimentos:</p>
          <ul>
           <li>Se você escolher <strong>Definir data específica</strong>: Selecione a data e a hora do prazo desejadas.</li>
           <li>Se você escolher <strong>Calcular a partir da data de ativação do estágio</strong>: Selecione o número de dias úteis que deseja adicionar à data de ativação do estágio para determinar o prazo.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">Bloquear palco</td>
         <td>Especifique quando o palco pode ser bloqueado. </td>
        </tr>
        <tr>
         <td role="rowheader">Tomador de decisão primário</td>
         <td><p>Selecione o decisor Principal no palco (disponível somente depois de adicionar pelo menos uma pessoa ao palco que tenha uma função de Aprovador ou superior). Se você selecionar um decisor Principal, a variável <strong>Apenas uma decisão é necessária</strong> está desabilitada nesse estágio.</p></td>
        </tr>
        <tr>
         <td role="rowheader">É necessária somente uma decisão</td>
         <td>Termina todo o processo de revisão quando um dos decisores tomar uma decisão.<p>Essa opção não estará disponível se você tiver designado um usuário na <strong>Tomador de decisão principal</strong> menu suspenso.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Fase privada</td>
         <td>Permite que apenas as pessoas a seguir visualizem comentários e decisões tomadas nesta fase: Supervisores, administradores da Adobe Workfront e administradores da Workfront Proof</td>
        </tr>
        <tr>
         <td role="rowheader">Notificar pessoas por email</td>
         <td>Alerta os revisores com uma notificação por email quando for sua vez de trabalhar na prova.</td>
        </tr>
       </tbody>
      </table>

   1. Clique em **Adicionar estágio**.

1. Repita a etapa anterior conforme necessário para adicionar mais estágios.

   À medida que você adiciona estágios ao Fluxo de trabalho automatizado, um diagrama é exibido na tela para representá-los:

   ![](assets/workflow-diagram-existing-proof-qs-350x215.png)

1. Quando terminar de adicionar estágios, clique em **Concluído**.

## Sobre o uso de modelos de Fluxo de trabalho automatizado {#about-using-automated-workflow-templates}

Considere o seguinte ao usar um modelo de Fluxo de trabalho automatizado:

1. As configurações de um modelo de Fluxo de trabalho automatizado determinam o que você pode fazer com o Fluxo de trabalho automatizado para uma prova. Por exemplo, se o botão Add a stage estiver desativado no template, ele não estará visível à medida que você trabalha com as configurações do Automated Workflow para a prova.
1. Quando uma pessoa é adicionada a uma página em um modelo de Fluxo de trabalho automatizado, mas também já está presente como um revisor na prova, a aplicação do modelo remove o revisor do estágio. Se você não adicionar outro revisor ao palco, uma mensagem solicitará que você adicione um.
1. A capacidade de modificar um modelo de Fluxo de trabalho automatizado depende das configurações do modelo definidas pelo administrador do Workfront, conforme descrito em . Se a capacidade de modificar o modelo estiver desativada, somente o proprietário do modelo poderá modificá-lo.

## Sobre como adicionar revisores a um estágio {#about-adding-reviewers-to-a-stage}

Considere o seguinte ao adicionar revisores a um estágio:

* Depois de adicionar um usuário a um palco, você pode definir as configurações para esse usuário na prova, como a função de prova e quaisquer permissões adicionais que ele deve ter e o tipo de alertas de email que eles receberão quando as pessoas fizerem comentários e decisões na prova.
* Você pode arrastar um ou mais usuários de um estágio para outro. Você pode arrastar usuários diretamente para outro palco, ou pode arrastar usuários para um palco no palco **Estágios** diagrama. Para selecionar vários usuários, pressione Shift+Ctrl (no Windows) ou Shift+Command (no Mac).
* É possível adicionar um revisor a uma prova apenas uma vez, o que significa que não é possível adicionar a mesma pessoa a mais de um estágio na prova.
* Os revisores que não são adicionados a uma fase privada não podem ver essa fase na prova ou nos comentários feitos nessa fase.
* Por padrão, adicionar um usuário a um palco concede a esse usuário acesso para visualizar a prova a partir do momento em que a prova é criada.

   O administrador do Workfront pode impedir que os usuários acessem a prova até que o workflow entre no estágio em que o usuário foi adicionado. Para obter mais informações, consulte em .
