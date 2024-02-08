---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Criar e gerenciar modelos de fluxo de trabalho automatizado
description: Como administrador do Adobe Workfront, se o processo de revisão de conteúdo da sua organização for repetido com frequência ou o conteúdo for revisado com frequência pelas mesmas pessoas, você poderá criar modelos de Fluxo de trabalho automatizado que contenham esses revisores com funções de prova e configurações de notificação especificadas. Um modelo de fluxo de trabalho automatizado pode ser simples com apenas um ou dois revisores ou complexo com vários estágios e dependências.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: a9f182c0-11cb-4e94-be86-b19ba5102faa
source-git-commit: ccfea4cdf7280f992068bc64bab27e63aaab8b74
workflow-type: tm+mt
source-wordcount: '2056'
ht-degree: 0%

---

# Criar e gerenciar modelos de fluxo de trabalho automatizado

<!-- Audited: 2/2024 -->

Como administrador do Adobe Workfront, se o processo de revisão de conteúdo da sua organização for repetido com frequência ou o conteúdo for revisado com frequência pelas mesmas pessoas, você poderá criar modelos de Fluxo de trabalho automatizado que contenham esses revisores com funções de prova e configurações de notificação especificadas. Um modelo de fluxo de trabalho automatizado pode ser simples com apenas um ou dois revisores ou complexo com vários estágios e dependências.

Os modelos de fluxo de trabalho automatizado facilitam a criação de uma prova com um fluxo de trabalho automatizado. Quando um usuário cria uma prova, ele simplesmente escolhe o modelo que precisa.

É possível alterar facilmente qualquer modelo de Fluxo de trabalho automatizado, adicionando ou removendo revisores e estágios, a qualquer momento. Os criadores de prova que usam o modelo podem adicionar ou remover revisores para a prova.

Considere o seguinte ao usar um modelo de Fluxo de trabalho automatizado:

1. As configurações de um modelo de Fluxo de trabalho automatizado determinam o que você pode fazer com o Fluxo de trabalho automatizado para uma prova. Por exemplo, se o botão Adicionar um estágio estiver desativado no modelo, ele não ficará visível enquanto você trabalhar com as configurações de Fluxo de trabalho automatizado para a prova.
1. Quando uma pessoa é adicionada a um estágio em um modelo de Fluxo de trabalho automatizado, mas também já está presente como revisor na prova, a aplicação do modelo remove o revisor do estágio. Se você não adicionar outro revisor ao estágio, uma mensagem solicitará que você adicione um.
1. Sua capacidade de modificar um modelo de Fluxo de trabalho automatizado depende das configurações do modelo definidas pelo administrador do Workfront, conforme descrito em . Se a capacidade de modificar o modelo estiver desativada, somente o proprietário do modelo poderá modificá-lo.

Para obter informações sobre Workflows automatizados, consulte [Visão geral do fluxo de trabalho automatizado](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Novo: Qualquer um</p><p>Atual: Pro ou superior</p><p>Herdados: Premium ou Select</p> <p>Para obter mais informações sobre acesso de prova com os diferentes planos, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de prova no Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Novo: Padrão</p><p>Atual: Trabalho ou Plano</p> <p>Herdado: qualquer um (Você deve ter a prova ativada para o usuário)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>É necessário ter Administrador selecionado no seu Perfil de permissão de prova. </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Criar um modelo de fluxo de trabalho automatizado

{{step1-to-proofing}}

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
      <td>É possível selecionar o administrador do Workfront ou o administrador do Workfront Proof que gerenciará o modelo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Grupo de modelos</td> 
      <td> <p> Se os fluxos de trabalho automatizados de sua organização estiverem organizados em grupos, você poderá selecionar o nome do grupo. Consulte <a href="#create-automated-workflow-template-groups" class="MCXref xref">Criar grupos de modelo de fluxo de trabalho automatizado</a> neste artigo para obter mais informações.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Fuso horário de modelo </td> 
      <td> <p>O fuso horário padrão do modelo é aquele em que você está trabalhando. Se o fuso horário dos criadores e revisores de prova que usarão o modelo for diferente, você poderá alterá-lo aqui para garantir que os prazos de preparo sejam definidos nos momentos certos para esses usuários. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir</td> 
      <td> <p>É possível selecionar as atividades de preparo que você deseja que estejam disponíveis para a pessoa que cria provas usando o modelo.</p> 
      <p><b>AVISO</b>: se você não selecionar as opções Adicionar um estágio e Adicionar pessoas aos estágios, o proprietário do modelo e o proprietário de qualquer prova que esteja usando esse modelo não poderão adicionar um estágio ou compartilhar a prova. 
      </p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. No **Estágios** configure cada estágio do modelo de Fluxo de Trabalho Automatizado.

   É possível adicionar vários estágios e criar entre eles.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>O nome do estágio é exibido no diagrama de Fluxo de trabalho automatizado na parte superior da seção Fluxo de trabalho, na página Detalhes da prova e nas notificações por email enviadas aos revisores.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ativar estágio</td> 
      <td> <p>Especifique se o estágio é ativado automática ou manualmente. Para o primeiro estágio, é possível selecionar <strong>Na criação da prova</strong>, <strong>Em uma data e hora específicas</strong>ou <strong>Manualmente</strong>.</p> <p>As outras opções ficam disponíveis quando você adiciona um segundo estágio, pois exigem que você selecione um estágio principal. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prazo calculado de</td> 
      <td> <p>Especifique como deseja que o prazo seja calculado:</p> 
       <ul> 
        <li> <p><strong>Criação de prova</strong>: Na lista suspensa em <strong>Prazo (+ dias úteis)</strong>, selecione o número de dias úteis que deseja adicionar à data de criação da prova para definir automaticamente um prazo na prova.</p> </li> 
        <li><strong>Quando o estágio começa</strong>: Na lista suspensa em <strong>Prazo (+ dias úteis)</strong>, selecione o número de dias úteis que deseja adicionar à data de ativação do estágio para definir automaticamente um prazo na prova.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear estágio</td> 
      <td>Especifique se deseja permitir que o estágio seja bloqueado para comentários. As opções são bloquear um estágio manual ou automaticamente, quando o próximo estágio é iniciado ou quando todas as decisões são tomadas no estágio principal.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tomador de decisão primário</td> 
      <td> <p>Os tomadores de decisão disponíveis são exibidos na lista somente após adicionar os revisores ao estágio.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">É necessária somente uma decisão</td> 
      <td>O processo de revisão da fase será concluído assim que um dos tomadores de decisão apresentar a sua decisão. Para obter mais informações, consulte <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Definir configurações de prova no Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Estágio privado</td> 
      <td>Oculta comentários e decisões de para pessoas que não foram adicionadas ao estágio ou que não são administradores do Workfront. Para obter mais informações, consulte <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Visão geral do fluxo de trabalho automatizado</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Não permitir que este estágio seja excluído</td> 
      <td> <p>Torna o estágio obrigatório.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Se as provas que usarão esse template forem sempre enviadas para as mesmas pessoas no estágio, adicione-as aqui para que os usuários não precisem adicioná-las sempre que criarem uma prova.

   Escolha o de cada pessoa **Função** sobre as provas que usarão esse modelo e o **Alertas de email** que você deseja que o usuário receba ao trabalhar em provas que usam esse template.

   Para obter informações sobre funções em uma prova, consulte [Configurar funções de prova padrão](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md). Para obter informações sobre alertas de email de prova, consulte a seção [Configurar padrões de prova para um usuário](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur) no artigo  [Definir configurações de notificação por email no Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Cada usuário pode ser adicionado a apenas um estágio. Você pode adicionar quantos usuários quiser a um estágio.

   >[!TIP]
   >
   >Você pode arrastar e soltar nomes de revisores entre estágios no diagrama de estágios. As etapas disponíveis são destacadas em azul.

1. Repita as duas etapas anteriores para quaisquer outros estágios que deseja adicionar ao modelo.

   Na parte superior do **Fluxo de trabalho** é possível ver um diagrama do Fluxo de trabalho automatizado que está sendo configurado. À medida que você continua a adicionar estágios, eles aparecem no diagrama com linhas mostrando as dependências entre eles. Você pode clicar em um estágio no diagrama para exibir as configurações desse estágio.

   Se não precisar ver o diagrama, clique em **Ocultar Diagrama**.

1. No **Compartilhar modelo com** clique em uma opção (se o modelo ainda não estiver compartilhado com toda a organização) para especificar quem poderá usá-lo.

   Por padrão, os novos modelos de Fluxo de trabalho automatizado são compartilhados com todos em sua organização.

1. Clique em **Criar**.

## Modificar um modelo de fluxo de trabalho automatizado

Como administrador do Workfront Proof, você pode modificar um modelo de fluxo de trabalho automatizado. Suas alterações são salvas automaticamente à medida que são feitas.

{{step1-to-proofing}}

1. Clique em **Fluxos de trabalho** no painel esquerdo.
1. No **Modelos de fluxo de trabalho** que for exibida, clique no modelo que você deseja modificar.
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
      <td>É possível selecionar o administrador do Workfront ou o administrador do Workfront Proof que gerenciará o modelo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Grupo de modelos</td> 
      <td> <p> Se os fluxos de trabalho automatizados de sua organização estiverem organizados em grupos, você poderá selecionar o nome do grupo. Consulte <a href="#create-automated-workflow-template-groups" class="MCXref xref">Criar grupos de modelo de fluxo de trabalho automatizado</a> neste artigo para obter mais informações.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fuso horário de modelo </td> 
      <td> <p>O fuso horário padrão do modelo é aquele em que você está trabalhando. Se o fuso horário dos criadores e revisores de prova que usarão o modelo for diferente, você poderá alterá-lo aqui para garantir que os prazos de preparo sejam definidos nos momentos certos para esses usuários. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir</td> 
      <td> <p>Selecione as atividades de estágio que você deseja disponibilizar para aqueles que criam provas usando o template. </p> <p><b>AVISO</b>: se você não selecionar as opções Adicionar um estágio e Adicionar pessoas aos estágios, o proprietário do modelo e o proprietário de qualquer prova que esteja usando esse modelo não poderão adicionar um estágio ou compartilhar a prova.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. No **Fluxo de trabalho** altere o nome de qualquer estágio e expanda suas configurações ![](assets/arrow-button.png) para fazer as alterações necessárias:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Prazo calculado de</td> 
      <td> <p>Especifique como deseja que o prazo seja calculado:</p> 
       <ul> 
        <li> <p><strong>Prazo calculado a partir da criação da prova</strong>: na caixa <strong>Definir o prazo final do estágio</strong> selecione o número de dias úteis que deseja adicionar à data de criação da prova para definir automaticamente um prazo na prova.</p> </li> 
        <li><strong>Prazo calculado a partir da ativação do estágio</strong>: na caixa <strong>Definir o prazo final do estágio</strong> selecione o número de dias úteis que deseja adicionar à data de ativação do estágio para definir automaticamente um prazo na prova.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ativar estágio</td> 
      <td> <p>Especifique se o estágio é ativado automática ou manualmente. Para o primeiro estágio, é possível selecionar <strong>Na criação da prova</strong>, <strong>Em uma data e hora específicas</strong>ou <strong>Manualmente</strong>.</p> <p>As outras opções ficam disponíveis quando você adiciona um segundo estágio, pois exigem que você selecione um estágio principal. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear estágio</td> 
      <td>Especifique se deseja permitir que o estágio seja bloqueado para comentários. As opções são bloquear um estágio manual ou automaticamente, quando o próximo estágio é iniciado ou quando todas as decisões são tomadas no estágio principal.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisão</td> 
      <td>Termina o estágio na primeira vez que um dos tomadores de decisão envia sua decisão. Para obter mais informações, consulte <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Definir configurações de prova no Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Privacidade</td> 
      <td>Oculta comentários e decisões de para pessoas que não foram adicionadas ao estágio ou que não são Supervisores e superiores na conta. Para obter mais informações, consulte <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Visão geral do fluxo de trabalho automatizado</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exclusão de preparo</td> 
      <td>Torna o estágio obrigatório.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mais <img src="assets/more-icon.png"></td> 
      <td>Adicione revisores ao estágio ou exclua o estágio.<p>Se cada uma de suas provas for enviada para as mesmas pessoas em um estágio específico, você poderá especificar seus nomes aqui e nomeá-los para que não precise adicioná-los toda vez que criar uma prova. Digite e selecione o nome de um usuário que deseja adicionar ao estágio e, em seguida, adicione seus <strong>Função</strong> sobre a prova e <strong>Alertas de email</strong> configurações desejadas para o usuário. Para obter informações sobre funções de prova, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">Configurar funções de prova padrão</a>. Para obter informações sobre alertas de email de prova, consulte a seção <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">Configurar padrões de prova para um usuário</a> no artigo <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Definir configurações de notificação por email no Workfront Proof</a>.</p><p>Você pode adicionar quantos usuários quiser a um estágio</p><p>Dica: você pode arrastar e soltar nomes de revisores entre estágios no diagrama de estágios. As etapas disponíveis são destacadas em azul.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Repita a etapa para quaisquer outros estágios que deseja adicionar ao modelo.

   Na parte superior do **Fluxo de trabalho** é possível ver um diagrama do Fluxo de trabalho automatizado que está sendo configurado. À medida que você continua a adicionar estágios, eles aparecem no diagrama com linhas mostrando as dependências entre eles. Você pode clicar em um estágio no diagrama para exibir as configurações desse estágio.

   Se não precisar ver o diagrama, clique em **Ocultar Diagrama**.

1. No **Compartilhado com** seção, se quiser excluir um usuário, clique no botão Mais ![](assets/more-icon.png) à direita e clique em **Remover**.

## Criar grupos de modelo de fluxo de trabalho automatizado {#create-automated-workflow-template-groups}

Como administrador do Workfront, você pode visualizar e gerenciar todos os modelos de Fluxo de trabalho automatizado na conta da sua organização. Pode ser útil organizar modelos em grupos.

Para criar um grupo de modelos de Fluxo de trabalho automatizado:

{{step1-to-proofing}}

1. Clique em **Fluxos de trabalho** no painel esquerdo.
1. No **Fluxo de trabalho** clique em **Novo** > **Novo grupo de modelos**.
1. Digite um nome descritivo para o novo grupo de modelos e pressione **Enter**.

Você pode mover os modelos entre grupos arrastando e soltando.

## Gerenciar modelos de fluxo de trabalho automatizado

{{step1-to-proofing}}

1. No painel esquerdo, em Workfront Proof, clique em **Fluxos de trabalho**.
1. No **Fluxos de trabalho** que for exibida, siga um destes procedimentos:

   * Adicionar um novo modelo
   * Adicionar um novo grupo de modelos
   * Excluir um ou mais grupos de modelos
   * Acessar os detalhes de um modelo
   * Arrastar um modelo para outro grupo de modelos
