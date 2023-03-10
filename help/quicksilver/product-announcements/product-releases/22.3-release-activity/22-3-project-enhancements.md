---
title: atualizações do projeto durante o período de lançamento da versão 2.3
description: atualizações do projeto durante o período de lançamento da versão 2.3
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 1235ad4a-72dd-45c5-8513-d073b3e9a2da
source-git-commit: 0fea13b0a1d8f14c2d601e0ed0a8d15684a3c4d7
workflow-type: tm+mt
source-wordcount: '1549'
ht-degree: 0%

---

# 2.3 Aprimoramentos do projeto

Esta página descreve todas as melhorias do projeto feitas com a versão 2.3 para o ambiente de visualização. Esses aprimoramentos foram disponibilizados no ambiente de Produção na semana de 11 de julho de 2022. Para obter uma lista de todas as alterações disponíveis com a versão 22.3, consulte [Visão geral da versão 2.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Delegação de atividades fora do escritório

Agora, você pode delegar temporariamente as tarefas e os problemas atribuídos a você a outros usuários quando planeja estar fora do escritório por um breve período de tempo. Isso garante que sua ausência não se torne um obstáculo para o trabalho que está sendo concluído.

Antes desse aprimoramento, você só podia delegar aprovações.

Estes são alguns dos recursos que adicionamos com esta atualização:

* Uma configuração na área Preferências de tarefas e problemas da Configuração do Administrador do sistema ou do Grupo para habilitar a delegação no seu ambiente.

* Uma nova opção para &quot;Delegar tarefas e problemas&quot; na área inicial para usuários com uma licença Revisar ou superior para delegar seus itens de trabalho.

* Indicar na Página Inicial e na área Atribuições de tarefas e emitir cabeçalhos que os itens são delegados a outros.

* Notificações de eventos na área Configuração e notificações por email no perfil do usuário para controlar notificações por email sobre trabalho delegado


>[!NOTE]
>
>Somente usuários com uma licença Revisar ou superior podem delegar seu trabalho a outros. O trabalho pode ser delegado a qualquer usuário, independentemente de seu nível de acesso. Os usuários delegados recebem as mesmas permissões que os destinatários nos itens delegados. Se essas permissões forem inferiores à configuração de nível de acesso de um usuário, os usuários delegados poderão ser impedidos de executar algumas das atividades nas tarefas e problemas que são delegados a eles.


Para obter mais informações, consulte [Delegar tarefa e visão geral do problema](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md).

## Nova experiência ao converter um problema em uma tarefa

Para tornar seu uso do Workfront consistente com a nova experiência do Workfront, reprojetamos a interface para converter um problema em uma tarefa.

Esta atualização inclui:

* Uma interface do usuário atualizada que corresponde ao restante da nova experiência do Workfront.

* Acesso para converter um problema em tarefas de uma lista ou relatório.

* Os formulários personalizados padrão definidos na área Configurações de tarefas do projeto de destino foram adicionados à nova tarefa.


Para obter mais informações, consulte [Converter um problema em uma tarefa no Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-task.md).

## Nova experiência ao converter um problema em um projeto sem um modelo

Para tornar seu uso do Workfront consistente com a nova experiência do Workfront, reprojetamos a interface para converter um problema em um projeto sem usar um modelo.

Além de uma interface do usuário atualizada que corresponde ao resto da nova experiência do Workfront, também adicionamos a capacidade de converter um problema em projetos em branco a partir de uma lista ou relatório.

Para obter mais informações, consulte [Converter um problema em um projeto no Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-project.md).

## Marcação inteligente no fluxo de atualização

Melhoramos a marcação de usuários no fluxo de atualização ao criar uma nova atualização ou responder a uma existente. Agora, ao marcar um usuário para incluí-lo em uma atualização, além do nome e avatar, também exibimos a Função primária e o email. Isso ajuda a distinguir entre vários usuários com nomes semelhantes ou idênticos.

Para obter mais informações, consulte [Marcar outras pessoas em atualizações](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Nova sintaxe para cálculos em campos personalizados

Para nos prepararmos para aprimoramentos futuros que ajudarão você a adicionar cálculos a formulários personalizados, padronizamos a sintaxe dos campos referenciados adicionados a um cálculo. É fácil usar essa nova sintaxe porque o sistema a insere para você ao digitar o nome de um campo e depois selecioná-lo.

Para obter mais informações, consulte a seção &quot;Criar o cálculo para seu campo personalizado calculado&quot; na [artigo Adicionar dados calculados a um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Manter informações precisas quando dois usuários com uma função comum estiverem envolvidos em um processo de aprovação

Para garantir a precisão de seus dados para aprovação do trabalho, fizemos uma alteração na maneira como as informações de aprovação são registradas em um item quando um processo de aprovação de várias funções está associado ao item.

Alguns processos de aprovação exigem aprovação de duas funções diferentes, e dois aprovadores diferentes podem ter uma dessas funções em comum. Agora, quando isso acontece, depois que as decisões de aprovação são tomadas, o Workfront registra cada aprovador e sua respectiva função associada ao processo de aprovação.

Antes dessa alteração, ambas as aprovações eram registradas para o segundo usuário porque compartilhavam uma das funções de aprovação com o primeiro aprovador. Nesse caso, o segundo aprovador foi substituir as informações do primeiro aprovador.

Para obter mais informações sobre processos de aprovação no Workfront, consulte [Visão geral do processo de aprovação](/help/quicksilver/review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

## As horas de alocação não serão mais removidas ao fazer alterações em atribuições

>[!NOTE]
>
>Esse recurso foi originalmente planejado para ser lançado com a versão 2.2. Ele foi lançado para produção em 21 de abril de 2022.


Para garantir a precisão dos seus dados, fizemos uma alteração para preservar as horas de alocação e manter as Horas Planejadas da tarefa inalteradas ao fazer alterações nas atribuições na tarefa.

As seguintes alterações foram feitas em tarefas com um Tipo de duração simples:

* As Horas Planejadas são preservadas ao remover todos os destinatários.

* As alocações de atribuição individuais são preservadas ao substituir usuários e funções.

* As alocações de atribuição individuais são preservadas na função ao remover o usuário. (Removido da versão. Agora, as Horas Planejadas serão definidas como 0 após remover todos os destinatários.)


Para obter mais informações sobre Horas Planejadas, consulte [Visão geral das Horas Planejadas](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).

## Melhorias nas placas

Os seguintes aprimoramentos foram adicionados às placas Adobe Workfront:

* Opções de filtro - Agora é possível filtrar por data de vencimento ou status em um quadro. O filtro também foi atualizado com seções que podem ser recolhidas para separar as opções.

* Quadro de arquivamento - agora é possível arquivar um quadro enquanto você está no quadro, em vez de precisar ir para o painel de quadros.

* Adicionar uma equipe a um quadro - ao procurar membros, você pode adicionar uma equipe inteira. Escolher uma equipe adiciona todos da equipe ao quadro.

* Solte as zonas em colunas - ao arrastar e soltar um cartão de uma coluna de quadro para outra, uma &quot;zona de soltar&quot; cinza agora mostra onde o cartão será colocado. Anteriormente, não havia um indicador visual da posição do cartão.

* Cartões conectados - Agora é possível adicionar cartões conectados a tarefas e problemas da Workfront. Atualizar o nome, a descrição ou o destinatário no cartão ou na tarefa atualizará os mesmos campos no outro local.

* Campo Status em todos os cartões - Um campo Status e um botão Marcar como concluído foram adicionados aos cartões ad hoc e conectados. Ao clicar em Marcar como concluído, o status é automaticamente alterado para Concluído.

* Converter cartão ad hoc em cartão conectado - agora você tem a opção de converter um cartão ad hoc em um cartão conectado a partir dos detalhes do cartão.

* Desconectar placa conectada - Desconectar uma placa conectada interrompe a conexão com o objeto Workfront. O cartão permanece como um cartão ad hoc no quadro e o objeto Workfront não é afetado.

* Mapeamento de status em colunas - As novas configurações e políticas de coluna permitem definir um status, destinatário ou tag aplicada aos cartões movidos para essa coluna. Além disso, os nomes de coluna padrão em um novo quadro foram alterados para Coluna 1, Coluna 2 e Coluna 3.

* Indicador de atualização de campo - Um indicador agora é exibido quando você salva um cartão, para confirmar que suas atualizações foram salvas.


Para obter mais informações, consulte [Introdução a quadros no Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/get-started-with-boards.md).

## Compartilhar pastas somente nos cinco principais níveis de uma hierarquia de pastas

Para garantir o melhor desempenho para os usuários que compartilham pastas, atualmente limitamos o compartilhamento para os cinco principais níveis em uma hierarquia de pastas em um objeto.

Cada pasta no sexto nível ou abaixo herda suas configurações de compartilhamento da pasta diretamente acima dela.

Para obter mais informações sobre compartilhamento de pastas, consulte [Compartilhar uma pasta de documentos de nível superior](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Campanhas do Workfront (Beta) - uma nova maneira de gerenciar seu trabalho

>[!NOTE]
>
>Esse recurso está planejado para ser removido da Visualização em 9 de janeiro de 2023. Para obter mais informações, consulte o [Página de visão geral da versão 23.1](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

>[!NOTE]
>
>Esse recurso não será incluído na versão de produção 22.3. Ele será lançado para produção com uma versão futura.


>[!NOTE]
>
>Essa funcionalidade está disponível somente como um beta e está em construção no momento. Continuaremos a adicionar recursos para o fluxo de trabalho do Campaign com versões futuras. A participação no programa beta para Campanhas Workfront é voluntária.

Estamos introduzindo um novo objeto no Adobe Workfront que tem o potencial de mudar a maneira como você gerencia o trabalho.

As Campanhas do Workfront permitem organizar projetos de diferentes portfólios e programas em um novo contêiner de trabalho. Esse novo contêiner evoluirá em versões futuras para eventualmente incluir todos os objetos de trabalho que estão gerenciados no momento em silos separados.

Os seguintes recursos estão incluídos nesta versão:

* Um novo objeto do Workfront chamado Campaign

* Uma nova área Campanhas (Beta) no Menu principal

* Uma lista de campanhas na área Campanhas

* Uma página Detalhes da campanha que exibe informações adicionais sobre uma campanha

* Capacidade de adicionar projetos a uma campanha

* Capacidade de editar informações sobre uma campanha

* Capacidade de renomear o objeto da campanha a partir do modelo de layout

   Os administradores de sistema e de grupo do Workfront podem adicionar a área Campanhas (Beta) no Menu principal de um modelo de layout. Isso o disponibiliza para todos os usuários atribuídos ao modelo. Depois que estiver disponível, qualquer pessoa no Workfront poderá criar uma campanha.




