---
content-type: release-notes
navigation-topic: product-releases-archive
title: Atividade da versão Beta 5 2018.3
description: Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão Beta 5 de 2018.3. A funcionalidade estará disponível no ambiente de Pré-visualização em 21 de setembro de 2018. Ele estará disponível no ambiente de Produção em novembro de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f208b566-2529-4c4d-aa66-0c8756e55a5a
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2147'
ht-degree: 0%

---

# Atividade da versão Beta 5 2018.3

Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão Beta 5 de 2018.3. A funcionalidade estará disponível no ambiente de Pré-visualização em 21 de setembro de 2018. Ele estará disponível no ambiente de Produção em novembro de 2018.

Para obter uma lista de todas as alterações feitas em 2018.3, consulte  [Visão geral da atividade da versão 2018.3](../../../../product-announcements/product-releases/quarterly-release-archive/2018.3-release-activity/2018-3-release-activity-overview.md).

A versão Beta 5 de 2018.3 contém melhorias para todos os usuários:

* [Rastrear aprovações enviadas na área Página inicial](#track-approvals-you-ve-submitted-in-the-home-area)
* [Substituição de ferramentas baseadas em Flashes no Workfront](#replacement-of-flash-based-tools-in-workfront)
* [Permitindo que Usuários da Licença de Trabalho Acessem a Subguia Agendamento de um Projeto](#allowing-work-license-users-to-access-the-scheduling-subtab-of-a-project)
* [Filtros aprimorados no Planejador de recursos](#improved-filters-in-the-resource-planner)
* [Visualizar Horas efetivas no Planejador de recursos](#view-actual-hours-in-the-resource-planner)
* [Dados do Planejador de Recursos na Exportação de Business Case](#resource-planner-data-in-the-business-case-export)
* [Habilitar Substituição de Taxa de Cobrança no Nível da Empresa](#enable-company-level-billing-rate-override)
* [Aprovações simplificadas com base em funções](#simplified-role-based-approvals)
* [Relatório de Utilização: Preenche Horas Orçadas da Nova Área de Orçamento de Recursos](#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area)
* [Relatório de Utilização: Exibir Horas Orçadas por Usuário em um Projeto](#utilization-report-view-budgeted-hours-by-user-on-a-project)
* [Arquivos SWF não são mais suportados no visualizador de provas](#swf-files-no-longer-supported-in-the-proofing-viewer)
* [Ações mais rapidamente acessíveis na Lista de comentários no visualizador de provas](#actions-more-quickly-accessible-in-the-comment-list-in-the-proofing-viewer)
* [Melhorias no compartilhamento de provas no visualizador de provas](#proof-sharing-improvement-in-the-proofing-viewer)
* [Aprimoramentos da lista de comentários no visualizador de provas](#comments-list-enhancements-in-the-proofing-viewer)
* [Provas de vídeo de Zoom e Panorâmica no visualizador de provas](#zoom-and-pan-video-proofs-in-the-proofing-viewer)
* [Plano de fundo mais claro no visualizador de provas](#lighter-background-in-the-proofing-viewer)
* [Melhor visibilidade quando um comentário é editado no visualizador de provas](#better-visibility-when-a-comment-has-been-edited-in-the-proofing-viewer)
* [Exibir o Número de Comentários Associados a uma Ação na Lista de Comentários no visualizador da prova](#view-the-number-of-comments-associated-with-an-action-in-the-comment-list-in-the-proofing-viewer)
* [Especificar o estágio ao adicionar usuários a uma prova no visualizador de provas](#specify-the-stage-when-adding-users-to-a-proof-in-the-proofing-viewer)
* [Abrir o site associado a partir de uma prova interativa ou estática do site](#opening-the-associated-website-from-an-interactive-or-static-website-proof)
* [Melhorias no resumo de impressão](#print-summary-enhancements)
* [Tempo de carregamento de prova aprimorado](#improved-proof-loading-time)
* [Nova aparência da guia Atualizações no aplicativo móvel do Workfront](#new-look-and-feel-of-the-updates-tab-in-the-workfront-mobile-app)

## Rastrear aprovações enviadas na área Página inicial {#track-approvals-you-ve-submitted-in-the-home-area}

Agora você pode usar a área da página inicial para interagir com as aprovações enviadas a outros usuários.

Em Casa, você pode:

* Cancelar aprovações
* Lembrar usuários de aprovações
* Adicionar usuários às aprovações de documentos
* Exibir aprovações de provas

  Anteriormente, só era possível interagir com aprovações enviadas na área Meu trabalho. 

Para obter mais informações, consulte [Gerenciar aprovações](../../../../review-and-approve-work/manage-approvals/manage-approvals.md). 

## Substituição de ferramentas baseadas em Flashes no Workfront {#replacement-of-flash-based-tools-in-workfront}

Toda a funcionalidade que depende da tecnologia Flash está planejada para ser removida do Workfront com a versão 2018.3 e será substituída por uma nova solução.

Para obter mais informações sobre todas as áreas afetadas pela remoção desses recursos e para entender quais ferramentas os substituirão, consulte [Substituição de ferramentas baseadas em Flashes no Adobe Workfront](../../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).

## Permitindo que Usuários da Licença de Trabalho Acessem a Subguia Agendamento de um Projeto {#allowing-work-license-users-to-access-the-scheduling-subtab-of-a-project}

Os usuários com uma licença de Trabalho agora podem acessar a subguia Agendamento de um projeto, na guia Equipe.

Antes dessa melhoria, somente os usuários com uma licença de Plano podiam acessar essa subguia.

Para obter informações sobre o acesso necessário para acessar a subguia Agendamento de um projeto, consulte &quot;Introdução ao Agendamento de recursos&quot;.

>[!NOTE]
>
>As ferramentas de Agendamento de recursos foram substituídas e removidas do Workfront com a versão 23.1. Para obter informações sobre como programar recursos usando o Balanceador de carga de trabalho, consulte [Visão geral do Balanceador de carga de trabalho](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## Filtros aprimorados no Planejador de recursos {#improved-filters-in-the-resource-planner}

Agora é possível filtrar as informações no Planejador de recursos para incluir campos específicos do projeto e do usuário, incluindo campos personalizados.

Antes dessa melhoria, você só poderia filtrar por um número limitado de campos e critérios integrados no Planejador de recursos.

Para obter informações sobre como filtrar informações no Planejador de recursos, consulte [Filtrar informações no Planejador de recursos](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

## Visualizar Horas efetivas no Planejador de recursos {#view-actual-hours-in-the-resource-planner}

Você pode ver as Horas efetivas na visão de usuário do Planejador de recursos.

Antes dessa melhoria, as Horas efetivas não estavam visíveis no Planejador de recursos.

Para obter informações sobre a exibição de informações de horas no Planejador de recursos, consulte [Visão geral do Planejador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Dados do Planejador de Recursos na Exportação de Business Case {#resource-planner-data-in-the-business-case-export}

Quando você exporta o Business Case para um PDF, as informações financeiras no arquivo exportado agora refletem as informações na área Orçamento de recursos e no Planejador de recursos. 

Anteriormente, o arquivo exportado refletia as informações na área Estimativas de recursos legados e no Planejador de capacidade. 

Para obter informações sobre como exportar o Business Case, consulte o [Criar um Business Case para um projeto](../../../../manage-work/projects/define-a-business-case/create-business-case.md) seção em [Criar um Business Case para um projeto](../../../../manage-work/projects/define-a-business-case/create-business-case.md).

## Habilitar Substituição de Taxa de Cobrança no Nível da Empresa {#enable-company-level-billing-rate-override}

Agora você pode habilitar uma opção para permitir que taxas de cobrança no nível da empresa substituam taxas de cobrança no nível do projeto. Depois de atualizar as taxas de cobrança no nível da empresa, você pode recalcular manualmente as finanças do projeto para refletir essas alterações.

Se você habilitar essa configuração, as taxas de cobrança no nível da empresa substituirão as taxas de função de trabalho históricas no projeto.

Anteriormente, você não podia aplicar alterações de taxas de cobrança no nível da empresa a um projeto, a menos que removesse a empresa do projeto e, em seguida, o reanexasse.

Para obter mais informações, consulte [Sobrepor Taxas de Cobrança no Nível do Projeto com Taxas de Cobrança no Nível da Empresa](../../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md). 

## Aprovações simplificadas com base em funções {#simplified-role-based-approvals}

As aprovações com base em funções agora funcionam mais simplesmente em um projeto. Agora, os usuários devem ser atribuídos à equipe do projeto e ter a função atribuída em seu perfil de usuário para ver as aprovações atribuídas a suas funções principais ou secundárias.

Anteriormente, você tinha que atribuir usuários à equipe do projeto, garantir que eles tivessem a função correta em seu perfil de usuário e selecionar essa função no Construtor de equipe herdado.

Para obter mais informações, consulte a seção [Visão geral da equipe do projeto](../../../../manage-work/projects/planning-a-project/project-team-overview.md) no artigo [Visão geral da equipe do projeto](../../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Relatório de Utilização: Preenche Horas Orçadas da Nova Área de Orçamento de Recursos {#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area}

>[!NOTE]
>
> Essa funcionalidade foi introduzida pela primeira vez no ambiente de Pré-visualização com a versão 2018.2. Ele será lançado para o ambiente de Produção com a versão 2018.3. 

As horas orçadas no Relatório de utilização agora são preenchidas com base nas informações disponíveis na nova área Orçamento de recursos do Business Case.

Antes dessa alteração, eram usadas informações da área Estimativas de recursos herdada.

Para obter mais informações, consulte  [Visão Geral do relatório de Utilização de Recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) no artigo  [Visão Geral do relatório de Utilização de Recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Relatório de Utilização: Exibir Horas Orçadas por Usuário em um Projeto {#utilization-report-view-budgeted-hours-by-user-on-a-project}

>[!NOTE]
>
>Essa funcionalidade foi introduzida pela primeira vez no ambiente de Pré-visualização com a versão 2018.2. Ele será lançado para o ambiente de Produção com a versão 2018.3. 

O relatório de Utilização em um projeto agora exibe Horas orçadas por usuário.

Antes dessa alteração, o relatório de Utilização exibia as Horas Orçadas somente por função de trabalho. 

Para obter mais informações, consulte  [Visão Geral do relatório de Utilização de Recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) no artigo  [Visão Geral do relatório de Utilização de Recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Arquivos SWF não são mais suportados no visualizador de provas {#swf-files-no-longer-supported-in-the-proofing-viewer}

Devido a preocupações de segurança associadas ao Flash Adobe, o visualizador de provas não é mais compatível com provas criadas a partir de arquivos SWF. Se você abrir uma prova criada anteriormente para um arquivo SWF, será exibida uma mensagem mostrando onde o conteúdo da prova era exibido anteriormente no visualizador de provas. Você pode ver qualquer comentário na prova. Você também pode baixar comentários e o arquivo SWF original.

Para obter mais informações, consulte [Visão geral de tipos de arquivo de comprovação e limites de tamanho compatíveis](../../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md) no artigo [Visão geral de tipos de arquivo de comprovação e limites de tamanho compatíveis](../../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md). 

## Ações mais rapidamente acessíveis na Lista de comentários no visualizador de provas {#actions-more-quickly-accessible-in-the-comment-list-in-the-proofing-viewer}

Agora é possível adicionar ou alterar mais rapidamente a ação de um comentário no visualizador de provas. Basta clicar no ícone Mais em qualquer comentário e, em seguida, clicar na ação desejada no menu suspenso.

Anteriormente, era necessário abrir o comentário, abrir um menu suspenso, abrir um submenu e clicar na ação desejada.

Para obter mais informações, consulte [Usar ações em comentários de prova](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md).

## Melhorias no compartilhamento de provas no visualizador de provas {#proof-sharing-improvement-in-the-proofing-viewer}

Ao enviar um URL do revisor de provas, as opções exibidas agora são organizadas exatamente como as opções exibidas ao compartilhar um URL na área Documentos.

Anteriormente, essas opções forneciam a mesma funcionalidade que agora, mas sua organização era inconsistente com as opções correspondentes na lista Documentos.

Para obter mais informações, consulte a seção  [Compartilhar o URL](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-the-url) no artigo  [Compartilhar uma prova do visualizador de provas](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

## Aprimoramentos da lista de comentários no visualizador de provas {#comments-list-enhancements-in-the-proofing-viewer}

As seguintes melhorias estão disponíveis na Lista de comentários:

* Um plano de fundo cinza-claro agora é exibido atrás do texto do comentário para destacá-lo de outro texto exibido no painel Comentários, como nomes de revisores, tempos de revisão e números de página de prova. Isso facilita a leitura de comentários de prova somente quando essa é a única coisa que você deseja ler.

  Anteriormente, o plano de fundo inteiro do painel Comentários era branco.

  Para obter mais informações, consulte.

* As respostas a um comentário agora são recuadas abaixo do comentário. Isso facilita a distinção entre as respostas do comentário original acima delas.

  Anteriormente, as respostas em um comentário eram alinhadas à esquerda com o comentário.

  Para obter mais informações, consulte em .

* Ao resolver um comentário no visualizador de provas, o ícone de marca de seleção verde Resolvido é exibido sem texto no canto superior direito do comentário. Isso dá ao painel Comentário uma aparência mais limpa, mais fácil de pesquisar as informações necessárias.

  Anteriormente, o ícone de marca de seleção Resolvido aparecia ao lado da palavra RESOLVIDO no canto superior esquerdo do comentário 

  Para obter mais informações, consulte em .

## Provas de vídeo de Zoom e Panorâmica no visualizador de provas {#zoom-and-pan-video-proofs-in-the-proofing-viewer}

Agora é possível ampliar as provas de vídeo e deslocar para áreas da prova que você precisa examinar mais detalhadamente.

## Plano de fundo mais claro no visualizador de provas {#lighter-background-in-the-proofing-viewer}

O plano de fundo no visualizador de provas agora é um pouco mais claro. Essa alteração facilita a distinção de conteúdo de prova que contém bordas e planos de fundo pretos.

Anteriormente, o plano de fundo do visualizador de provas estava preto.

## Melhor visibilidade quando um comentário é editado no visualizador de provas {#better-visibility-when-a-comment-has-been-edited-in-the-proofing-viewer}

O rótulo &quot;Editado&quot; agora aparece em qualquer comentário que um revisor tenha alterado. Ao passar o mouse sobre ele, o nome do revisor e a data da alteração são exibidos.

## Exibir o Número de Comentários Associados a uma Ação na Lista de Comentários no visualizador da prova {#view-the-number-of-comments-associated-with-an-action-in-the-comment-list-in-the-proofing-viewer}

Ao clicar no ícone Filtro na lista Comentário, agora é possível ver quantos comentários estão associados a cada ação.

As ações estão disponíveis na lista Comentário somente se estiverem habilitadas para sua organização.

## Especificar o estágio ao adicionar usuários a uma prova no visualizador de provas {#specify-the-stage-when-adding-users-to-a-proof-in-the-proofing-viewer}

Ao adicionar um revisor a uma prova que tenha um fluxo de trabalho automatizado no visualizador de provas, você pode especificar o estágio em que deseja que o revisor trabalhe na prova. Essa é a funcionalidade disponível ao adicionar usuários a uma prova fora do visualizador de provas.

Anteriormente, ao adicionar revisores a uma prova do visualizador de provas, o Workfront os colocava no estágio que estava ativo no momento.

Para obter mais informações, consulte [Compartilhar uma prova adicionando usuários a ela](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) in [Compartilhar uma prova do visualizador de provas](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

## Abrir o site associado a partir de uma prova interativa ou estática do site {#opening-the-associated-website-from-an-interactive-or-static-website-proof}

Ao revisar uma prova com conteúdo da Web interativo ou estático, agora é possível clicar em um botão para abrir facilmente o site associado em uma nova guia do navegador no visualizador de provas. Isso permite comparar o que você vê na prova com o site real usando duas guias diferentes.

Anteriormente, você podia abrir o site associado passando o mouse sobre o URL e clicando na dica de ferramenta. Essa abordagem era acessível e intuitiva.

## Melhorias no resumo de impressão {#print-summary-enhancements}

As seguintes melhorias estão disponíveis na página Resumo de impressão:

* Agora é possível especificar se deseja incluir todas as páginas na prova ou somente as páginas que contêm comentários.

  Anteriormente, só era possível incluir as páginas que continham comentários.

* Se sua prova tiver estágios, agora é possível incluir um diagrama que mostra a ordem dos estágios da prova e as decisões tomadas para cada estágio.

  Anteriormente, esse diagrama não estava disponível.

* Agora, quando várias marcações são associadas a um comentário, o número desse comentário aparece em cada marcação na página Resumo de impressão.

  Anteriormente, o número do comentário aparecia somente na primeira marcação associada ao comentário. As outras marcações do comentário exibidas sem um número.

* Se a prova for uma captura da Web, qualquer página contendo comentários exibirá a resolução na qual a página da Web foi capturada. Isso é útil, por exemplo, se a prova contiver páginas capturadas para dispositivos móveis e as mesmas páginas capturadas para notebooks e desktops.
* Agora, ao filtrar comentários na página Resumo de impressão por Ação, Autor ou status Não resolvido, o filtro se aplica às provas exportadas como arquivos PDF ou Excel, não apenas provas impressas.

Para obter mais informações, consulte [Imprimir um resumo de prova no Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

## Tempo de carregamento de prova aprimorado {#improved-proof-loading-time}

Fizemos algumas melhorias de desempenho que devem resultar em tempos de carregamento melhores ao abrir provas.

Para obter informações sobre como abrir provas, consulte.

## Nova aparência da guia Atualizações no aplicativo móvel do Workfront {#new-look-and-feel-of-the-updates-tab-in-the-workfront-mobile-app}

A aparência da guia Atualizações no Aplicativo móvel foi atualizada. No momento, esse aprimoramento está disponível somente no aplicativo beta do Workfront para Android.

Para obter informações sobre como gerenciar atualizações e comentários no aplicativo móvel do Workfront, consulte a seção em .
