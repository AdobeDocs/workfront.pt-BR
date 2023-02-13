---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Criar e gerenciar modelos de Fluxo de trabalho automatizado
description: Como administrador da Adobe Workfront, se o processo de revisão de conteúdo da sua organização for repetido com frequência ou se o conteúdo for revisado com frequência pelas mesmas pessoas, você poderá criar modelos de Fluxo de trabalho automatizado que contenham esses revisores com funções de prova e configurações de notificação especificadas. Um modelo de Fluxo de trabalho automatizado pode ser simples com apenas um ou dois revisores ou complexos com vários estágios e dependências.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: a9f182c0-11cb-4e94-be86-b19ba5102faa
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '2096'
ht-degree: 0%

---

# Criar e gerenciar modelos de Fluxo de trabalho automatizado

Como administrador da Adobe Workfront, se o processo de revisão de conteúdo da sua organização for repetido com frequência ou se o conteúdo for revisado com frequência pelas mesmas pessoas, você poderá criar modelos de Fluxo de trabalho automatizado que contenham esses revisores com funções de prova e configurações de notificação especificadas. Um modelo de Fluxo de trabalho automatizado pode ser simples com apenas um ou dois revisores ou complexos com vários estágios e dependências.

Os modelos de Fluxo de trabalho automatizado facilitam a criação de uma prova com um Fluxo de trabalho automatizado. Quando um usuário cria uma prova, ele simplesmente escolhe o template necessário.

Você pode alterar facilmente qualquer modelo de Fluxo de trabalho automatizado, adicionando ou removendo revisores e estágios, a qualquer momento. E os criadores de prova que usam o modelo podem adicionar ou remover revisores para a prova.

Considere o seguinte ao usar um modelo de Fluxo de trabalho automatizado:

1. As configurações de um modelo de Fluxo de trabalho automatizado determinam o que você pode fazer com o Fluxo de trabalho automatizado para uma prova. Por exemplo, se o botão Add a stage estiver desativado no template, ele não estará visível à medida que você trabalha com as configurações do Automated Workflow para a prova.
1. Quando uma pessoa é adicionada a uma página em um modelo de Fluxo de trabalho automatizado, mas também já está presente como um revisor na prova, a aplicação do modelo remove o revisor do estágio. Se você não adicionar outro revisor ao palco, uma mensagem solicitará que você adicione um.
1. A capacidade de modificar um modelo de Fluxo de trabalho automatizado depende das configurações do modelo definidas pelo administrador do Workfront, conforme descrito em . Se a capacidade de modificar o modelo estiver desativada, somente o proprietário do modelo poderá modificá-lo.

Para obter informações sobre fluxos de trabalho automatizados, consulte [Visão geral do fluxo de trabalho automatizado](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

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

## Criar um modelo de Fluxo de trabalho automatizado

1. No Workfront, clique no Menu principal ![](assets/main-menu-icon.png)e, em seguida, clique em Verificação ![](assets/proofing-in-main-menu.png) para acessar o Workfront Proof.
1. Clique em **Fluxos de trabalho** no painel esquerdo.
1. No **Fluxo de trabalho** clique em **Novo** > **Novo modelo**.

1. No **Detalhes** especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome do modelo</td> 
      <td>(Obrigatório) Digite um nome para o modelo. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proprietário do modelo</td> 
      <td>Você pode selecionar o administrador do Workfront ou o administrador do Workfront Proof que gerenciará o modelo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Grupo de modelos</td> 
      <td> <p> Se os fluxos de trabalho automatizados da sua organização estiverem organizados em grupos, você poderá selecionar o nome do grupo. Consulte <a href="#create-automated-workflow-template-groups" class="MCXref xref">Criar grupos de modelo de Fluxo de trabalho automatizado</a> mais adiante neste artigo para obter mais informações.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Fuso horário de modelo </td> 
      <td> <p>O fuso horário padrão do modelo é aquele em que você está trabalhando. Se o fuso horário dos criadores e revisores de prova que usarão o modelo for diferente, você poderá alterá-lo aqui para garantir que os prazos do estágio sejam definidos no momento certo para esses usuários. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir</td> 
      <td> <p>Você pode selecionar as atividades de estágio que deseja disponibilizar para a pessoa cria provas usando o modelo.</p> <!--
        <p><b>WARNING</b>: If you don't select the options Add a stage and Add people to stages, neither the template owner nor the owner of any proof using this template will be able to add a stage or share the proof. <!--
          <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Test this. Andrzej thinks it's wrong info or a bug.</span>
         --></p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. No **Estágios** , configure cada estágio do modelo de Fluxo de trabalho automatizado.

   É possível adicionar vários estágios e criar entre eles.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>O nome do palco é exibido no diagrama de Fluxo de trabalho automatizado na parte superior da seção Fluxo de trabalho, na página Detalhes da prova e nas notificações por email enviadas aos revisores.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ativar estágio</td> 
      <td> <p>Especifique se o estágio é ativado automática ou manualmente. Para o primeiro estágio, você pode selecionar <strong>Na criação da prova</strong>, <strong>Em uma data e hora específicas</strong>ou <strong>Manualmente</strong>.</p> <p>As outras opções ficam disponíveis ao adicionar uma segunda etapa, pois exigem que você selecione uma etapa principal. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prazo calculado a partir de</td> 
      <td> <p>Especifique como deseja calcular o prazo:</p> 
       <ul> 
        <li> <p><strong>Criação de prova</strong>: Na lista suspensa em <strong>Prazo (+ dias úteis)</strong>, selecione o número de dias úteis que deseja adicionar à data de criação da prova para definir automaticamente um prazo na prova.</p> </li> 
        <li><strong>Quando o estágio começa</strong>: Na lista suspensa em <strong>Prazo (+ dias úteis)</strong>, selecione o número de dias úteis que deseja adicionar à data de ativação do estágio para definir automaticamente um prazo na prova.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear palco</td> 
      <td>Especifique se deseja permitir que o palco seja bloqueado para comentários. As opções são bloquear um estágio manualmente ou automaticamente, quando o próximo estágio inicia ou quando todas as decisões são tomadas no estágio principal.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tomador de decisão primário</td> 
      <td> <p>Os tomadores de decisão disponíveis são exibidos na lista somente após ter adicionado os revisores ao palco.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">É necessária somente uma decisão</td> 
      <td>O processo de revisão da fase será concluído assim que um dos decisores apresentar a sua decisão. Para obter mais informações, consulte <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Definir configurações de prova na Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fase privada</td> 
      <td>Oculta comentários e decisões de para pessoas que não são adicionadas ao palco ou que não são administradores do Workfront&lt;!&gt;— DESENHADO EM FLARE: Autoridades de supervisão

       -->. Para obter mais informações, consulte &lt;a href=&quot;../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md&quot; class=&quot;MCXref xref&quot;>Visão geral do fluxo de trabalho automatizado&lt;/a>.&lt;/td>
   </tr> 
     <tr> 
      <td role="rowheader">Não permitir que esta fase seja eliminada</td> 
      <td> <p>Torna o estágio obrigatório.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Se as provas que usarão esse modelo forem sempre enviadas para as mesmas pessoas no palco, adicione-as aqui para que os usuários não precisem adicioná-las sempre que criarem uma prova.

   Escolha o **Função** nas provas que usarão este modelo e a variável **Alertas por email** você deseja que o usuário receba ao trabalhar com provas que usam esse modelo.

   Para obter informações sobre funções em uma prova, consulte [Configurar funções de prova padrão](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md). Para obter informações sobre alertas de email de prova, consulte a seção [Configurar padrões de prova para um usuário](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur) no artigo  [Definir configurações de notificação de email no Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Cada usuário pode ser adicionado a apenas um estágio. Você pode adicionar quantos usuários quiser a um palco.

   >[!TIP]
   >
   >Você pode arrastar e soltar nomes de revisores entre estágios no diagrama de estágios. Os estágios disponíveis são destacados em azul.

1. Repita as duas etapas anteriores para qualquer outro estágio que desejar adicionar ao modelo.

   Na parte superior do **Fluxo de trabalho** , você pode ver um diagrama do Fluxo de trabalho automatizado que está configurando. À medida que você continua a adicionar palcos, eles aparecem no diagrama com linhas que mostram as dependências entre eles. Você pode clicar em um estágio no diagrama para exibir as configurações desse estágio.

   Se não precisar ver o diagrama, clique em **Ocultar Diagrama**.

1. No **Compartilhar modelo com** clique em uma opção (se o modelo ainda não estiver compartilhado com a organização inteira) para especificar quem poderá usá-lo.

   Por padrão, os novos modelos de Fluxo de trabalho automatizado são compartilhados com todos em sua organização.

1. Clique em **Criar**.

## Modificar um modelo de Fluxo de trabalho automatizado

Como administrador da Workfront Proof, você pode modificar um modelo de Fluxo de trabalho automatizado. As alterações são salvas automaticamente à medida que você as faz.

1. No Workfront, clique no Menu principal ![](assets/main-menu-icon.png)e, em seguida, clique em Verificação ![](assets/proofing-in-main-menu.png) para acessar o Workfront Proof.
1. Clique em **Fluxos de trabalho** no painel esquerdo.
1. No **Templates de workflow** for exibida, clique no modelo que deseja modificar.
1. No **Detalhes** especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome do modelo</td> 
      <td>(Obrigatório) Digite um nome para o modelo. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proprietário do modelo</td> 
      <td>Você pode selecionar o administrador do Workfront ou o administrador do Workfront Proof que gerenciará o modelo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Grupo de modelos</td> 
      <td> <p> Se os fluxos de trabalho automatizados da sua organização estiverem organizados em grupos, você poderá selecionar o nome do grupo. Consulte <a href="#create-automated-workflow-template-groups" class="MCXref xref">Criar grupos de modelo de Fluxo de trabalho automatizado</a> mais adiante neste artigo para obter mais informações.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fuso horário de modelo </td> 
      <td> <p>O fuso horário padrão do modelo é aquele em que você está trabalhando. Se o fuso horário dos criadores e revisores de prova que usarão o modelo for diferente, você poderá alterá-lo aqui para garantir que os prazos do estágio sejam definidos no momento certo para esses usuários. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir</td> 
      <td> <p>Selecione as atividades de estágio que deseja disponibilizar para aqueles que criam provas usando o template. </p> <p><b>AVISO</b>: Se você não selecionar as opções Adicionar um palco e Adicionar pessoas aos palcos, nem o proprietário do modelo nem o proprietário de qualquer prova usando este modelo poderão adicionar um palco ou compartilhar a prova.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. No **Fluxo de trabalho** alterar o nome de qualquer estágio e expandir suas configurações ![](assets/arrow-button.png) para fazer as alterações necessárias:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Prazo calculado a partir de</td> 
      <td> <p>Especifique como deseja calcular o prazo:</p> 
       <ul> 
        <li> <p><strong>Prazo calculado a partir da criação da prova</strong>: No <strong>Definir o prazo do estágio</strong> na lista suspensa, selecione o número de dias úteis que deseja adicionar à data de criação da prova para definir automaticamente um prazo na prova.</p> </li> 
        <li><strong>Prazo calculado a partir da ativação do estágio</strong>: No <strong>Definir o prazo do estágio</strong> na lista suspensa, selecione o número de dias úteis que deseja adicionar à data de ativação do estágio para definir automaticamente um prazo na prova.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ativar estágio</td> 
      <td> <p>Especifique se o estágio é ativado automática ou manualmente. Para o primeiro estágio, você pode selecionar <strong>Na criação da prova</strong>, <strong>Em uma data e hora específicas</strong>ou <strong>Manualmente</strong>.</p> <p>As outras opções ficam disponíveis ao adicionar uma segunda etapa, pois exigem que você selecione uma etapa principal. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear palco</td> 
      <td>Especifique se deseja permitir que o palco seja bloqueado para comentários. As opções são bloquear um estágio manualmente ou automaticamente, quando o próximo estágio inicia ou quando todas as decisões são tomadas no estágio principal.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisão</td> 
      <td>Termina a fase na primeira vez que um dos decisores apresentar a sua decisão. Para obter mais informações, consulte <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Definir configurações de prova na Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Privacidade</td> 
      <td>Oculta comentários e decisões de pessoas que não são adicionadas ao palco ou que não são Supervisores ou superiores na conta. Para obter mais informações, consulte <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Visão geral do fluxo de trabalho automatizado</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exclusão de estágio</td> 
      <td>Torna o estágio obrigatório.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mais <img src="assets/more-icon.png"></td> 
      <td>Adicione revisores ao palco ou exclua o palco.<p>Se cada uma das provas for enviada para as mesmas pessoas em um estágio específico, você pode especificar os nomes aqui para não precisar adicioná-las toda vez que criar uma prova. Digite e selecione o nome de um usuário que deseja adicionar ao palco e adicione-o <strong>Função</strong> na prova e <strong>Alertas por email</strong> configurações desejadas para o usuário. Para obter informações sobre revisão de funções, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">Configurar funções de prova padrão</a>. Para obter informações sobre alertas de email de prova, consulte a seção <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">Configurar padrões de prova para um usuário</a> no artigo <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Definir configurações de notificação de email no Workfront Proof</a>.</p><p>Você pode adicionar quantos usuários quiser em um palco</p><p>Dica: Você pode arrastar e soltar nomes de revisores entre estágios no diagrama de estágios. Os estágios disponíveis são destacados em azul.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Repita a etapa para qualquer outro estágio que desejar adicionar ao modelo.

   Na parte superior do **Fluxo de trabalho** , você pode ver um diagrama do Fluxo de trabalho automatizado que está configurando. À medida que você continua a adicionar palcos, eles aparecem no diagrama com linhas que mostram as dependências entre eles. Você pode clicar em um estágio no diagrama para exibir as configurações desse estágio.

   Se não precisar ver o diagrama, clique em **Ocultar Diagrama**.

1. No **Compartilhado com** , se quiser excluir um usuário, clique no botão Mais ![](assets/more-icon.png) à direita e clique em **Remover**.

## Criar grupos de modelo de Fluxo de trabalho automatizado {#create-automated-workflow-template-groups}

Como administrador da Workfront, você pode exibir e gerenciar todos os modelos de Fluxo de trabalho automatizado na conta da sua organização. Pode ser útil organizar modelos em grupos.

Para criar um grupo de modelo de Fluxo de trabalho automatizado:

1. No Workfront, clique no Menu principal ![](assets/main-menu-icon.png)e, em seguida, clique em Verificação ![](assets/proofing-in-main-menu.png) para acessar o Workfront Proof.
1. Clique em **Fluxos de trabalho** no painel esquerdo.
1. No **Fluxo de trabalho** clique em **Novo** > **Novo grupo de modelos**.
1. Digite um nome descritivo para o novo grupo de modelos e pressione **Enter**.

Você pode mover os modelos entre grupos arrastando e soltando.

## Gerenciar modelos de fluxo de trabalho automatizado

1. No Workfront, clique no Menu principal ![](assets/main-menu-icon.png)e, em seguida, clique em Verificação ![](assets/proofing-in-main-menu.png) para acessar o Workfront Proof.

1. No painel esquerdo da Workfront Proof, clique em **Fluxos de trabalho**.
1. No **Fluxos de trabalho** na página exibida, execute um dos seguintes procedimentos:

   * Adicionar um novo modelo
   * Adicionar um novo grupo de modelos
   * Excluir um ou mais grupos de modelo
   * Acessar os detalhes de um modelo
   * Arrastar um modelo para um grupo de modelos diferente
