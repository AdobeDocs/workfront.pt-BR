---
product-area: documents
navigation-topic: approvals
title: O que há de diferente no armazenamento em nuvem do Adobe
description: Entenda as principais diferenças nos objetos de armazenamento na nuvem do Adobe, incluindo a nova área Documentos, o visualizador Frame.io, permissões de documento, regras de nomenclatura de objetos, cota de armazenamento e Workfront Fusion.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: 4f63b6c4f4c73bedba707aed6b02c9046f9b356c
workflow-type: tm+mt
source-wordcount: '1717'
ht-degree: 0%
---
# O que há de diferente no armazenamento em nuvem do Adobe

Depois que seu contrato for atualizado para incluir a nova experiência unificada de revisão e aprovação, seu ambiente poderá conter dois tipos de objetos: objetos no armazenamento herdado do Workfront (os objetos que você tem hoje) e objetos criados usando o armazenamento em nuvem da Adobe. A nova área Documentos, o visualizador Frame.io e os outros comportamentos descritos aqui se aplicam apenas a objetos que usam o armazenamento na nuvem do Adobe.

Para obter uma orientação para a movimentação e o que é ativado quando, consulte [Mover para o Workfront no Adobe Cloud Storage](/help/quicksilver/review-and-approve-work/workfront-storage.md).

## Entenda o armazenamento herdado do Workfront e o armazenamento em nuvem do Adobe

Em um alto nível, os dois modelos de armazenamento diferem em onde os dados residem, quais produtos da Adobe podem visualizá-los e qual funcionalidade está disponível:

|  | Objeto no armazenamento herdado do Workfront | Objeto no armazenamento em nuvem do Adobe |
|---|---|---|
| Infraestrutura de armazenamento | Somente Workfront | Armazenamento na nuvem da Adobe |
| Visibilidade entre produtos | Somente Workfront | Workfront, Frame.io e Creative Cloud |
| Funcionalidade | Funcionalidade herdada | Nova funcionalidade |

Os objetos criados antes do armazenamento na nuvem do Adobe são o padrão, permanecem no armazenamento herdado do Workfront. Os comportamentos descritos neste artigo se aplicam apenas aos objetos de armazenamento em nuvem do Adobe que você e seus usuários criam depois que o armazenamento em nuvem do Adobe é o padrão.

## Resumo das diferenças

A maior alteração diária com o armazenamento em nuvem do Adobe é a nova área Documentos e o visualizador Frame.io que possibilita a revisão e a aprovação dentro dela. Há outras diferenças que afetam como você gerencia objetos, documentos e revisões. Cada área na tabela a seguir está vinculada à seção detalhada abaixo.

| Área | O que é diferente | O que saber |
|---|---|---|
| [A nova área Documentos](#the-new-documents-area) | Uma área Documentos unificada e reprojetada substitui a área Documentos herdada. | Não há uma área de Documentos global. Você acessa documentos de um programa, portfólio, projeto, tarefa ou problema. |
| [Permissões de documento](#document-permissions) | Os documentos herdam permissões do projeto, tarefa ou problema ao qual estão vinculados. | Você não pode compartilhar ou definir permissões em documentos individuais. Você gerencia todo o acesso por meio do modal Compartilhamento de objetos no Workfront, que é enviado em cascata para pastas de documentos geradas pelo sistema. |
| [Mapeamento de permissões de objeto](#object-permissions-mapping) | As permissões Gerenciar e Contribute mapeiam para Editar e Compartilhar no Frame.io. Visualizar mapas para Somente comentário. | Você gerencia permissões no Workfront. Os usuários do Manage e do Contribute obtêm o recurso de compartilhamento externo no Frame.io. |
| [Visualizador de revisão e aprovação](#review-and-approval-viewer) | O visualizador Frame.io substitui o visualizador do Workfront Proofing. | Está incluído para todos os usuários do Workfront, incluindo usuários externos atribuídos a uma revisão ou aprovação. Ele é compatível com marcação, comentários com carimbo de data e hora, histórico de versões, dispositivos móveis, formatos com mais de 40 anos e arquivos de até 500 GB. |
| [Regras de nomenclatura de objetos](#object-naming-rules) | Regras de nomenclatura rígidas se aplicam: nomes exclusivos em um portfólio ou projeto, sem caracteres especiais, sem ponto ou espaço à direita e um limite de 255 caracteres. | O Workfront renomeia objetos automaticamente quando surgem conflitos. Auditoria de modelos que geram novos nomes e estrutura de projeto. |
| [Portabilidade de objeto](#object-portability) | Na maioria dos cenários, você pode mover, copiar e converter objetos somente entre modelos de armazenamento semelhantes. | Você pode converter um objeto herdado para o armazenamento em nuvem do Adobe em três casos específicos. Os documentos e as pastas de documentos não são movidos do armazenamento herdado durante a conversão. |
| [Recursos não disponíveis](#capabilities-not-available-on-adobe-cloud-storage-objects) | Workfront Proof, o visualizador de documentos do Workfront, documentos favoritos e documentos de solicitação não fazem parte da experiência. | Os objetos herdados retêm esses recursos. O Workfront Proof não receberá novo investimento e será removido em uma versão futura. |
| [Cota de armazenamento](#storage-quota) | O armazenamento é agrupado para projetos herdados do Workfront e projetos Adobe de armazenamento na nuvem, a 60 GB por usuário licenciado, sem limite rígido. | Os administradores do sistema podem visualizar o uso do armazenamento na página Informações do cliente em Configuração. |
| [Limite anual de análise de vídeo](#annual-video-review-cap) | Há um limite em nível de organização para solicitações de prova de vídeo de 10% das licenças pagas de usuário do Workfront (Standard e Light). | Depois de atingir o limite, você não poderá criar novas análises de vídeo até o próximo período anual. Você recebe notificações no aplicativo em 80% e 100%. O limite não se aplica a clientes do Frame.io Enterprise. |
| [Workfront Fusion](#workfront-fusion-on-adobe-cloud-storage-projects) | Os cenários de Fusão baseados em prova existentes não funcionam automaticamente em projetos de armazenamento em nuvem do Adobe. | Os cenários com escopo para projetos herdados continuam a funcionar. Cada cenário afetado toma um dos três caminhos: editar, reconstruir ou desativar. |

## A nova área Documentos

A nova área Documentos é uma experiência de documentos unificada projetada para o armazenamento em nuvem do Adobe. Ele simplifica a navegação, consolida a atividade de revisão e aprovação e é o ponto de entrada para o visualizador Frame.io.

A área Documentos global não faz parte da nova experiência. Em projetos de armazenamento na nuvem do Adobe, você acessa documentos de um programa, portfólio, projeto, tarefa ou problema.

Para obter mais informações, consulte [A área Documentos](/help/quicksilver/documents/managing-documents/documents-area.md).

## Permissões de documento

As permissões de documento são fundamentalmente diferentes em projetos de armazenamento em nuvem do Adobe:

* Você não pode compartilhar ou definir permissões em documentos individuais. Em vez disso, as permissões são aplicadas às pastas de documentos geradas pelo sistema que contêm os documentos.
* As pastas de documentos geradas pelo sistema herdam permissões do projeto, tarefa ou problema pai.
* As subpastas herdam permissões da pasta de documentos gerada pelo sistema principal.
* Subtarefas não herdam permissões de tarefas pai. Você deve ser adicionado diretamente a uma subtarefa para acessar sua pasta de documentos gerada pelo sistema.

Para obter mais informações sobre como as permissões de documento funcionam, consulte [Visão geral sobre permissões de objeto e nível de acesso do modelo de armazenamento na nuvem do Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

## Mapeamento de permissões de objeto

As permissões são definidas no Workfront e fluem em uma direção até o Frame.io. Você não pode convidar usuários para um projeto de armazenamento em nuvem do Adobe no Frame.io ou modificar permissões de usuário no Frame.io.

>[!TIP]
>
>Treine coordenadores de projetos para que o acesso ao Frame.io seja um reflexo downstream das permissões do Workfront. Se uma parte interessada relatar que não pode acessar uma revisão em um projeto de armazenamento na nuvem da Adobe, a correção será no Workfront, não no Frame.io.

A tabela a seguir mapeia permissões de objetos do Workfront para permissões de Frame.io:

| Permissão do Workfront | Permissão de Frame.io |
|---|---|
| Gerenciar | Editar e compartilhar |
| Contribuir | Editar e compartilhar |
| Exibir | Somente comentário |

Gerenciar e Contribute mapear para Editar e Compartilhar no Frame.io. Ao analisar os padrões de compartilhamento para projetos de armazenamento na nuvem do Adobe, considere se o modelo de governança ideal para os colaboradores tem os mesmos recursos de revisão que os gerentes, incluindo compartilhamento externo.

Para obter mais informações, consulte [Visão geral das permissões de objeto e do nível de acesso para o modelo de armazenamento na nuvem do Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#permission-mapping-to-frameio).

## Visualizador de revisão e aprovação

Em objetos de armazenamento na nuvem do Adobe, o visualizador Frame.io é a superfície de revisão e aprovação no lugar do Workfront Proof. O visualizador Frame.io é incluído para todos os usuários do Workfront sem custo adicional, incluindo usuários externos que são atribuídos a uma revisão ou aprovação.

O visualizador Frame.io fornece:

* Ferramentas de marcação e comentários, incluindo desenho à mão livre e formas padrão, como círculos, setas e quadrados
* Comentários com carimbo de data e hora com precisão de quadro preciso para revisões de vídeo
* Histórico de versão e comparação de versão
* Acesso móvel para revisões e aprovações em qualquer lugar
* Suporte para mais de 40 formatos de arquivo, incluindo todos os tipos comuns de vídeo, imagem, áudio, PDF e Microsoft Office, com reprodução nativa para formatos de vídeo profissional, como ProRes, H.265 e DNxHD, e suporte para arquivos de até 500 GB

## Regras de nomenclatura de objeto

O Adobe Cloud Storage aplica regras estruturais e de nomenclatura rigorosas para manter a camada de armazenamento consistente em todos os produtos da Adobe. Essas regras se aplicam aos objetos criados em projetos de armazenamento na nuvem do Adobe. Os projetos herdados existentes mantêm seus nomes atuais.

As seguintes regras se aplicam aos projetos de armazenamento em nuvem do Adobe:

| Regra | Detalhe |
|---|---|
| Nomes exclusivos de programas e projetos | Programas e projetos não podem ter o mesmo nome se pertencerem ao mesmo portfólio. |
| Nomes exclusivos de documentos | Documentos não podem ter o mesmo nome se pertencerem ao mesmo projeto. Os nomes de documento devem ser exclusivos dentro do mesmo pai na hierarquia de pastas. |
| Caracteres proibidos | Programas, portfólios, projetos, modelos, tarefas, problemas, pastas de documentos e documentos não podem conter nenhum dos seguintes caracteres especiais: `\ / : * ? " \| < >` |
| Caracteres finais | Programas, portfólios, projetos, modelos, tarefas, problemas e pastas de documentos não podem ter nomes que terminem com um ponto ou um espaço. |
| Limite de comprimento do nome | Os nomes dos objetos são limitados a 255 caracteres. |

Se um nome entrar em conflito com essas regras, o Workfront renomeará automaticamente o objeto para resolver o conflito.

>[!TIP]
>
>Se você criar projetos do Adobe Cloud Storage a partir de modelos, revise seus modelos existentes para que os nomes e a estrutura dos projetos gerados se encaixem nas regras acima.

## Portabilidade do objeto

Na maioria dos cenários, você pode mover, copiar e converter objetos Workfront somente entre modelos de armazenamento semelhantes. Por exemplo, você pode mover uma tarefa de um projeto de armazenamento em nuvem do Adobe para outro projeto de armazenamento em nuvem do Adobe. Em três casos específicos, você pode converter um objeto de armazenamento herdado do Workfront no armazenamento em nuvem do Adobe.

Para obter mais informações, consulte [Converter objetos herdados para o armazenamento na nuvem do Adobe](/help/quicksilver/review-and-approve-work/convert-objects-to-adobe-cloud-storage.md).

## Recursos não disponíveis em objetos de armazenamento na nuvem do Adobe

Os seguintes recursos não fazem parte dos objetos de armazenamento na nuvem do Adobe:

* Workfront Proof
* O visualizador de documentos do Workfront
* Documentos favoritos
* Solicitar documentos

Os projetos herdados mantêm o acesso ao Workfront Proof e aos recursos de documento herdados listados acima. A Workfront Proof não receberá novos investimentos no futuro e será removida em uma versão futura.

## Cota de armazenamento

O armazenamento é agrupado para objetos herdados do Workfront e objetos de armazenamento na nuvem do Adobe. Cada usuário licenciado recebe 60 GB de armazenamento. Não há limite rígido para o uso de armazenamento, mas os administradores do Workfront recebem notificações por email quando o uso atinge 75%, 90% e 100% da cota.

Para exibir o uso e a cota de armazenamento atuais, vá para **Configuração** > **Sistema** > **Informações do Cliente**.

Para obter mais informações, consulte [Verificar limites de armazenamento de documentos](/help/quicksilver/documents/managing-documents/check-document-storage.md).

## Limite anual de análise de vídeo

Há um limite anual de solicitações de prova de vídeo definido em 10% do total de licenças pagas de usuário do Workfront da sua organização (Standard e Light). Esse limite é aplicado no nível da organização.

* Os administradores do Workfront recebem notificações no aplicativo quando o uso atinge 80% e 100% do limite.
* Depois de atingir o limite, você não poderá criar novas solicitações de análise de vídeo até o próximo período anual.
* Esse limite não se aplica a clientes do Frame.io Enterprise. Se sua organização analisa regularmente grandes volumes de conteúdo de vídeo, entre em contato com o representante de conta da Adobe para saber mais sobre o licenciamento Frame.io Enterprise.

Para obter mais informações, consulte as Perguntas frequentes sobre revisão e aprovação de ativos e vídeos na [Visão geral de revisão e aprovação unificada](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

## Workfront Fusion em projetos de armazenamento em nuvem do Adobe

Os cenários do Workfront Fusion existentes criados em revisões herdadas não funcionam automaticamente em projetos de armazenamento na nuvem do Adobe. Módulos específicos de prova, webhooks e endpoints de API têm equivalentes diretos em alguns casos e alterações significativas em outros. Os cenários com escopo para projetos herdados continuam a funcionar como funcionam atualmente.

Para obter informações detalhadas sobre o impacto em tipos de cenários comuns e como classificar cada cenário como Editar, Recompilar ou Desativar com base em sua funcionalidade, consulte [Atualizar cenários do Workfront Fusion para revisão e aprovação unificadas](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).
