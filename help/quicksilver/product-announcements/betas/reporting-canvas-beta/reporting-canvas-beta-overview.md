---
content-type: reference
navigation-topic: betas
title: 'Versão beta da tela de relatórios: visão geral'
description: Informações sobre o programa beta para a próxima ferramenta Tela de relatórios do Adobe Workfront
author: Nolan
feature: Product Announcements
exl-id: cc0adf28-08ab-4330-b901-219ab687f02f
source-git-commit: d738ef3f6642d5b1a646f58896575a2971bbc06a
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 1%

---


# Beta da Tela de Relatório: visão geral

## Tela de relatórios

Uma reformulação completa dos relatórios no Workfront, a nova ferramenta Tela de relatórios está em desenvolvimento no momento. Ao projetar a Tela de relatórios, trabalhamos duro para fornecer uma experiência que ofereça flexibilidade máxima, juntamente com um design intuitivo e modular, para que os usuários como você possam aproveitar seus próprios dados com mais eficiência na criação e no compartilhamento de relatórios. Por meio de um novo tipo de relatório unificado que permite arrastar e soltar quase todos os elementos em uma tela sem limites, criar uma obra-prima de dados visuais será mais fácil do que nunca.

Este artigo contém informações sobre o beta privado atual, que é limitado a clientes específicos. Os novos recursos da Tela de relatórios agora estão sendo implantados por meio dos Painéis de tela. Consulte **Plano de desenvolvimento** abaixo para obter mais informações.

### Plano de desenvolvimento

Estamos nos estágios finais para resolver um problema de qualidade de dados que observamos no início do beta da Tela de relatórios. Em breve, retomaremos o trabalho para fornecer novas visualizações, expandir a seleção de objetos Workfront reportáveis e melhorar a criação de relatórios e as experiências de distribuição, que são integrantes à realização de nossas metas para a Tela de relatórios.

Forneceremos essas novas experiências de forma incremental, a partir da versão 23.2, por meio da nova página Painéis de Tela que agora está disponível em seu ambiente de Visualização. Os Painéis de Tela permitem exibir relatórios existentes junto com os novos recursos de relatório que estamos criando e servirão como nosso ambiente principal para implantar e testar novos recursos para a Tela de relatórios. Para obter mais informações sobre como ativar e usar Painéis de Tela, consulte [Visão geral dos painéis da tela de desenho](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/canvas-dashboards-overview.md).

## Participe do beta

>[!IMPORTANT]
>
>As informações beta abaixo são para administradores que já foram incluídos no beta da Tela de relatórios, que não está mais aceitando novos participantes. Se quiser testar novos recursos da Tela de relatórios à medida que são adicionados, consulte **Plano de desenvolvimento** acima para obter informações sobre como ativar Painéis de Tela.

### Disponibilidade

O beta da Tela de relatórios está disponível para todas as organizações que estão no AWS, independentemente da região.

### Associe-se ao beta

O beta da Tela de relatórios é completamente opcional, mas só pode ser optado por um administrador do Workfront. Para aceitar como Administrador do sistema:

1. Selecione o **Relatório (beta)** no menu Main da instância do Workfront.
1. Clique em **Aceitar** para aceitar os termos e condições.
1. Permitir que os dados da organização sejam adicionados à Tela de relatórios (isso pode levar até algumas horas).
1. Comece a usar a Tela de relatórios.

Depois que os dados de sua organização forem adicionados à Tela de relatórios, outros administradores de sistema poderão optar por participar individualmente da mesma maneira (sem esperar que os dados sejam adicionados novamente).

Para aceitar outros usuários que não são administradores do Workfront:

1. Selecione o **Relatório (beta)** no menu Main da instância do Workfront.
1. Clique em **Permissões da Tela de relatórios**.
1. Procure e selecione os usuários específicos que deseja participar.

   >[!IMPORTANT]
   >
   >Os usuários aos quais você concede acesso à Tela de relatórios terão acesso **all** dados no sistema em uma capacidade somente leitura, independentemente de suas permissões padrão para exibir esses dados.

1. Clique em **Salvar**.
1. Adicione o **Relatório (beta)** no modelo de layout principal de cada usuário selecionado. Para obter mais informações, consulte [Personalizar o Menu principal usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).
1. Cada usuário deve então navegar individualmente para o **Relatório (beta)** no menu principal e aceite os termos e condições.

### Enviar feedback

Para enviar feedback sobre o beta:

1. Na Tela de relatórios do Workfront, clique no botão **Enviar feedback** botão.
1. Preencha o formulário e clique em **Enviar**.

## Perguntas frequentes sobre Beta

+++Posso migrar meus relatórios herdados para a Tela de relatórios?

Em resumo, a migração de relatórios herdados não estará disponível durante o beta. No entanto, é um recurso planejado (com algumas limitações descritas abaixo) para o lançamento oficial.

Embora a barreira para a criação de novos relatórios tenha sido significativamente reduzida com a Tela de relatórios, entendemos que trazer alguns de seus relatórios e painéis existentes ajudará a acelerar o processo de adoção. Dessa forma, queremos fornecer as ferramentas e os recursos necessários para garantir que você possa trazer quaisquer itens herdados relevantes para garantir que comece no pé direito na Tela de relatórios. Como a Tela de relatórios é uma mudança radical na maneira como o relatório atual funciona, no entanto, seria impossível migrar cada relatório ou painel exatamente como está hoje.

Nossa estratégia atual de migração nas versões oficiais permite fazer o seguinte:

1. Identificar os relatórios e painéis que são relevantes

   1. Forneça a capacidade de exportar um CSV de todos os relatórios e painéis do sistema, juntamente com quaisquer informações de rastreamento relevantes (número de visualizações, quando e por quem).
   1. Forneça uma exportação de relatórios configurados com entregas programadas junto com os recipients.

1. Selecione os relatórios e painéis que deseja migrar e clique em **Migrar**

   Essa é uma migração unidirecional. Ele cria uma cópia dos relatórios e painéis selecionados para a Tela de relatórios, deixando o relatório herdado ou o painel intacto na ferramenta de relatório atual.

   Você pode migrar o mesmo relatório ou painel quantas vezes desejar.

1. Na Tela de relatórios, verifique se todos os relatórios e painéis selecionados foram migrados.
+++

+++Por que não consigo ver todos os objetos que eu normalmente faço?

Para fornecer o beta aos clientes o mais rápido possível, lançamos com apenas um subconjunto dos vários tipos de objeto disponíveis no Workfront hoje. Abaixo estão os tipos de objeto suportados atualmente no beta:

* Atribuição
* Documento
* Aprovação de documento
* Despesa
* Hora
* Problema
* Nota
* Portfólio
* Projeto
* Programa
* Tarefa
* Planilha de horas
* Item de trabalho
+++

+++Se algo der errado na Tela de relatórios durante o beta, os dados da minha organização serão afetados?

não. O beta usa uma cópia dos dados de sua organização preenchidos na Tela de relatórios. Embora isso signifique que você é seguro fazer testes durante o beta sem correr o risco de afetar dados importantes, também significa que a edição de dados em linha na Tela de relatórios não estará disponível até o lançamento oficial.
+++

+++Posso recusar o beta depois de ingressar?

Um administrador do Workfront não pode recusar o beta; no entanto, administradores que não são do sistema podem ser removidos fazendo o seguinte:

1. Faça logon como administrador do sistema.
1. Navegue até a Tela de relatórios.
1. Clique em Tela de relatórios **permissões**.
1. Remova os usuários que deseja excluir do beta da lista que foram aceitos.
1. Clique em **Salvar**.
+++
