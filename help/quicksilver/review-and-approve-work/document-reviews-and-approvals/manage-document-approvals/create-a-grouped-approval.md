---
product-area: documents
navigation-topic: approvals
title: Criar uma aprovação agrupada
description: É possível agrupar vários documentos em um único fluxo de trabalho de aprovação para que eles se movam pelos mesmos estágios juntos.
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: 31bba5df6f491bfd048c1005ecd5330d3321e748
workflow-type: tm+mt
source-wordcount: '1173'
ht-degree: 3%
---

# Criar uma aprovação agrupada

<span class="preview">As informações desta página não estão disponíveis no ambiente de Pré-visualização da Sandbox porque a integração Frame.io não está disponível lá. Essa funcionalidade estará disponível em ambientes de Produção em 14 e 15 de outubro de 2026.</span>

Uma aprovação agrupada agrupa vários documentos em um único fluxo de trabalho de aprovação. Você pode usar o modo Básico e Avançado, vários estágios e caminhos paralelos com aprovações agrupadas, da mesma forma que com aprovações de documento único.

Aprovações agrupadas estão disponíveis somente na nova área Documentos, que aparece quando sua organização usa o armazenamento em nuvem da Adobe. Para obter mais informações, consulte [visão geral do armazenamento na nuvem do Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">Pacote do Adobe Workfront</td>
   <td> <p>Qualquer pacote de fluxo de trabalho para gerenciar aprovações usando o Adobe Cloud Storage</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Licença do Adobe Workfront</td>
   <td>
   <p>Colaborador ou posterior</p>
   <p>Revisar ou superior</p>
   <p>Para objetos que usam o armazenamento na nuvem do Adobe, é necessário ter uma licença Standard para criar workflows de aprovação.</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">Configurações de nível de acesso</td>
   <td> <p>Visualize ou tenha acesso superior a projetos, tarefas, problemas, modelos, portfólios, programas, relatórios, painéis, calendários e documentos</p></td>
  </tr>
  <tr>
   <td role="rowheader">Permissões de objeto</td>
   <td> <p>Gerenciar acesso ao objeto associado à solicitação ou aprovação</p></td>
  </tr>
 </tbody>
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar uma aprovação agrupada básica

Para criar uma aprovação agrupada de estágio único:

1. Vá para o projeto, tarefa ou problema que contém os documentos e selecione **Documentos** no painel esquerdo.

1. Clique no primeiro documento que deseja incluir e pressione Shift e clique nos documentos adicionais para selecionar vários documentos.

1. Com os documentos selecionados, clique em **Solicitar Aprovação** no menu inferior. A caixa de diálogo **Solicitar aprovação** é aberta no modo Básico.

   ![criar uma aprovação agrupada](assets/requeset-grouped-approval.png)

1. Preencha os seguintes detalhes:

   <table>
   <tr>
   <td><strong>Usar um modelo de aprovação (opcional)</strong></td>
   <td>O campo templates é recolhido por padrão. Clique no campo para expandi-lo e selecione um template no menu suspenso. Se o modelo tiver um caminho e um estágio, ele se aplica no modo Básico. Se o modelo tiver mais de um estágio ou mais de um caminho, a caixa de diálogo alternará automaticamente para o modo Avançado e qualquer entrada inserida no modo Básico será substituída pelo conteúdo do modelo.</td>
   </tr>
   <tr>
   <td><strong>Adicionar pessoas ou equipes na visualização</strong></td>
   <td><p>Comece digitando um nome de usuário, equipe ou endereço de email e escolha se eles são um <strong>Aprovador</strong> ou <strong>Revisor</strong>. O Workfront adiciona cada membro ativo de uma equipe individualmente.</p>
   <p>Observação: se um usuário já tiver sido adicionado ou pertencer a mais de uma equipe adicionada, ele será incluído uma vez.</p></td>
   </tr>
   <tr>
   <td><strong>É necessária apenas uma decisão (opcional)</strong></td>
   <td>A primeira pessoa que toma uma decisão completa a etapa.</td>
   </tr>
   <tr>
   <td><strong>Vencimento em (opcional)</strong></td>
   <td>Defina uma data de vencimento para a aprovação. Os usuários são notificados por e-mail 72 horas e, em seguida, 24 horas antes da data de vencimento especificada.</td>
   </tr>
   <tr>
   <td><strong>Adicionar mensagem personalizada (opcional)</strong></td>
   <td>Digite uma mensagem na caixa de texto <strong>Adicionar mensagem personalizada</strong>. A mensagem aparece na notificação por email de aprovação e na guia Approvals no Workfront.</td>
   </tr>
   </table>

1. (Opcional) Clique na guia **Documentos** para revisar os documentos incluídos nesta aprovação.

1. Clique em **Solicitar aprovação**.

   ![aprovação básica agrupada](assets/basic-group-approval.png)

## Criar uma aprovação agrupada avançada

O modo avançado suporta caminhos paralelos. Cada caminho é executado independentemente e contém um ou mais estágios sequenciais. Quando todas as decisões necessárias em um estágio são tomadas, o próximo estágio nesse caminho começa, o estágio anterior é bloqueado e os revisores e aprovadores do novo estágio recebem uma notificação por email.

Uma decisão &quot;Precisa de trabalho&quot; interrompe o caminho em que está, mas não afeta o fluxo de trabalho de aprovação em outros caminhos.

<!--
You can configure up to 30 paths and 100 stages total.
-->

Para criar uma aprovação agrupada avançada:

1. Vá para o projeto, tarefa ou problema que contém os documentos e selecione **Documentos** no painel esquerdo.

1. Clique no primeiro documento que deseja incluir e pressione Shift e clique nos documentos adicionais para selecionar vários documentos.

1. Com os documentos selecionados, clique em **Solicitar Aprovação** no menu inferior.

   ![criar uma aprovação agrupada](assets/requeset-grouped-approval.png)

1. Na parte superior direita da caixa de diálogo **Solicitar aprovação**, clique em **Ir para avançado**. Qualquer entrada inserida no modo Básico é preservada e aplicada ao **Caminho 1**, **Estágio 1**.

   >[!TIP]
   >
   >Ao criar a aprovação, você pode retornar ao modo Básico clicando em **Ir para básico** no canto superior direito. Depois de enviar a solicitação de aprovação, a opção **Ir para básico** não estará mais disponível.

1. Preencha os detalhes para o Estágio 1 do Caminho 1:

   <table>
   <tr>
   <td><strong>Nome do estágio</strong></td>
   <td>Os estágios são nomeados como <em>Estágio 1</em>, <em>Estágio 2</em> e assim por diante por padrão. Renomeie o estágio para algo mais descritivo, como <em>Revisão inicial</em> ou <em>Aprovação final</em>.</td>
   </tr>
   <tr>
   <td><strong>Adicionar pessoas ou equipes na visualização</strong></td>
   <td><p>Comece digitando um nome de usuário, equipe ou endereço de email e escolha se eles são um <strong>Aprovador</strong> ou <strong>Revisor</strong>. O Workfront adiciona cada membro ativo de uma equipe individualmente.</p>
   <p>Observação: se um usuário já tiver sido adicionado ou pertencer a mais de uma equipe adicionada, ele será incluído uma vez.</p></td>
   </tr>
   <tr>
   <td><strong>É necessária apenas uma decisão (opcional)</strong></td>
   <td>A primeira pessoa que toma uma decisão completa a etapa.</td>
   </tr>
   <tr>
   <td><strong>Vencimento em (opcional)</strong></td>
   <td>O primeiro estágio de cada caminho suporta uma data de vencimento absoluta. Cada estágio subsequente no caminho suporta uma data de vencimento relativa (o número de dias a partir de quando esse estágio abre). Os usuários são notificados por e-mail 72 horas e, em seguida, 24 horas antes da data de vencimento.</td>
   </tr>
   <tr>
   <td><strong>Adicionar mensagem personalizada (opcional)</strong></td>
   <td>Digite uma mensagem na caixa de texto <strong>Adicionar mensagem personalizada</strong>. A mensagem aparece na notificação por email de aprovação e na guia Approvals no Workfront.<p>Ao adicionar um segundo estágio, <strong>Mostrar esta mensagem em todos os estágios</strong> é selecionado por padrão. Deixe-a selecionada para usar a mesma mensagem em cada estágio. Para usar uma mensagem diferente para cada estágio, desmarque <strong>Mostrar esta mensagem em todos os estágios</strong> e digite a mensagem específica do estágio na caixa de texto <strong>Adicionar Mensagem Personalizada</strong> de cada estágio.</p></td>
   </tr>
   </table>

1. (Opcional) Adicione outros estágios ao Caminho 1:
   1. Clique em **Adicionar estágio** para adicionar outro estágio ao caminho atual. Os estágios em um caminho são executados sequencialmente na ordem em que estão listados.
   1. Preencha os detalhes do novo estágio e repita essa etapa para adicionar mais estágios, conforme necessário.

      >[!NOTE]
      >
      >É possível reordenar os estágios em um caminho, mas não é possível mover um estágio de um caminho para outro. Cada caminho pode ter um número diferente de estágios.


1. (Opcional) Adicione um caminho paralelo:
   1. Em **Caminhos paralelos** no lado esquerdo da tela, clique em **Adicionar caminho** para adicionar outro caminho.
   1. Siga as mesmas etapas para adicionar estágios e participantes ao novo caminho. Cada caminho é executado independentemente para que você possa ter números diferentes de estágios e participantes diferentes em cada caminho.

1. (Opcional) Para remover um caminho, passe o mouse sobre o rótulo do caminho e clique no ícone de lixeira. **O Caminho 1** não pode ser removido e os caminhos não podem ser reordenados. Outros caminhos podem ser removidos somente se nenhum estágio no caminho estiver bloqueado ou concluído.

1. (Opcional) Para limpar todos os caminhos e estágios e começar novamente, clique em **Redefinir** no canto superior direito.

1. (Opcional) Clique na guia **Documentos** para revisar os documentos incluídos nesta aprovação.

1. Clique em **Solicitar aprovação**.

   ![aprovação agrupada avançada](assets/advanced-group-approval.png)


<!--

## Add additional documents to a grouped approval

You can add additional documents to a grouped approval after the approval has been created as long as the first stage has not been completed. 

To add an additional document to a grouped approval:

1. Click any document in the grouped approval, then click **Manage Approval** in the bottom menu.
1. Click **Documents on this approval**, then click **Add**.

   ![add document grouped approval](assets/add-document-to-grouped-approval.png)
1. Choose the documents you want to add, then click **Add to approval**. 
1. Once you add all of the documents, click **Edit approval**. The new documents are added to the grouped approval and all participants are notified of the change.

-->

## Limitações conhecidas

* Atualmente, não é possível adicionar ou remover documentos de um fluxo de trabalho de aprovação agrupado depois de criado. Essa funcionalidade está planejada para uma versão futura.
* As aprovações agrupadas estão temporariamente limitadas a 3 caminhos e 25 documentos por grupo.