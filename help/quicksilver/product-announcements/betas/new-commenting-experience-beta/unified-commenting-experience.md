---
product-area: betas
navigation-topic: new-commenting-experience-beta
title: Nova experiência de comentários
description: Uma atualização para a experiência de comentários no Adobe Workfront está em desenvolvimento no momento. Esta atualização inclui uma nova interface, novos recursos e melhor desempenho na seção Atualizações de objetos selecionados.
author: Alina
feature: Product Announcements
role: User
hide: true
hidefromtoc: true
exl-id: f750b35b-8021-4cc1-81d6-e1ece2530438
source-git-commit: 1eb1e919bede7e366956d8c0bd969329a641123f
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 1%

---

# Nova experiência de comentários

<!--take out legacy, preview, prod references from below-->

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers.</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

-->

>[!IMPORTANT]
>
>As informações neste artigo se referem aos recursos que foram lançados para a nova experiência de comentários.
>
>O programa beta para a nova experiência de comentários começou em abril de 2023 e terminou em outubro de 2023, com a versão de outubro de 2023.
>
>Desde 11 de abril de 2024, todos os recursos da nova experiência de comentários estão disponíveis no ambiente de produção para todos os clientes.
>
> A experiência de comentários anterior foi removida do Workfront.

## Recursos

A nova experiência de comentários inclui melhorias e alterações na seção Atualizações de objetos do Adobe Workfront.

Entre as melhorias incluídas na nova experiência de comentários estão as seguintes:

* Melhor desempenho e experiência do usuário
* Separação dos comentários do usuário das atualizações de atividade do sistema
* Indicador em tempo real quando novos comentários são adicionados a um objeto
* Edição de comentários após o envio

Os seguintes recursos foram removidos da nova experiência:

* Comentar em uma atualização do sistema. Comentários adicionados às atualizações do sistema no passado foram importados como comentários somente leitura na nova guia Atividade do sistema.
* Capacidade de editar Status, Condição, Data de confirmação e Percentual concluído ao comentar tarefas e problemas.

  Como alternativa, recomendamos que você adicione esses campos no painel Resumo de tarefas e problemas para acessá-los facilmente a partir de listas, da Página inicial, do Workfront Balancer ou de uma folha de horas.
* Capacidade de editar o formulário personalizado
* A informação &quot;em nome de &lt; user name >&quot; quando um administrador de Workfront ou grupo faz logon como outro usuário e adiciona um comentário em nome dele foi originalmente removida. Ele foi restabelecido em 19 de outubro de 2023.
* A opção &quot;Solicitar aprovação&quot; ao marcar pessoas ao adicionar um comentário a um documento.
* A configuração &quot;Mostrar o percentual concluído na atualização do status&quot; ao editar a caixa de perfil de um usuário será removida. A funcionalidade de atualizar o percentual concluído de uma tarefa ou problema foi removida.


<!--removed this note on November 28, 2023, when this limitation was removed: 

>[!NOTE]
>
>The objects listed below have only the comments and system updates starting with January 1, 2019 available in the new commenting experience.  
>
>You can view comments and system updates on these objects prior to January 1, 2019 when viewing the Updates section in the current experience:
>
>* Issues
>* Projects
>* Tasks
>* Documents

For more information, see the [New commenting experience FAQs](../../betas/new-commenting-experience-beta/new-commenting-faq.md). 
-->

A tabela a seguir ilustra os recursos que estarão disponíveis na nova experiência de comentários, bem como sua disponibilidade em áreas onde são compatíveis:

<table>
  <tr>
   <td><strong>Recurso </strong>
   </td>
   <td><strong>Existente na experiência de comentários antiga </strong>
   </td>
   <td><strong>Existe na nova experiência de comentários </strong>
   </td>

<td><strong>Introduzido na nova experiência de comentários </strong>
   </td>
   </tr>
  <tr>
   <td>Criar/ler/responder/excluir comentários 
   </td>
   <td>✓ µ 
  </td>
   <td>✓ µ 
   </td>

<td> 
   </td>

</tr>
  <tr>
   <td>Rich text (exclui aspas e emojis)
   </td>
   <td>✓ µ 
   </td>
   <td>✓ µ
   </td>

<td> 
   </td>
   &gt;
  </tr>

<tr>
   <td>Rich text (emojis)
   </td>
   <td>✓ µ 
   </td>
   <td>✓ µ
   </td>
   <td> 
   </td>

</tr>

<tr>
   <td>Rich text (aspas de bloco)
   </td>
   <td>✓ µ 
   </td>
   <td> ✓ µ
   </td>
    <td> 2 o trim. de 2023
   </td>

</tr>
  <tr>
<tr>
   <td> Citar comentários
   </td>
   <td>✓ µ 
   </td>
   <td> ✓ µ
   </td>
   <td> 2 o trim. de 2023
   </td>

</tr>
  <tr>
   <td>Reagir a comentários (Curtir) 
   </td>
   <td>✓ µ 
   </td>
   <td>✓ µ 
   </td>
   <td> 
   </td>

</tr>
  <tr>
   <td>Anexar imagens a comentários 
   </td>
   <td>✓ µ 
   </td>
   <td>✓ µ 
   </td>
      <td> 
   </td>

</tr>
  <tr>
   <td>Marcar pessoas em comentários 
   </td>
   <td>✓ µ 
   </td>
   <td>✓ µ 
   </td>
   <td> 
   </td>

</tr>
  <tr>
   <td>Remover participantes do thread
   </td>
   <td> 
   </td>
   <td>✓ µ
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Marcar automaticamente todos os participantes do thread
   </td>
   <td> 
   </td>
   <td>✓ µ
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Comentários privados de uma empresa 
   </td>
   <td>✓ µ 
   </td>
   <td>✓ µ 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Desfazer postagem de um comentário 
   </td>
   <td>✓ µ 
   </td>
   <td>Substituído pelo comentário de edição 
   </td>
     <td> 
   </td>
  </tr>
  <tr>
   <td>Desativar atualizações do sistema 
   </td>
   <td>✓ µ 
   </td>
   <td>Substituído pela guia Atividade 
   </td>
   <td> 
   </td>
    </tr>
  <tr>
   <td>Editar comentários 
   </td>
   <td> 
   </td>
   <td> ✓ µ
   </td>
   <td> 
   </td>
    </tr>
  <tr>
   <td>Salvar rascunhos de comentários ao sair da página 
   </td>
   <td>✓ µ 
   </td>
   <td>✓ µ 
   </td>
   <td> 
   </td>
    </tr>
  <tr>
   <td>Ver novos comentários em tempo real (inclui ver quando um comentário é excluído)
   </td>
   <td> 
   </td>
   <td>✓ µ
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Registrar de tempo 
   </td>
   <td>✓ µ 
   </td>
   <td>✓ µ
   </td>
   <td> 
   </td>
  </tr>
    <tr>
   <td>Copiar link da discussão 
   </td>
   <td>✓ µ 
   </td>
   <td> Substituído pelo link Copiar
   </td>
   <td>2 o trim. de 2023 
   </td>
  </tr>
  <tr>
   <td>Copiar link do comentário 
   </td>
   <td>✓ µ 
   </td>
   <td> Substituído pelo link Copiar
   </td>
   <td> 
   </td>
    </tr>
  <tr>
   <td>Citar texto de comentário 
   </td>
   <td>✓ µ 
   </td>
   <td>✓ µ
   </td>
  <td>2 o trim. de 2023 
   </td>
   </tr>
  <tr>
   <td>Copiar texto do corpo 
   </td>
   <td>✓ µ 
   </td>
   <td> ✓ µ
   </td>
   <td>
   </td>
   </tr>
    <tr>
   <td>Pesquisar em comentários 
   </td>
   <td> 
   </td>
   <td> ✓ µ
   </td>
   <td>1º trim. de 2024 
   </td>

</tr>

<tr>
   <td>Copiar e colar imagens em um comentário
   </td>
   <td> 
   </td>
   <td> ✓ µ
   </td>
   <td>1º trim. de 2024 
   </td>
     </tr>

<tr>
   <td>Arrastar e soltar imagens em um comentário
   </td>
   <td> ✓ µ
   </td>
   <td> ✓ µ
   </td>
   <td>1º trim. de 2024 
   </td>
    </tr>

<tr>
   <td>Editar formulário personalizado 
   </td>
   <td>✓ µ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Capacidade de editar Status, Condição, Data de confirmação ao comentar 
   </td>
   <td>✓ µ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
<tr>
   <td>Responder a atualizações do sistema 
   </td>
   <td> ✓ µ
   </td>
   <td> 
   </td>
   <td>
   </td>
  </tr>
<tr>
   <td>Exibir "em nome de" ao adicionar comentários conectados como outro usuário
   </td>
   <td> ✓ µ
   </td>
   <td> ✓ µ
   </td>
   <td>
   </td>
  </tr>

<tr>
   <td>Capacidade do Proprietário do Projeto de alterar a Data de Conclusão Planejada de uma tarefa quando a Data de Compromisso é alterada na seção Atualizações
   </td>
   <td> ✓ µ
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
</table>

## Linha do tempo de lançamento

>[!IMPORTANT]
>
>Para obter informações sobre os recursos lançados para a nova experiência de comentários durante o período beta, consulte [Nova atividade de lançamento de experiência beta de comentários](../../betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md).
>
>Para obter mais informações sobre como gerenciar atualizações para objetos do Workfront, consulte [Trabalho de atualização](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).


As informações a seguir descrevem a linha do tempo com os principais marcos para o lançamento da nova experiência de comentários para o ambiente de produção. Além dos marcos abaixo, continuaremos a melhorar a experiência de comentários com aprimoramentos menores.

Para obter informações sobre os recursos lançados para a nova experiência de comentários após o encerramento do período beta, consulte a página de visão geral da versão atual. Para obter mais informações, consulte [Versões do produto](/help/quicksilver/product-announcements/product-releases/product-releases.md).

A seguir, uma linha do tempo planejada para o lançamento da nova experiência de comentários:

* Com a versão 23.2 (6 de abril de 2023):
   * Iniciada a experiência de comentários do Beta para problemas
   * Lançamento da nova experiência de comentários para metas (como a única experiência)
* Com a versão 23.3 (20 de julho de 2023):
   * Iniciada a experiência de comentários do Beta para projetos, tarefas e documentos.
   * Lançamento da nova experiência de comentários para cartões na área Quadros (como a única experiência)
* Durante a versão do quarto trimestre de 2023 (versão limitada, disponível somente para clientes que escolhem a versão rápida):
   * Lançamento da nova experiência de comentários para modelos, tarefas de modelo, programas, portfólios, equipes, usuários e folhas de horas (como a única experiência)
   * Atualização da experiência de comentários no Beta para que projetos, tarefas, problemas e documentos se tornem a opção padrão. O rótulo &quot;Beta&quot; foi removido.
* Com a versão do quarto trimestre de 2023 (23.10) (26 de outubro de 2023)
   * Lançada a nova experiência de comentários para modelos, tarefas de modelo, programas, portfólios, equipes, usuários e folhas de horas (como a única experiência) para todos os clientes.
   * A nova experiência de comentários para projetos, tarefas, problemas e documentos tornou-se a opção padrão.

  >[!IMPORTANT]
  >
  >    Isso encerrou o estágio Beta da nova experiência de comentários.

   * Todos os recursos lançados para a nova experiência de comentários começando com essa data fizeram parte das versões mensais e trimestrais atuais.
* Final de 2023:
   * Manteve a experiência de comentários herdada como uma opção secundária para os seguintes objetos: projetos, tarefas, problemas e documentos. A nova experiência de comentários é a opção padrão para todos os usuários desses objetos.
   * A nova experiência de comentários foi a única experiência para todos os outros objetos.

* Com a segunda versão do trimestre de 2024 (11 de abril de 2024):

  Remoção da opção de alternar de volta para o fluxo de comentários herdado e tornar o novo fluxo de comentários a única experiência para todos os objetos.

* 3 de outubro de 2024:

  Remoção do botão Deixar feedback na área Atualizações.

## Localizar a nova experiência de comentários

A nova experiência de comentários está disponível nas seguintes áreas do Workfront:

* Na seção Atualizações de todos os objetos.

  Para obter informações sobre como acessar a seção Atualizações de objetos do Workfront, consulte [Visão geral da seção Atualizações](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

* No painel Resumo de tarefas, problemas e documentos em todas as áreas em que isso está disponível (listas, folhas de horas, Balanceador de carga de trabalho e Página inicial).
* Na área da Página inicial para tarefas e problemas.



<!--

The new commenting experience is currently available for all customers and for all environments.

Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:

* Both the new and legacy commenting experience for the following objects: 

    * Project
    * Task (this includes Stories)
    * Issue
    * Document

      >[!NOTE]
      >
      ><span class="preview">The legacy commenting experience has been removed from the Preview environment since April 1, 2024. </span>

* Only the new commenting experience for the objects listed below. There is no option to enable the legacy commenting experience for these objects:   

    * Goal

    >[!NOTE]
    >
    >You must have an additional license to Adobe Workfront Goals to be able to access this area of Workfront. For more information, see [Requirements to use Workfront Goals](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
  * Card on a board
  * Team
  * Template
  * Template Task
  * Timesheet
  * Program
  * Portfolio
  * User

* Only the legacy commenting experience for the following objects:

  * Iterations
    
    There is no option to enable the new commenting experience for iterations. Only the legacy commenting experience is available for iterations. 

-->


<!--before August 17: 

The new commenting experience is currently supported for the following objects:


* When enabling the Beta experience in the Updates section for 

    * Issues, projects, tasks, and documents

    For more information about managing updates for Workfront objects, see [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 

* By default, as the only commenting experience for

    * Goals, cards on a board

    >[!NOTE]
    >
    >You must have an additional license to Adobe Workfront Goals to be able to access this area of Workfront. For more information, see [Requirements to use Workfront Goals](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

-->

<!--Depending on the environment you access the commenting experience you can do one of the following: 

* Enable the commenting experience Beta in the Production environment
* <span class="preview">Enable the legacy commenting experience in the Preview  environment </span>
-->

<!--

To enable the commenting experience option for projects, tasks, issues, and documents: 

1. (Conditional) In the Production environment, go to an object that you want to activate the new commenting experience for, then click **Updates** in the left panel.
1. (Conditional) If it is disabled, enable the **New commenting** option in the upper-right corner of the Updates area to enable it. This should be enabled by default. 
<span class="preview">The New commenting option has been removed from the Preview environment.</span> 

    ![](assets/new-commenting-toggle-off-highlighted.png)

1. Start typing an update in the **Comments** tab. The Comments tab is the default tab when the new experience opens

    Or

    Click the  **System Activity** tab to view the activity updates generated by Workfront. 

1. (Optional) To disable the new commenting experience and return to legacy commenting, deselect the **New commenting** option. 

-->
