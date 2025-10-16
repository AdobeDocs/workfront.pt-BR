---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Criar ou editar um Fluxo de trabalho automatizado para uma prova existente
description: Os fluxos de trabalho automatizados facilitam o gerenciamento do processo de revisão se ele for complexo ou se você enviar conteúdo regularmente para revisão para os mesmos grupos de pessoas. Ao criar uma prova com um fluxo de trabalho automatizado, a prova é movida de estágio para estágio até a aprovação final. Os participantes são notificados quando é a vez de revisar o documento.
author: Courtney
feature: Digital Content and Documents
exl-id: 852f960f-1b57-4a8a-a928-407ad52418e6
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '1142'
ht-degree: 1%

---

# Criar ou editar um Fluxo de trabalho automatizado para uma prova existente

Os fluxos de trabalho automatizados facilitam o gerenciamento do processo de revisão se ele for complexo ou se você enviar conteúdo regularmente para revisão para os mesmos grupos de pessoas. Ao criar uma prova com um fluxo de trabalho automatizado, a prova é movida de estágio para estágio até a aprovação final. Os participantes são notificados quando é a vez de revisar o documento.

Para obter informações sobre como criar um fluxo de trabalho automatizado para uma nova prova, consulte [Criar uma prova avançada com um fluxo de trabalho automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Trabalho ou Plano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de Permissões de Prova </td> 
   <td>Gerente ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a documentos</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar ou editar um Fluxo de trabalho automatizado para uma prova existente:

1. Passe o mouse sobre o documento na área Documentos, depois clique em Fluxo de trabalho de revisão.

   Ou

   Se você estiver revisando a prova no visualizador de provas, clique em **Fluxo de trabalho** ![ícone Fluxo de trabalho](assets/workflow-icon-proofing-viewer.png) no painel esquerdo e, em seguida, clique no ícone Editar ![ícone Editar](assets/edit-icon-proofing-viewer.png) para abrir as configurações de Fluxo de Trabalho Automatizado para a prova.

1. (Condicional) Se a prova estiver usando atualmente um fluxo de trabalho básico (sem estágios), clique em **Converter para Fluxo de Trabalho Automatizado** na tela exibida.

   >[!NOTE]
   >
   >Não é possível editar o primeiro estágio ao converter um fluxo de trabalho básico em um Fluxo de trabalho automatizado, mas você pode adicionar e configurar novos estágios.

1. Condicional) Para usar um modelo de Fluxo de Trabalho Automatizado que o administrador do Adobe Workfront criou e compartilhou com você, clique em **Adicionar modelo**, selecione o modelo na caixa exibida e clique em **Adicionar modelo**.

   Para obter mais informações, consulte [Sobre o uso de modelos de Fluxo de Trabalho Automatizado](#about-using-automated-workflow-templates) neste artigo.

1. Adicione um estágio ao Fluxo de trabalho automatizado:

   1. Clique em **Nova etapa** próximo ao canto superior direito.
   1. Na caixa exibida, digite um **Nome** para o estágio.
   1. (Opcional) Defina um prazo para o estágio.
   1. Na seção **Ativar estágio**, escolha como deseja ativar o estágio:


      <table>
      <tbody>
      <tr>
      <td><strong>Na criação da prova</strong></td>
      <td>O estágio se torna ativo automaticamente porque a prova já foi criada.</td>
      </tr>
      <tr>
      <td><strong>Quando o prazo final do estágio anterior passar</strong></td>
      <td>Clique no estágio anterior na lista suspensa <strong>Estágio pai</strong>.</td>
      </tr>
      <tr>
      <td><strong>Em uma data e hora específicas</strong></td>
      <td>Clique na caixa <strong>Em</strong> para selecionar a data e, em seguida, clique na caixa à direita para selecionar a hora.</td>
      </tr>
      <tr>
      <td><strong>Todas as decisões são Aprovadas ou Aprovadas com alterações no estágio principal</strong></td>
      <td>Clique no estágio pai na lista suspensa <strong>Estágio pai</strong>.</td>
      </tr>
      <tr>
      <td><strong>Todas as decisões são Aprovadas no estágio principal</strong></td>
      <td>Clique no estágio pai na lista suspensa <strong>Estágio pai</strong>.</td>
      </tr>
      <tr>
      <td><strong>Todas as decisões são tomadas</strong></td>
      <td>Clique no estágio pai na lista suspensa <strong>Estágio pai</strong>.</td>
      </tr>
      </tbody>
      </table>


   1. Insira um nome de contato ou endereço de email e defina as configurações dos revisores para o estágio.

      Para obter informações sobre como adicionar revisores, consulte [Sobre como adicionar revisores a um estágio](#about-adding-reviewers-to-a-stage) neste artigo.

   1. Use qualquer uma das seguintes opções para configurar ainda mais o estágio:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader"><strong>Opções de prazo final</strong> </td>
         <td><p>Para definir um prazo para o estágio, clique em uma opção na lista suspensa <strong>Opções de prazo</strong>. Em seguida, em <strong>Prazo</strong>, siga um destes procedimentos:</p>
          <ul>
           <li>Se você escolheu <strong>Definir data específica</strong>: selecione a data e a hora do prazo final desejadas.</li>
           <li>Se você escolheu <strong>Calcular a partir da data de ativação do estágio</strong>: selecione o número de dias úteis que deseja adicionar à data de ativação do estágio para determinar o prazo.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">Bloquear estágio</td>
         <td>Especifique quando o estágio pode ser bloqueado. </td>
        </tr>
        <tr>
         <td role="rowheader">Tomador de decisão primário</td>
         <td><p>Selecione o tomador de decisão principal no estágio (disponível somente depois de adicionar pelo menos uma pessoa ao estágio que tenha uma função de Aprovador ou superior). Se você selecionar um Tomador de decisão Principal, a opção <strong>Somente uma decisão necessária</strong> será desabilitada neste estágio.</p></td>
        </tr>
        <tr>
         <td role="rowheader">É necessária somente uma decisão</td>
         <td>Encerra todo o processo de revisão quando um dos tomadores de decisão toma uma decisão.<p>Esta opção não estará disponível se você tiver designado um usuário no menu suspenso <strong>Tomador de decisão principal</strong>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Estágio privado</td>
         <td>Permite que apenas as seguintes pessoas visualizem comentários e decisões tomadas durante esse estágio: Supervisores, administradores do Adobe Workfront e administradores do Workfront Proof</td>
        </tr>
        <tr>
         <td role="rowheader">Notificar pessoas por e-mail</td>
         <td>Alerta os revisores com uma notificação por email quando é a vez de trabalhar na prova.</td>
        </tr>
       </tbody>
      </table>

   1. Clique em **Adicionar estágio**.

1. Repita a etapa anterior conforme necessário para adicionar mais estágios.

   À medida que você adiciona estágios ao Fluxo de Trabalho Automatizado, um diagrama se forma na tela para representá-los:

   ![Diagrama de Fluxo de Trabalho](assets/workflow-diagram-existing-proof-qs-350x215.png)

1. Quando terminar de adicionar etapas, clique em **Concluído**.

## Sobre o uso de modelos de fluxo de trabalho automatizado {#about-using-automated-workflow-templates}

Considere o seguinte ao usar um modelo de Fluxo de trabalho automatizado:

1. As configurações de um modelo de Fluxo de trabalho automatizado determinam o que você pode fazer com o Fluxo de trabalho automatizado para uma prova. Por exemplo, se o botão Adicionar um estágio estiver desativado no modelo, ele não ficará visível enquanto você trabalhar com as configurações de Fluxo de trabalho automatizado para a prova.
1. Quando uma pessoa é adicionada a um estágio em um modelo de Fluxo de trabalho automatizado, mas também já está presente como revisor na prova, a aplicação do modelo remove o revisor do estágio. Se você não adicionar outro revisor ao estágio, uma mensagem solicitará que você adicione um.
1. Sua capacidade de modificar um modelo de Fluxo de trabalho automatizado depende das configurações do modelo definidas pelo administrador do Workfront, conforme descrito em . Se a capacidade de modificar o modelo estiver desativada, somente o proprietário do modelo poderá modificá-lo.

## Sobre a adição de revisores a um estágio {#about-adding-reviewers-to-a-stage}

Considere o seguinte ao adicionar revisores a um estágio:

* Depois de adicionar um usuário a um estágio, é possível definir as configurações para esse usuário na prova, como a função de prova e as permissões adicionais que ele deve ter, além do tipo de alertas de email que ele receberá quando as pessoas fizerem comentários e tomarem decisões sobre a prova.
* É possível arrastar um ou mais usuários de um estágio para outro. Você pode arrastar os usuários diretamente para outro estágio ou arrastar os usuários para um estágio no diagrama **Estágios**. Para selecionar vários usuários, pressione Shift+Ctrl (no Windows) ou Shift+Command (no Mac).
* É possível adicionar um revisor a uma prova apenas uma vez, o que significa que não é possível adicionar a mesma pessoa a mais de um estágio na prova.
* Os revisores que não são adicionados a um estágio privado não podem ver esse estágio na prova ou nos comentários feitos nesse estágio.
* Por padrão, adicionar um usuário a um estágio concede a ele acesso para visualizar a prova a partir do momento em que a prova é criada.

  O administrador do Workfront pode impedir que os usuários acessem a prova até que o fluxo de trabalho entre no estágio em que o usuário foi adicionado. Para obter mais informações, consulte  em .
