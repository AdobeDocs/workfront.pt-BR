---
product-area: documents
navigation-topic: approvals
title: Migrar para o Workfront no Adobe Cloud Storage
description: Planeje a implantação do Workfront no Adobe Cloud Storage. Saiba o que há de diferente nos objetos de armazenamento em nuvem do Adobe, incluindo a nova área Documentos e a experiência de revisão do Frame.io, e decida como o armazenamento em nuvem do Adobe é implantado em seu ambiente.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: 7fc5fe2f2692841a8663740441f70be0c82c4073
workflow-type: tm+mt
source-wordcount: '2359'
ht-degree: 0%

---

# Migrar para o Workfront no Adobe Cloud Storage

O Workfront no Adobe Cloud Storage permite a experiência completa de revisão e aprovação unificada: revisões no visualizador Frame.io, fluxos de trabalho de aprovação avançados, visibilidade entre produtos de ativos e muito mais.

Os objetos existentes continuam a funcionar da maneira que funcionam hoje. A nova área Documentos, o visualizador Frame.io e outros comportamentos de armazenamento em nuvem do Adobe se aplicam apenas a objetos que usam o armazenamento em nuvem do Adobe.

Este artigo é para administradores do Workfront que estão se preparando para implantar o Workfront no Adobe Cloud Storage. Ele aborda as principais diferenças nos objetos de armazenamento na nuvem do Adobe, como escolher o tipo de implantação e o que pensar antes de habilitar o armazenamento na nuvem do Adobe para seus usuários.

>[!IMPORTANT]
>
>Você deve ter uma versão do Workfront compatível com o armazenamento em nuvem da Adobe. Se sua organização ainda não tiver uma versão compatível, entre em contato com o representante de conta da Adobe.



## Entenda o armazenamento herdado do Workfront e o armazenamento em nuvem do Adobe

Depois que seu contrato for atualizado para incluir a nova experiência unificada de revisão e aprovação, seu ambiente poderá conter dois tipos de objetos: objetos no armazenamento herdado do Workfront (os objetos que você tem hoje) e objetos criados usando o armazenamento em nuvem da Adobe. Em um alto nível, os dois modelos de armazenamento diferem em onde os dados residem, quais produtos da Adobe podem visualizá-los e qual funcionalidade está disponível:

|  | Objeto no armazenamento herdado do Workfront | Objeto no armazenamento em nuvem do Adobe |
|---|---|---|
| Infraestrutura de armazenamento | Somente Workfront | armazenamento em nuvem Adobe |
| Visibilidade entre produtos | Somente Workfront | Workfront, Frame.io e Creative Cloud |
| Funcionalidade | Funcionalidade herdada | Nova funcionalidade |

Os objetos criados antes do armazenamento em nuvem do Adobe ser ativado na área Configuração permanecem no armazenamento herdado do Workfront. Os novos comportamentos descritos neste artigo se aplicam apenas aos objetos de armazenamento em nuvem do Adobe que você e seus usuários criam depois que o armazenamento em nuvem do Adobe é ativado.

## O que há de diferente com o armazenamento em nuvem da Adobe

A maior alteração diária com o armazenamento em nuvem do Adobe é a nova área Documentos e o visualizador Frame.io que possibilita a revisão e a aprovação dentro dela. Há outras diferenças que afetam a maneira como você gerencia objetos, documentos e revisões.

A tabela a seguir resume as principais diferenças ao alternar para o armazenamento na nuvem da Adobe. Cada área na tabela está vinculada à seção detalhada abaixo.

| Área | O que é diferente | O que saber |
|---|---|---|
| [A nova área Documentos](#the-new-documents-area) | Uma área Documentos unificada e reprojetada substitui a área Documentos herdada. | Nenhuma área Documentos global. Acesse documentos de um programa, portfólio, projeto, tarefa ou problema. |
| [Permissões de documento](#document-permissions) | Os documentos herdam permissões do projeto, tarefa ou problema ao qual estão vinculados. | Você não pode compartilhar ou definir permissões em documentos individuais. Você gerencia todo o acesso por meio do modal Compartilhamento de objetos no Workfront, que é enviado em cascata para pastas de documentos geradas pelo sistema. |
| [Mapeamento de permissões de objeto](#object-permissions-mapping) | As permissões Gerenciar e Contribuir da Workfront são mapeadas para Editar e Compartilhar no Frame.io. Visualizar mapas para Somente comentário. | As permissões são gerenciadas no Workfront. Os usuários do Manage e do Contribute obtêm o recurso de compartilhamento externo no Frame.io. |
| [Visualizador de revisão e aprovação](#review-and-approval-viewer) | O visualizador Frame.io substitui o visualizador do Workfront Proofing. | Incluído para todos os usuários da Workfront com uma licença paga. Suporta marcação, comentários com carimbo de data e hora, histórico de versões, dispositivos móveis, formatos com mais de 40 anos e arquivos de até 500 GB. |
| [Regras de nomenclatura de objetos](#object-naming-rules) | Regras de nomenclatura rígidas se aplicam: nomes exclusivos em um portfólio ou projeto, sem caracteres especiais, sem ponto ou espaço à direita e limite de 255 caracteres. | O Workfront renomeia objetos automaticamente quando surgem conflitos. Modelos de auditoria que geram novos nomes e estrutura de projeto. |
| [Portabilidade de objeto](#object-portability) | Você pode mover, copiar e converter objetos somente entre modelos de armazenamento semelhantes. | Os objetos de armazenamento na nuvem do Adobe não podem ser movidos para projetos herdados, ou o inverso. Mover um projeto do Adobe Cloud Storage para um portfólio ou programa herdado converte o pai no Adobe Cloud Storage. |
| [Recursos não disponíveis](#capabilities-not-available-on-adobe-cloud-storage-objects) | Workfront Proof, o visualizador de documentos do Workfront, documentos favoritos e documentos de solicitação não fazem parte da experiência. | Os objetos herdados retêm esses recursos. O Workfront Proof não receberá novo investimento e será removido em uma versão futura. |
| [Cota de armazenamento](#storage-quota) | O armazenamento é agrupado para projetos herdados do Workfront e projetos do Adobe Cloud Storage. 60 GB por usuário licenciado. Sem tampa dura. | Os administradores de sistema podem visualizar o uso do armazenamento na página Informações do cliente em Configuração. |
| [Limite anual de análise de vídeo](#annual-video-review-cap) | Limite de nível organizacional para solicitações de prova de vídeo em 10% das licenças de usuário pagas do Workfront (Standard e Light). | Uma vez alcançado, nenhum novo vídeo é revisado até o próximo período anual. Notificações no aplicativo em 80% e 100%. Não se aplica a clientes do Frame.io Enterprise. |
| [Workfront Fusion](#workfront-fusion-on-adobe-cloud-storage-projects) | Os cenários de Fusão baseados em prova existentes não funcionam automaticamente em projetos de armazenamento em nuvem do Adobe. | Os cenários com escopo para projetos herdados continuam a funcionar. Cada cenário afetado obtém um dos três caminhos: editar, reconstruir ou desativar. Novos conectores esperados para o terceiro trimestre de 2026. |

### A nova área Documentos

A nova área Documentos é uma experiência de documentos unificada projetada para o armazenamento em nuvem do Adobe. Ele simplifica a navegação, consolida a atividade de revisão e aprovação e é o ponto de entrada para o visualizador Frame.io.

A área Documentos global não faz parte da nova experiência. Em projetos de armazenamento na nuvem do Adobe, você acessa documentos de um programa, portfólio, projeto, tarefa ou problema.

Para obter mais informações, consulte [A área Documentos](/help/quicksilver/documents/managing-documents/documents-area.md).

### Permissões de documento

As permissões de documento são fundamentalmente diferentes em projetos de armazenamento em nuvem do Adobe:

* Você não pode compartilhar ou definir permissões em documentos individuais. Em vez disso, as permissões são aplicadas a pastas de documentos geradas pelo sistema que contêm os documentos.
* As pastas de documentos geradas pelo sistema herdam permissões do projeto, tarefa ou problema pai.
* As subpastas herdam permissões da pasta de documentos gerada pelo sistema principal.
* Subtarefas não herdam permissões de tarefas pai. Você deve ser adicionado diretamente a uma subtarefa para acessar sua pasta de documentos gerada pelo sistema.


Para obter mais informações sobre como as permissões de documento funcionam, consulte [Visão geral sobre permissões de objeto e nível de acesso do modelo de armazenamento na nuvem do Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).


### Mapeamento de permissões de objeto

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

Gerenciar e contribuir mapear para **Editar e compartilhar** no Frame.io. Ao analisar os padrões de compartilhamento para projetos de armazenamento na nuvem do Adobe, considere se o modelo de governança ideal para os colaboradores tem os mesmos recursos de revisão que os gerentes, incluindo compartilhamento externo.

Para obter mais informações, consulte [Visão geral das permissões de objeto e do nível de acesso para o modelo de armazenamento na nuvem do Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#permission-mapping-to-frameio).


### Visualizador de revisão e aprovação

Em objetos de armazenamento na nuvem do Adobe, o visualizador Frame.io é a superfície de revisão e aprovação no lugar do Workfront Proof. O visualizador Frame.io está incluído para todos os usuários do Workfront com uma licença paga.

O visualizador Frame.io fornece:

* Ferramentas de marcação e comentários, incluindo desenho à mão livre e formas padrão, como círculos, setas e quadrados
* Comentários com carimbo de data e hora com precisão de quadro preciso para revisões de vídeo
* Histórico de versão e comparação de versão
* Acesso móvel para revisões e aprovações em qualquer lugar
* Suporte para mais de 40 formatos de arquivo, incluindo todos os tipos comuns de vídeo, imagem, áudio, PDF e Microsoft Office, com reprodução nativa para formatos de vídeo profissional, como ProRes, H.265 e DNxHD, e suporte para arquivos de até 500 GB


### Regras de nomenclatura de objeto

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


### Portabilidade do objeto

Você pode mover, copiar e converter objetos Workfront entre modelos de armazenamento semelhantes. Por exemplo, você pode mover uma tarefa de um projeto de armazenamento em nuvem do Adobe para outro projeto de armazenamento em nuvem do Adobe. Não é possível mover ou copiar uma tarefa ou problema de um projeto do Adobe Cloud Storage para um projeto herdado, ou vice-versa.

Atualmente, ao criar ou mover um projeto do Adobe Cloud Storage para um portfólio ou programa herdado, o portfólio ou programa é convertido automaticamente em um objeto do Adobe Cloud Storage. Uma versão futura dará aos administradores do sistema mais controle sobre quais objetos serão convertidos automaticamente.

### Recursos não disponíveis em objetos de armazenamento na nuvem do Adobe

Os seguintes recursos não fazem parte dos objetos de armazenamento na nuvem do Adobe:

* Workfront Proof
* O visualizador de documentos do Workfront
* Documentos favoritos
* Solicitar documentos

Os projetos herdados mantêm o acesso ao Workfront Proof e aos recursos de documento herdados listados acima. A Workfront Proof não receberá novos investimentos no futuro e será removida em uma versão futura.

### Cota de armazenamento

O armazenamento é agrupado para objetos herdados do Workfront e objetos de armazenamento na nuvem do Adobe. Cada usuário licenciado recebe 60 GB de armazenamento. Não há limite rígido para o uso de armazenamento, mas os administradores do Workfront recebem notificações por email quando o uso atinge 75%, 90% e 100% da cota.

Os administradores do sistema podem ir para **Configuração** > **Sistema** > **Informações do cliente** para exibir a cota e o uso de armazenamento atuais.

Para obter mais informações, consulte [Verificar limites de armazenamento de documentos](/help/quicksilver/documents/managing-documents/check-document-storage.md).


### Limite anual de análise de vídeo

Há um limite anual de solicitações de prova de vídeo definido em 10% do total de licenças pagas de usuário do Workfront da sua organização (Standard e Light). Esse limite é aplicado no nível da organização.

* Os administradores do Workfront recebem notificações no aplicativo quando o uso atinge 80% e 100% do limite.
* Quando o limite for atingido, você não poderá criar novas solicitações de análise de vídeo até o próximo período anual.
* Esse limite não se aplica a clientes do Frame.io Enterprise. Se sua organização analisa regularmente grandes volumes de conteúdo de vídeo, entre em contato com o representante de conta da Adobe para saber mais sobre o licenciamento Frame.io Enterprise.

Para obter mais informações, consulte as Perguntas frequentes sobre revisão e aprovação de ativos e vídeos na [Visão geral de revisão e aprovação unificada](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

### Workfront Fusion em projetos de armazenamento em nuvem do Adobe

Os cenários do Workfront Fusion existentes criados em revisões herdadas não funcionam automaticamente em projetos de armazenamento na nuvem do Adobe. Módulos específicos de prova, webhooks e endpoints de API têm equivalentes diretos em alguns casos e alterações significativas em outros. Os cenários com escopo para projetos herdados continuam a funcionar como funcionam atualmente.

Os conectores de fusão com suporte nativo para revisão e aprovação unificadas devem estar disponíveis no terceiro trimestre de 2026.

Para obter informações detalhadas sobre o impacto em tipos de cenários comuns e como classificar cada cenário como Editar, Recompilar ou Desativar com base em sua funcionalidade, consulte [Atualizar cenários do Workfront Fusion para revisão e aprovação unificadas](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).


## Escolha como o armazenamento em nuvem do Adobe é implantado

Você decide como o Adobe Cloud Storage é exibido para os usuários. Há duas configurações, e uma delas pode ser aplicada a toda a organização ou a grupos específicos da Workfront.

Para obter instruções passo a passo, consulte [Habilitar o Adobe Cloud Storage para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

* **Somente armazenamento em nuvem do Adobe**: novos projetos usam o armazenamento em nuvem do Adobe por padrão. Os usuários não podem criar projetos herdados.
* **Armazenamento em nuvem do Adobe e armazenamento herdado do Workfront**: quando os usuários criam um projeto, eles escolhem entre o armazenamento em nuvem do Adobe (rotulado como &quot;Novo projeto&quot;) e o armazenamento herdado do Workfront (rotulado &quot;Armazenamento herdado&quot;).

  ![escolher um tipo de projeto](assets/choose-project-type.png)



>[!TIP]
>
>Para colocar o armazenamento em nuvem do Adobe na frente de uma equipe menor primeiro, aplique qualquer configuração a um único grupo do Workfront. Isso permite executar um piloto direcionado antes de lançar o projeto de forma mais ampla. Recomendamos começar com uma implantação em nível de grupo para um ritmo controlado e, em seguida, expandir para toda a organização depois que o grupo piloto tiver validado a experiência.

Os objetos existentes mantêm o modelo de armazenamento com o qual foram criados. A alteração da preferência de armazenamento padrão não altera nenhum objeto existente.

## Planejar a implantação

Cada ambiente do Workfront é diferente. Antes de habilitar o Adobe Cloud Storage para seus usuários, reserve um tempo para planejar a aparência de uma implantação bem-sucedida para sua organização. As sugestões abaixo não são uma lista de verificação, mas um ponto de partida para seu próprio plano.

**1. Escolha um grupo piloto.** Uma implantação com escopo de grupo permite que você coloque o armazenamento em nuvem do Adobe na frente de uma equipe menor primeiro, colete feedback e ajuste antes de uma implantação mais ampla. Escolha um grupo cujos padrões de trabalho sejam representativos o suficiente para exibir problemas que você deseja saber antecipadamente.

**2. Comunicar a alteração aos usuários finais.** A maior alteração visível para revisores, aprovadores e proprietários de projetos é a nova área Documentos e o visualizador Frame.io que possibilita a revisão e a aprovação de projetos de armazenamento na nuvem do Adobe. Planeje a apresentação para que os usuários saibam o que esperar quando encontrarem seu primeiro projeto de armazenamento na nuvem da Adobe. O artigo [Introdução à revisão e aprovação unificadas](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md) é um ponto de partida útil para material voltado para o usuário final.

**3. Planeje a disponibilidade do conector Workfront Fusion.** Os conectores de fusão com suporte nativo para revisão e aprovação unificadas devem estar disponíveis no terceiro trimestre de 2026. Os cenários de Fusão baseados em prova existentes continuam a funcionar em projetos herdados. Antes de trazer equipes que dependem desses cenários para o piloto de armazenamento em nuvem do Adobe, decida se deve aguardar os novos conectores, recriar com base na API atual ou substituir esses cenários pelos recursos nativos de revisão e aprovação unificados.

Para obter informações detalhadas sobre o impacto em tipos de cenários comuns e como classificar cada cenário como Editar, Recompilar ou Desativar com base em sua funcionalidade, consulte [Atualizar cenários do Workfront Fusion para revisão e aprovação unificadas](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).


## Artigos relacionados

* [Visão geral do armazenamento em nuvem do Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md)
* [Habilitar o armazenamento em nuvem do Adobe para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)
* [Visão geral unificada de revisão e aprovação](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Introdução à revisão e aprovação unificadas](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [A área Documentos](/help/quicksilver/documents/managing-documents/documents-area.md)
* [Visão geral das permissões de objeto e do nível de acesso para o modelo de armazenamento em nuvem do Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)

