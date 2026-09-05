---
content-type: release-notes
title: Atividade da versão do quarto trimestre de 2026 para o Adobe Workfront Planning
description: Esta é a atividade de lançamento do produto Adobe Workfront Planning para o quarto trimestre de 2026.
author: Becky
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 1b37b57f764d1579629e019c2025c809530124ea
workflow-type: tm+mt
source-wordcount: '1780'
ht-degree: 1%

---

# Atividade da versão do quarto trimestre de 2026 para o Adobe Workfront Planning

Este artigo descreve os recursos que estão sendo lançados para o Workfront Planning durante a versão do Quarto trimestre de 2026.

Para obter uma lista de todos os recursos lançados para o Adobe Workfront Planning, consulte [atividade de versão do Adobe Workfront Planning: índice do artigo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Gerenciar a visibilidade das miniaturas e cores dos registros a partir da coluna de campo principal na exibição de tabela

>[!NOTE]
>
>Visualização: 3 de setembro de 2026
>Versão rápida de produção: 17 de setembro de 2026
>Produção para todos: 15 de outubro de 2026

Agora é possível gerenciar a visibilidade das miniaturas e cores dos registros ao editar a coluna de campo principal na exibição de tabela.

Com esta atualização, as configurações de Miniatura e Cor serão removidas do ícone Campos na barra de ferramentas da exibição de tabela.

Para obter informações, consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md).

## Criar regras de negócios para tipos de registro

>[!NOTE]
>
>Visualização: 3 de setembro de 2026
>Versão rápida de produção: 17 de setembro de 2026
>Produção para todos: 15 de outubro de 2026

Como um gerenciador de espaço de trabalho, agora é possível definir regras de negócios para tipos de registro que refletirão posteriormente sobre como os registros desse tipo são gerenciados. Você pode definir regras que permitam aos usuários editar ou excluir registros somente quando determinadas condições forem atendidas ou determinados campos forem preenchidos.

É possível criar uma condição para a regra de negócios que faça referência a todos os tipos de campo, exceto para o seguinte:

* Campos de fórmula
* Campos de pesquisa
* Campos de referência

Não é possível adicionar regras de negócios a tipos de registros globais.

Para obter mais informações, consulte [Configurar regras de negócios do tipo registro](/help/quicksilver/planning/architecture/configure-business-rules.md).

>[!NOTE]
>
>Com esta atualização, as seguintes opções de menu no menu Mais de um tipo de registro também foram atualizadas:
>
>* **Criar formulários de solicitação** e **Gerenciar formulários de solicitação** foram alterados para **Formulários de solicitação**
>* **Gerenciar automações** alterada para **Automações**

## Introdução de semanas personalizadas para a exibição de linha do tempo

>[!NOTE]
>
>Visualização: 3 de setembro de 2026
>Versão rápida de produção: 17 de setembro de 2026
>Produção para todos: 15 de outubro de 2026

Como administrador do Workfront, agora você pode configurar semanas personalizadas, além de trimestres personalizados. Semanas e trimestres personalizados são visíveis na exibição da linha do tempo do Workfront Planning. O Workfront gera semanas sequenciais a partir da Semana 1 no início do Trimestre personalizado 1.

Você pode personalizar rótulos de semana que estejam visíveis na exibição de linha do tempo. Você pode escolher um formato predefinido ou inserir um personalizado.

As semanas personalizadas não estão visíveis no Workfront. Elas só são visíveis na exibição de linha do tempo do Workfront Planning.

Para obter informações, consulte [Habilitar trimestres personalizados](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md).

## Filtros para campos de registro conectados dependentes

>[!NOTE]
>
>Visualização: 3 de setembro de 2026
>Versão rápida de produção: 17 de setembro de 2026
>Produção para todos: 15 de outubro de 2026

Agora é possível filtrar por determinados tipos de registro que atendem a um critério de filtro quando você adiciona conexões dependentes no Planning.

Em vez de todos os tipos de registro estarem disponíveis em campos conectados dependentes, somente aqueles que atenderem aos seus critérios de filtragem serão exibidos.

Para esse recurso, adicionamos uma nova opção Record filtering rules na guia New connection ao conectar tipos de registro.

Para obter informações, consulte [Gerenciar conexões dependentes](/help/quicksilver/planning/architecture/manage-dependent-connections.md).

## Recolher e expandir todos os agrupamentos na exibição de linha do tempo

>[!NOTE]
>
>Visualização: 27 de agosto de 2026
>Versão rápida de produção: 17 de setembro de 2026
>Produção para todos: 15 de outubro de 2026

As exibições de linha do tempo agora incluem Recolher tudo e Expandir todas as opções de linhas do tempo agrupadas. Isso facilita a navegação em exibições de roteiro grandes: você pode reduzir rapidamente a exibição para cabeçalhos de agrupamento e expandir apenas as seções que deseja revisar.

Para obter mais informações, consulte [Gerenciar a exibição da linha do tempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Ver nomes completos dos grupos e redimensionar o painel de agrupamento na visualização de linha do tempo

>[!NOTE]
>
>Visualização: 27 de agosto de 2026
>Versão rápida de produção: 17 de setembro de 2026
>Produção para todos: 15 de outubro de 2026

Na exibição de linha do tempo, passar o mouse sobre um rótulo de grupo truncado agora mostra o texto completo em uma dica de ferramenta, na exibição de grupo Raia e Empilhado. Rótulos não truncados não mostram nenhuma dica de ferramenta.

O painel esquerdo de agrupamento na exibição Swimlane agora pode ser redimensionado arrastando seu divisor. A exibição é atualizada em tempo real, o que é consistente com a exibição de tabela. A largura do painel de cada usuário é salva entre as sessões, com uma largura padrão para usuários pela primeira vez.

Para obter informações, consulte [Gerenciar a exibição da linha do tempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Desempenho de calendário aprimorado para grandes conjuntos de registros na exibição semanal

>[!NOTE]
>
>Visualização: 27 de agosto de 2026
>Versão rápida de produção: 17 de setembro de 2026
>Produção para todos: 15 de outubro de 2026

A exibição da semana do calendário agora exibe apenas os primeiros 1.000 registros no período semanal visível. Se houver mais registros, a seguinte mensagem será exibida na parte inferior do calendário, indicando que registros adicionais estão disponíveis: &quot;Há mais registros. Carregue mais.&quot;

Para obter informações, consulte [Gerenciar a exibição de calendário](/help/quicksilver/planning/views/manage-the-calendar-view.md).

## Cabeçalhos de coluna atualizados para campos de registro conectados dependentes

>[!NOTE]
>
>Visualização: 20 de agosto de 2026
>Versão rápida de produção: 17 de setembro de 2026
>Produção para todos: 15 de outubro de 2026

Fizemos melhorias visuais nos cabeçalhos de coluna para um campo de registro conectado dependente na exibição de tabela.

Para obter informações, consulte [Gerenciar conexões dependentes](/help/quicksilver/planning/architecture/manage-dependent-connections.md).

## Aprimoramentos da exibição de tabela ao arrastar e soltar várias linhas

>[!NOTE]
>
>Visualização: 13 de agosto de 2026
>Versão rápida de produção: 13 de agosto de 2026
>Produção para todos: 15 de outubro de 2026
>[!BADGE Fora do cronograma]{type=Neutral}

Há novos indicadores visuais quando você arrasta e solta várias linhas na exibição de tabela. Um sinal de adição mais proeminente e um indicador de número agora mostram quantas linhas estão selecionadas para a ação arrastar e soltar.

Para obter informações, consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md).

## Rotear o objeto de solicitação enviado para o espaço de trabalho correto ao usar tipos de registro global

>[!NOTE]
>
>Visualização: 13 de agosto de 2026
>Versão rápida de produção: 17 de setembro de 2026
>Produção para todos: 15 de outubro de 2026

Os registros criados para tipos de registros globais enviando um formulário de solicitação agora são encaminhados automaticamente para o espaço de trabalho do qual foram enviados.

Os registros criados enviando uma solicitação de um espaço de trabalho secundário de um tipo de registro global são adicionados a esse espaço de trabalho secundário. Os registros criados submetendo uma solicitação do espaço de trabalho original ou da área Solicitações principal são adicionados ao espaço de trabalho original.

Se o formulário de entrada incluir um campo do Workspace e um usuário selecionar um espaço de trabalho antes de enviar, a solicitação será roteada para o espaço de trabalho selecionado, independentemente de onde o formulário foi iniciado. Isso garante que os registros sejam organizados no espaço de trabalho desejado a partir do momento em que são criados.

Para obter informações, consulte [Enviar solicitações do Adobe Workfront Planning para criar registros](/help/quicksilver/planning/requests/submit-requests.md).

## Introdução à Habilidade do Workfront Planning Solution Architect

>[!NOTE]
>
>Visualização: 10 de agosto de 2026
>Produção: 10 de agosto de 2026

Estamos lançando uma nova habilidade, o Arquiteto de soluções de planejamento da Workfront, que traz uma orientação prática recomendada e eficiente para o planejamento do Workfront diretamente para o Claude:

* **Configure** novos espaços de trabalho do Planning para especificação, com o servidor MCP do Workfront executando a instalação em seu ambiente.
* **Auditoria** configurações existentes para antipadrões em escala.
* **Verifique o uso** em relação aos limites recomendados (registros, conexões, profundidade da hierarquia).
* **Faça perguntas** sobre o Planejamento a qualquer momento.

Além da configuração inicial, a habilidade oferece suporte à governança contínua, capturando a deriva da configuração antes que ela cause atrito, sinalizando os limites próximos antes que eles se tornem bloqueadores, aplicando padrões consistentes em todos os espaços de trabalho, independentemente de quem os configura, e dando a qualquer pessoa da equipe respostas precisas sem esperar por um especialista. Juntos, isso abrange o ciclo de vida completo da configuração correta de um espaço de trabalho e sua manutenção conforme o uso cresce.

Para obter informações, consulte [Habilidades disponíveis para instalação direta](/help/quicksilver/workfront-basics/workfront-mcp-server/direct-skills.md).

## Arrastar e soltar linhas na exibição de tabela

>[!NOTE]
>
>Visualização: 30 de julho de 2026
>Versão rápida de produção: 13 de agosto de 2026
>Produção para todos: 15 de outubro de 2026

A experiência de arrastar e soltar linhas na exibição de tabela foi aprimorada visualmente.

Para obter informações, consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md).


## Campos de registro conectados dependentes

>[!NOTE]
>
>Visualização: 30 de julho de 2026
>Versão rápida de produção: 13 de agosto de 2026
>Produção para todos: 15 de outubro de 2026

Agora, os gerentes do Workspace podem definir dependências entre tipos de registro conectados. Por exemplo, garantir que um campo Região mostre apenas valores vinculados à Geografia selecionada. Isso é configurado diretamente na configuração do campo de conexão: ao adicionar uma conexão de um tipo de registro Geográfico a um tipo de registro dependente (como Região), uma nova configuração permite que os gerentes de espaço de trabalho marquem-na como dependente do tipo de registro Geográfico, usando os relacionamentos já estabelecidos entre esses tipos de registro.

Uma vez configurado, qualquer tipo de registro que referencie ambos os campos (como uma Campanha) verá o efeito imediatamente: selecionar um valor Geográfico restringe o seletor de Região somente às Regiões realmente vinculadas a essa Geografia. Isso reforça a estrutura de registros automaticamente, eliminando combinações incompatíveis e reduzindo a limpeza manual.

Os seguintes recursos estão incluídos nesta atualização:

* Adicionamos a nova seção Configurações de conexão na guia Nova conexão, ao conectar tipos de registro
* Adicionamos uma configuração Tornar essa conexão dependente na nova seção
* Alteramos a maneira como você adiciona campos de pesquisa a conexões


Para obter informações, consulte [Gerenciar conexões dependentes](/help/quicksilver/planning/architecture/manage-dependent-connections.md).




## Mostrar novo indicador de comentário para um registro na exibição de tabela

>[!NOTE]
>
>Visualização: 30 de julho de 2026
>Versão rápida de produção: 13 de agosto de 2026
>Produção para todos: 15 de outubro de 2026

Adicionamos um novo indicador que mostra quando há comentários não lidos em um registro. O indicador é exibido no canto superior direito do campo principal do registro na exibição de tabela.

Para obter mais informações, consulte [Gerenciar comentários de registro](/help/quicksilver/planning/records/manage-record-comments.md).

## Cor de registro personalizável e codificação de cores baseada em conexão

>[!NOTE]
> 
>Visualização: 23 de julho de 2026
>Versão rápida de produção: 13 de agosto de 2026
>Produção para todos: 15 de outubro de 2026

Os registros agora oferecem suporte a paletas de cores personalizáveis, que permitem atualizar as cores automaticamente atribuídas a novos registros para cores padrão ou personalizadas.

As seguintes alterações estão incluídas neste aprimoramento: 

* Adicionamos a opção Cor às seguintes áreas:
  * O ícone Campos na exibição de tabela. 
  * A seção Estilo da barra na área Configurações de uma linha do tempo e uma visão de calendário

    Quando a configuração Cor está ativada, a cor atribuída a um novo registro é exibida em todos os locais em que o registro é exibido nessas exibições. 

* Um círculo de cores é adicionado à página Detalhes do registro. 
* Agora é possível adicionar campos de registro de seleção única, múltipla e conectados à codificação por cores de barras nas exibições de linha do tempo e calendário ao colorir por valores de Campo. 
* É possível habilitar a exibição da cor, além do nome e da imagem de um registro ao criar campos de registro conectados. 
* A seção Cor, na área Configurações, também foi simplificada com a remoção da opção &quot;Nenhum&quot;.  

Para obter informações, consulte [Criar registros](/help/quicksilver/planning/records/create-records.md). 

## O Planning Designer agora exige a aceitação do contrato do Beta

>[!NOTE]
>Pré-visualização e produção para todos os clientes: 20 de julho de 2026
>[!BADGE Fora do cronograma]{type=Neutral}

O Planning Designer agora exige um contrato aceito do Beta para ser usado. Sua empresa não precisa assinar um contrato de IA. Isso está disponível para todos os clientes.

Para isso, movemos a opção Planning Designer na seção Configuração da seção Opt in to AI Betas.

Iniciar o Planning Designer sem um contrato Beta aceito agora solicitará a aceitação antes que o construtor do espaço de trabalho seja aberto.

Para obter informações, consulte [Introdução ao Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).
