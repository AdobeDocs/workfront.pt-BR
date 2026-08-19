---
product-area: documents
navigation-topic: approvals
title: Transferência de aprovações de documentos herdados para Aprovações unificadas
description: Entenda o que acontece com seus fluxos de trabalho de aprovação de documento existentes quando sua organização muda para uma versão do Workfront que oferece suporte a Aprovações unificadas.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: 8f3c5ed32c6496a13703a5dce771a84462aa7f05
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 3%

---

# Transferência de aprovações de documentos herdados para Aprovações unificadas

A migração para uma versão do Workfront compatível com o Adobe Cloud Storage também move sua organização de aprovações de documentos herdados para aprovações unificadas. Este artigo fornece informações sobre qual funcionalidade estará disponível em Aprovações unificadas, bem como recomendações para administradores do Workfront que afastam os usuários das aprovações de documentos herdados.


>[!IMPORTANT]
>
>Essa alteração se aplica em toda a organização assim que você migra para uma versão do Workfront compatível com o armazenamento em nuvem da Adobe. Não há grupo piloto ou opção de implantação gradual para mudar de aprovações de documentos herdadas para aprovações unificadas.<br>
>Para obter detalhes sobre as alterações no Adobe Cloud Storage, consulte [Mover para o Workfront no Adobe Cloud Storage](/help/quicksilver/review-and-approve-work/workfront-storage.md).

## Entenda o que está mudando de aprovações de documentos herdadas para Aprovações unificadas

|  | Aprovações de documentos herdados | Aprovações unificadas |
| --- | --- | --- |
| Aprovadores e revisores | Aprovação somente por usuários individuais | Aprovação ou revisão por usuários ou equipes individuais |
| Prazos e lembretes | Nenhum lembrete automático | Lembretes automatizados de 72 horas, 24 horas e na data de vencimento |
| Estágios e caminhos de aprovação | Uma fase de aprovação, sem caminhos paralelos | [Vários estágios de aprovação e caminhos de revisão paralela](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) |
| Modelos de aprovação | Cada aprovação configurada do zero | [Modelos reutilizáveis](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md) disponíveis na Instalação do Workfront |
| Revisão e marcação | Visualizador de provas | [Visualizador de provas](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md) em objetos de armazenamento herdados do Workfront ou o [visualizador do Frame.io](/help/quicksilver/review-and-approve-work/workfront-storage.md#review-and-approval-viewer) em objetos de armazenamento na nuvem do Adobe |
| Revisão assistida por IA | Não disponível | Verificações automáticas de conformidade da marca com o [Revisor de Conteúdo](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md) |
| Relatórios | Relatórios herdados | Widgets de KPI da página inicial e [Painéis do Canvas](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md) |

### O que acontece com as aprovações já em andamento

As aprovações em andamento que foram criadas em aprovações de documentos herdados continuarão a funcionar da mesma forma que antes da atualização. No entanto, qualquer nova aprovação criada após a atualização usará Aprovações unificadas.


## Preparar para a atualização

* Compartilhe o artigo [Introdução à revisão e aprovação unificadas](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md) com seus usuários finais.
* Revise seus cenários existentes do Workfront Fusion. Se você usa aprovações de documentos herdados com comprovação, consulte [Atualizar cenários do Workfront Fusion para revisão e aprovação unificadas](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md) antes de atualizar sua organização.
* Configure um painel de revisão e aprovação nos Painéis do Canvas para substituir quaisquer relatórios de aprovação herdados. Consulte [Criar um painel de revisão e aprovação](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md) para obter detalhes.


### Artigos de ajuda para usuários finais

* [Introdução à revisão e aprovação unificadas](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [Funcionalidade disponível para aprovações de documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md)
* [Visão geral unificada de revisão e aprovação](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Revisar e aprovar com o visualizador Frame.io](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)
* [Usar recursos de aprovação unificada e revisão juntos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md)
* [Visão geral do status de decisão do documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md)
* [Introdução ao Workfront Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)