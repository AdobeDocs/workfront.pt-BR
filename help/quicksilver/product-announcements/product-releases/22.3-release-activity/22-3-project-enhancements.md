---
title: atualizações de projeto durante o período da versão 22.3
description: atualizações de projeto durante o período da versão 22.3
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1235ad4a-72dd-45c5-8513-d073b3e9a2da
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1562'
ht-degree: 0%

---

# 22.3 Aprimoramentos do projeto

Esta página descreve todas as melhorias feitas no Project com a versão 22.3 para o ambiente de Pré-visualização. Essas melhorias foram disponibilizadas no ambiente de Produção na semana de 11 de julho de 2022. Para obter uma lista de todas as alterações disponíveis com a versão 22.3, consulte a [Visão geral da versão 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Delegação de trabalho fora do escritório

Agora, você pode delegar temporariamente as tarefas e problemas atribuídos a você a outros usuários quando planeja ficar fora do escritório por um breve período. Isso garante que sua ausência não se torne um obstáculo para a conclusão do trabalho.

Antes dessa melhoria, você só poderia delegar aprovações.

Veja a seguir alguns dos recursos que adicionamos com essa atualização:

* Uma configuração na área Preferências de tarefas e problemas da Configuração para o administrador de sistema ou grupo habilitar a delegação no seu ambiente.

* Uma nova opção para &quot;Delegar tarefas e problemas&quot; na área da Página inicial para usuários com uma licença de Revisão ou superior delegarem seus itens de trabalho.

* Indicação na Página inicial e na área Atribuições dos cabeçalhos de tarefas e ocorrências de que os itens são delegados a outras pessoas.

* Notificações de eventos na área Configuração e notificações por email no perfil do usuário para controlar notificações por email sobre trabalho delegado


>[!NOTE]
>
>Somente usuários com uma licença de Revisão ou superior podem delegar seu trabalho a outras pessoas. O trabalho pode ser delegado a qualquer usuário, independentemente do nível de acesso. Os usuários delegados recebem as mesmas permissões que os atribuídos nos itens delegados. Se essas permissões forem menores que a configuração do nível de acesso de um usuário, os usuários delegados poderão ser impedidos de executar algumas atividades nas tarefas e problemas que são delegados a eles.


Para obter mais informações, consulte [Visão geral da tarefa de delegação e do problema](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md).

## Nova experiência ao converter um problema em uma tarefa

Para tornar seu uso do Workfront consistente com a nova experiência do Workfront, reprojetamos a interface para converter um problema em uma tarefa.

Esta atualização inclui:

* Uma interface atualizada que corresponde ao restante da nova experiência do Workfront.

* Acesso para converter um problema em tarefas de uma lista ou de um relatório.

* Os formulários personalizados padrão definidos na área Configurações de tarefas do projeto de destino foram adicionados à nova tarefa.


Para obter mais informações, consulte [Converter um problema em uma tarefa no Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-task.md).

## Nova experiência ao converter um problema em um projeto sem um modelo

Para tornar seu uso do Workfront consistente com a nova experiência do Workfront, reprojetamos a interface para converter um problema em um projeto sem usar um modelo.

Além de uma interface atualizada que corresponde ao restante da nova experiência do Workfront, também adicionamos a capacidade de converter um problema em projetos em branco de uma lista ou de um relatório.

Para obter mais informações, consulte [Converter um problema em um projeto no Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-project.md).

## Marcação inteligente no fluxo de atualização

Melhoramos ao marcar usuários no fluxo de atualização ao criar uma nova atualização ou responder a uma existente. Agora, ao marcar um usuário para incluí-lo em uma atualização, além do nome e avatar, também exibimos a função principal e o email. Isso ajuda a distinguir entre vários usuários com nomes semelhantes ou idênticos.

Para obter mais informações, consulte [Marcar outros em atualizações](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Nova sintaxe para cálculos em campos personalizados

Para se preparar para aprimoramentos futuros que ajudarão você a adicionar cálculos a formulários personalizados, padronizamos a sintaxe dos campos referenciados que você adiciona a um cálculo. É fácil usar essa nova sintaxe porque o sistema a insere quando você começa a digitar o nome de um campo e o seleciona.

Para obter mais informações, consulte a seção &quot;Criar o cálculo para o campo personalizado calculado&quot; no [artigo Adicionar dados calculados a um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Manter informações precisas quando dois usuários com uma função em comum estiverem envolvidos em um processo de aprovação

Para garantir a precisão de seus dados para aprovação de trabalho, fizemos uma alteração na maneira como as informações de aprovação são registradas em um item quando um processo de aprovação de várias funções está associado ao item.

Alguns processos de aprovação exigem aprovação de duas funções diferentes, e dois aprovadores diferentes podem ter uma dessas funções em comum. Agora, quando isso acontece, depois que as decisões de aprovação são tomadas, o Workfront registra cada aprovador e sua respectiva função associada ao processo de aprovação.

Antes dessa alteração, ambas as aprovações eram registradas para o segundo usuário porque elas compartilhavam uma das funções de aprovação com o primeiro aprovador. Nesse caso, o segundo aprovador estava substituindo as informações do primeiro aprovador.

Para obter mais informações sobre processos de aprovação no Workfront, consulte [Visão geral do processo de aprovação](/help/quicksilver/review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

## As horas de alocação não serão mais removidas quando forem feitas alterações nas atribuições

>[!NOTE]
>
>Este recurso foi originalmente planejado para ser lançado com a versão 22.2. Foi lançado para produção em 21 de abril de 2022.


Para garantir a precisão de seus dados, fizemos uma alteração para preservar as horas de alocação e manter as Horas planejadas da tarefa inalteradas ao fazer alterações em atribuições na tarefa.

As seguintes alterações foram feitas em tarefas com um Tipo de Duração Simples:

* As horas planejadas são preservadas ao remover todos os atribuídos.

* As alocações de atribuição individuais são preservadas ao substituir usuários e funções.

* As alocações de atribuição individuais são preservadas na função ao remover o usuário. (Removido da versão. Agora, as Horas planejadas serão definidas como 0 após remover todos os atribuídos.)


Para obter mais informações sobre as Horas Planejadas, consulte [visão geral das Horas Planejadas](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).

## Melhorias nas placas

As seguintes melhorias foram adicionadas às placas Adobe Workfront:

* Opções de filtro - Agora é possível filtrar por data de vencimento ou status em um quadro. O filtro também foi atualizado com seções que podem ser recolhidas para separar as opções.

* Arquivar quadro - Agora é possível arquivar um quadro enquanto estiver no quadro, em vez de precisar ir para o painel de quadros.

* Adicionar uma equipe a um quadro - Ao pesquisar membros, é possível adicionar uma equipe inteira. Escolher uma equipe adiciona todos na equipe ao quadro.

* Zonas de soltar em colunas - Ao arrastar e soltar um cartão de uma coluna do quadro para outra, uma &quot;zona de soltar&quot; cinza agora mostra onde o cartão será colocado. Anteriormente, não havia um indicador visual da inserção do cartão.

* Cartões conectados - Agora é possível adicionar cartões conectados a tarefas e problemas do Workfront. Atualizar o nome, a descrição ou o destinatário no cartão ou na tarefa atualizará os mesmos campos no outro local.

* Campo de status em todos os cartões - Um campo Status e um botão Marcar como concluído foram adicionados aos cartões ad hoc e conectados. Quando você clica em Marcar como concluído, o status muda automaticamente para Concluído.

* Converter cartão ad hoc em cartão conectado - Agora há a opção de converter um cartão ad hoc em um cartão conectado dos detalhes do cartão.

* Desconectar placa conectada - A desconexão de uma placa conectada interrompe a conexão com o objeto do Workfront. O cartão permanece como um cartão ad hoc no quadro e o objeto Workfront não é afetado.

* Mapeamento de status em colunas - Novas configurações e políticas de coluna permitem definir um status, destinatário ou tag aplicada aos cartões movidos para essa coluna. Além disso, os nomes de coluna padrão em um novo quadro foram alterados para Coluna 1, Coluna 2 e Coluna 3.

* Indicador de atualização de campo - Um indicador agora é exibido ao salvar um cartão, para confirmar que as atualizações foram salvas.


Para obter mais informações, consulte [Introdução aos painéis no Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/get-started-with-boards.md).

## Compartilhar pastas somente nos cinco níveis superiores de uma hierarquia de pastas

Para garantir o melhor desempenho para usuários que compartilham pastas, estamos limitando o compartilhamento aos cinco principais níveis em uma hierarquia de pastas em um objeto.

Cada pasta no sexto nível ou abaixo herda suas configurações de compartilhamento da pasta diretamente acima dela.

Para obter mais informações sobre pastas de compartilhamento, consulte [Compartilhar uma pasta de documentos de nível superior](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Campanhas do Workfront (Beta) - uma nova maneira de gerenciar seu trabalho

>[!NOTE]
>
>A remoção desse recurso da visualização está planejada para 9 de janeiro de 2023. Para obter mais informações, consulte a [página de visão geral da versão](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md) do 23.1.

>[!NOTE]
>
>Esse recurso não será incluído na versão de produção 22.3. Ele será lançado para produção com uma versão futura.


>[!NOTE]
>
>Essa funcionalidade está disponível somente como um beta e está atualmente em construção. Continuaremos a adicionar recursos para o fluxo de trabalho do Campaign com versões futuras. A participação no programa beta para campanhas do Workfront é voluntária.

Estamos introduzindo um novo objeto no Adobe Workfront que tem o potencial de mudar a maneira como você gerencia o trabalho.

O Workfront Campaigns permite organizar projetos de diferentes portfólios e programas em um novo container de trabalho. Esse novo contêiner evoluirá em versões futuras para eventualmente incluir todos os objetos de trabalho que são gerenciados atualmente em silos separados.

Os seguintes recursos estão incluídos nesta versão:

* Um novo objeto do Workfront chamado Campanha

* Uma nova área Campanhas (Beta) no menu principal

* Uma lista de Campanhas na área Campanhas

* Uma página de Detalhes da campanha que exibe informações adicionais sobre uma campanha

* Capacidade de adicionar projetos a uma campanha

* Capacidade de editar informações sobre uma campanha

* Capacidade de renomear o objeto Campaign a partir do Modelo de layout

  Os administradores de sistema e de grupo do Workfront podem adicionar a área Campanhas (Beta) no menu principal de um modelo de layout. Isso o torna disponível para todos os usuários atribuídos ao modelo. Depois que estiver disponível, qualquer pessoa no Workfront poderá criar uma campanha.




