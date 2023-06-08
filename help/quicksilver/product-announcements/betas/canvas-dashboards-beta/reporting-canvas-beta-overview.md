---
content-type: reference
navigation-topic: betas
title: "Tela de relatório beta: visão geral"
description: Informações sobre o programa beta da próxima ferramenta de tela de relatório do Adobe Workfront
author: Nolan
feature: Product Announcements
hidefromtoc: true
exl-id: cc0adf28-08ab-4330-b901-219ab687f02f
source-git-commit: 1536d7425b5c5d3c676ff0c8c6a2a9531690ac3e
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 1%

---


# Versão beta do relatório do Canvas: visão geral

## Tela de relatório

Uma recriação completa dos relatórios no Workfront, a nova ferramenta Tela de relatório está sendo desenvolvida no momento. Ao projetar a Tela de relatórios, trabalhamos arduamente para fornecer uma experiência que ofereça flexibilidade máxima combinada com um design intuitivo e modular, para que usuários como você possam aproveitar seus próprios dados na criação e no compartilhamento de relatórios com mais eficiência. Por meio de um novo tipo de relatório unificado que permite arrastar e soltar quase todos os elementos em uma tela ilimitada, criar uma obra-prima de dados visuais logo será mais fácil do que nunca.

Este artigo contém informações sobre o beta privado atual, que se limita a clientes específicos. Os novos recursos da Tela de relatório agora estão sendo implantados por meio dos Painéis da Tela de relatório. Consulte **Plano de desenvolvimento** abaixo para obter mais informações.

### Plano de desenvolvimento

Estamos nos estágios finais de resolução de um problema de qualidade de dados que observamos no início da versão beta da Tela de relatório. Em breve, retomaremos o trabalho para fornecer novas visualizações, expandir a seleção de objetos reportáveis do Workfront e melhorar as experiências de criação e distribuição de relatórios, que são fundamentais para a realização de nossas metas da Tela de relatórios.

Forneceremos essas novas experiências de forma incremental, começando com a versão 23.2, por meio da nova página Painéis da tela, que agora está disponível em seu ambiente de Pré-visualização. Os Painéis do Canvas permitem exibir relatórios existentes junto com os novos recursos de relatórios que estamos criando, e servirão como nosso ambiente principal para implantar e testar novos recursos do Canvas de relatórios. Para obter mais informações sobre como ativar e usar Painéis do Canvas, consulte [Visão geral dos Painéis do Canvas](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/canvas-dashboards-overview.md).

## Participe da versão beta

>[!IMPORTANT]
>
>As informações beta abaixo são para administradores que já foram incluídos na versão beta da Tela de relatório, que não está mais aceitando novos participantes. Se você quiser testar novos recursos da Tela de relatório à medida que forem adicionados, consulte **Plano de desenvolvimento** acima para obter informações sobre como ativar o Canvas Dashboards.

### Disponibilidade

A versão beta da Tela de relatório está disponível para todas as organizações que estão na AWS, independentemente da região.

### Associar-se ao beta

A versão beta da Tela de relatório é totalmente opcional, mas só pode ser aceita por um administrador do Workfront. Para aceitar o como Administrador do sistema:

1. Selecione o **Relatórios (beta)** no menu Principal da sua instância do Workfront.
1. Clique em **Aceitar** para aceitar os termos e condições.
1. Permitir que os dados de sua organização sejam adicionados à Tela de relatório (isso pode levar algumas horas).
1. Comece a usar a Tela de relatório.

Depois que os dados da sua organização forem adicionados à Tela de relatório, outros administradores do sistema poderão optar por ingressar individualmente da mesma maneira (sem esperar que os dados sejam adicionados novamente).

Para aceitar outros usuários que não sejam administradores do Workfront:

1. Selecione o **Relatórios (beta)** no menu Principal da sua instância do Workfront.
1. Clique em **Permissões da Tela de relatório**.
1. Procure e selecione os usuários específicos dos quais deseja participar.

   >[!IMPORTANT]
   >
   >Os usuários aos quais você conceder acesso à Tela de relatório terão acesso **all** dados no sistema na capacidade de somente leitura, independentemente das permissões padrão para visualizar esses dados.

1. Clique em **Salvar**.
1. Adicione o **Relatórios (beta)** no modelo de layout principal de cada usuário selecionado. Para obter mais informações, consulte [Personalizar o menu principal usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).
1. Cada usuário deve então navegar individualmente para o **Relatórios (beta)** no menu principal e aceite os termos e condições.

### Enviar feedback

Para enviar feedback sobre o beta:

1. Na Tela de relatório no Workfront, clique na guia **Enviar feedback** botão.
1. Preencha o formulário e clique em **Enviar**.

## Perguntas frequentes sobre Beta

+++Posso migrar meus relatórios herdados para a Tela de relatórios?

Resumindo, a migração de relatórios herdados não estará disponível durante a versão beta. No entanto, é um recurso planejado (com algumas limitações descritas abaixo) para o lançamento oficial.

Embora a barreira para criar novos relatórios tenha sido significativamente reduzida com a Tela de relatório, entendemos que trazer alguns de seus relatórios e painéis existentes ajudará a acelerar o processo de adoção. Dessa forma, queremos fornecer as ferramentas e os recursos necessários para garantir que você possa trazer quaisquer itens herdados relevantes para garantir que inicie com o pé direito na Tela de relatório. Como a Tela de relatório é uma mudança tão radical no modo como os relatórios atuais funcionam, no entanto, seria impossível migrar cada relatório ou painel exatamente como é hoje.

Nossa estratégia atual de migração na versão oficial é permitir que você faça o seguinte:

1. Identificar os relatórios e painéis de controle relevantes

   1. Permitem exportar um CSV de todos os relatórios e painéis do sistema juntamente com quaisquer informações de rastreamento relevantes (número de visualizações, quando e por quem).
   1. Forneça uma exportação de relatórios configurados com entregas programadas junto com os recipients.

1. Selecione os relatórios e painéis de controle que você deseja migrar e clique em **Migrar**

   Esta é uma migração de mão única. Ele cria uma cópia dos relatórios e painéis selecionados para a Tela de relatório, deixando o relatório ou painel herdado intacto na ferramenta de relatório atual.

   Você pode migrar o mesmo relatório ou painel quantas vezes quiser.

1. Na Tela de relatório, verifique se todos os relatórios e painéis selecionados foram migrados.
+++

+++Por que não consigo ver todos os objetos que normalmente faço?

Para fornecer a versão beta a nossos clientes o mais rápido possível, lançamos somente um subconjunto dos vários tipos de objetos disponíveis no Workfront atualmente. Abaixo estão os tipos de objetos aceitos atualmente na versão beta:

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

+++Se algo der errado no Reporting Canvas durante o beta, os dados da minha organização serão afetados?

não. A versão beta usa uma cópia dos dados de sua organização que é preenchida na Tela de relatório. Embora isso signifique que você esteja seguro para experimentar durante o beta sem risco de afetar dados importantes, também significa que a edição em linha de dados na Tela de relatórios estará indisponível até o lançamento oficial.
+++

+++Posso recusar o beta depois de entrar?

Um administrador do Workfront não pode recusar o beta; no entanto, não administradores do sistema podem ser removidos fazendo o seguinte:

1. Efetue login como um administrador do sistema.
1. Navegue até Tela de Relatório.
1. Clique em Tela de relatório **permissões**.
1. Remova os usuários que deseja excluir da versão beta da lista de opções de participação.
1. Clique em **Salvar**.
+++
