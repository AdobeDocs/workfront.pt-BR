---
product-area: documents
navigation-topic: approvals
title: Visão geral unificada de revisão e aprovação
description: Saiba mais sobre a revisão e aprovação unificadas possibilitadas pelo Workfront e Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 32cb95c2-8d12-492b-ad89-b38e2a337fc5
source-git-commit: e31242349496f61b4282dc6fd628ecf62676d370
workflow-type: tm+mt
source-wordcount: '3892'
ht-degree: 0%

---


# Visão geral unificada de revisão e aprovação

A análise e a aprovação unificadas reúnem o Adobe Workfront e o Adobe Frame.io em uma única experiência profundamente conectada, preenchendo as lacunas entre o gerenciamento de marketing, a análise criativa e a entrega de conteúdo.
Os coordenadores de projeto gerenciam o trabalho no Workfront enquanto criativos, profissionais de marketing e participantes revisam e aprovam ativos no visualizador de Frame.io de nível profissional, tudo sem mover arquivos entre ferramentas desconectadas.

![Diagrama mostrando o fluxo de trabalho unificado de revisão e aprovação, com coordenadores de projeto gerenciando o trabalho no Workfront e revisores e aprovadores fornecendo feedback e tomando decisões no visualizador Frame.io.](assets/Unified-Review-Approvals-Image.png)


## Requisitos de integração

* O Workfront e o Frame.io devem ser implantados na mesma organização do Identity Management System (IMS).

* Os usuários podem pertencer a apenas uma instância do Workfront na organização IMS.

* A instância do Workfront deve ser ativada no armazenamento corporativo da Adobe Unified Experience e do Adobe.

* A integração deve ser configurada pelo Adobe Professional Services.


## Baseado em armazenamento corporativo Adobe

A análise e a aprovação unificadas são criadas com base no armazenamento corporativo Adobe — uma solução de armazenamento em nuvem que serve como repositório central para ativos em produtos corporativos da Adobe, incluindo Workfront e Frame.io. <!--, and Creative Cloud.-->

Os principais benefícios do armazenamento corporativo da Adobe incluem:

* Camada de armazenamento unificado para ativos criativos e de gerenciamento de trabalho
* Permissões centralizadas com o Adobe Identity Management System (IMS) para controle de acesso seguro
* Visibilidade completa de ativos no Workfront e Frame.io <!--, and Creative Cloud apps -->
* Gerenciamento dimensionável de armazenamento e cotas para as necessidades corporativas

Para obter mais detalhes, consulte [visão geral do armazenamento corporativo da Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Revisão e aprovação unificadas

Com a revisão e aprovação unificadas, você pode:

* Criar e gerenciar revisões e aprovações diretamente da Workfront
* Rastrear o status de revisões e aprovações em tempo real
* Centralizar feedback e aprovações em um único local
* Garantir que todas as partes interessadas tenham acesso às versões mais recentes dos ativos
* Utilizar Revisores de IA para automatizar revisões de conformidade da marca
* e muito mais

Para obter mais informações, consulte [Aprovações de documentos unificados: índice do artigo](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md).


### Usar o visualizador do Frame.io

Use o visualizador Frame.io para revisar e aprovar ativos. O visualizador Frame.io fornece

* Ferramentas de marcação e comentários
* Histórico e comparação de versões
* Comentários com carimbo de data e hora para análises de vídeo
* Acesso móvel para revisões e aprovações em qualquer lugar

Para obter mais informações, consulte [Introdução à revisão e aprovação unificadas](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

#### Limites de análise de vídeo

Há um limite anual para solicitações de prova de vídeo definido em 10% do total de licenças pagas de usuário da Workfront de uma organização: Standard e Light. Esse limite é aplicado no nível da organização.

Os administradores do Workfront recebem notificações quando o uso atinge 80% e 100% do limite.

Esse limite não se aplica a clientes do Frame.io Enterprise.

#### Tipos de arquivo compatíveis no visualizador Frame.io

O visualizador Frame.io suporta todos os tipos comuns de vídeo, imagem, áudio, PDF e MS® Office. Para obter uma lista detalhada dos arquivos suportados, consulte [Tipos de arquivos suportados no Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Acesso e licenciamento para o visualizador Frame.io

O visualizador Frame.io é o visualizador padrão para todos os fluxos de trabalho de revisão e aprovação do Workfront. Ele é incluído automaticamente para todos os usuários do Workfront com uma licença paga. Nenhuma licença adicional do Frame.io é necessária para usar o visualizador do Frame.io para revisões e aprovações.

Se sua organização quiser aproveitar a funcionalidade adicional do Frame.io disponível com essa integração, como carregar ativos diretamente para projetos no Frame.io, você pode comprar uma licença do Frame.io Enterprise. Entre em contato com seu representante de conta da Adobe para agendar uma demonstração e explorar os benefícios da solução Frame.io completa.

A funcionalidade Workfront Proofing não está disponível com essa integração.

## Gerenciamento eficiente de projetos no Workfront

Os coordenadores de projetos podem aproveitar os poderosos recursos de gerenciamento de projetos da Workfront para planejar, acompanhar e gerenciar trabalho.

Para obter mais informações sobre como gerenciar projetos no Workfront, consulte [Projetos: índice do artigo](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

### Convenções de nomenclatura e estrutura impostas

Como a revisão e a aprovação unificadas são criadas usando o armazenamento corporativo Adobe, há algumas convenções de estrutura e nomenclatura aplicadas que devem ser levadas em conta ao gerenciar projetos e documentos.

* Os nomes dos objetos devem ser exclusivos e não podem ser duplicados.
* O armazenamento corporativo do Adobe requer nomes exclusivos para objetos de mesmo nível com o mesmo pai na árvore hierárquica.
* Documentos não podem ter o mesmo nome se pertencerem ao mesmo projeto.
* Os nomes de objetos não podem conter nenhum dos seguintes caracteres especiais: \ / : * ? &quot; | &lt; >
* Os nomes de objetos são limitados a no máximo 255 caracteres.

Com essas limitações em mente, o Workfront renomeia automaticamente objetos ou documentos conforme necessário para evitar conflitos.

### Compartilhamento e permissões

Como parte da integração, as permissões do usuário são controladas no Workfront e fluem para o Frame.io. Isso significa que não é possível convidar um usuário para um projeto no Frame.io ou modificar permissões de usuário no Frame.io. Essas ações precisam ser feitas por meio do modal Compartilhamento de projetos no Workfront.

A tabela a seguir mostra como as permissões do Workfront são mapeadas para permissões de Frame.io:

<table>
<tr>
<th>Permissão de usuário do Workfront</th>
<th>Permissão de usuário do Frame.io</th>
</tr>
<tr>
<td>Gerenciar</td>
<td>Editar e compartilhar</td>
</tr>
<tr>
<td>Contribuir</td>
<td>Editar e compartilhar</td>
</tr>
<tr>
<td>Exibir</td>
<td>Somente comentário</td>
</tr>
</table>



### Gerenciamento de documentos no Workfront

Os documentos carregados no Workfront são armazenados no armazenamento corporativo do Adobe e podem ser acessados no Workfront e no Frame.io. Ao fazer upload de um documento para uma tarefa ou problema no Workfront, uma pasta gerada pelo sistema é criada no Adobe Enterprise Storage que herda permissões da tarefa ou problema. Todos os documentos carregados para essa tarefa ou problema são armazenados nessa pasta e herdam permissões dela. Para obter mais informações sobre documentos no Workfront, consulte [A visão geral da nova área de documentos](/help/quicksilver/documents/managing-documents/documents-area.md) e [Visão geral das permissões de objeto e do nível de acesso para o modelo de armazenamento corporativo do Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

### Limitações da experiência de documento

Os seguintes recursos do documento não estão incluídos:

<!--* External document providers-->
* Acesso à revisão no Workfront
* Visualizador de documentos no Workfront
* Documentos favoritos
* Solicitar documentos

## Introdução à revisão e aprovação unificadas

Para começar a revisão e aprovação unificadas, consulte [Introdução à revisão e aprovação unificadas](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

## Perguntas frequentes

### Introdução à revisão e aprovação unificadas

+++ Expanda para visualizar as perguntas frequentes para começar a revisão e aprovação unificadas.

**O que é revisão e aprovação unificadas?**

A revisão e aprovação unificadas é uma integração nativa entre o Adobe Workfront e o Adobe Frame.io que reúne o gerenciamento de trabalho e a revisão criativa em um único sistema conectado. Os coordenadores de projeto planejam e rastreiam o trabalho no Workfront, enquanto os revisores e aprovadores usam o visualizador de Frame.io de nível profissional para fornecer feedback, marcar ativos e tomar decisões de aprovação, sem alternar entre ferramentas separadas ou mover arquivos manualmente.

A análise e a aprovação estão no centro de cada operação de conteúdo. É onde o trabalho criativo, a participação das partes interessadas e as decisões empresariais convergem. Quando esse processo é distribuído entre ferramentas desconectadas (threads de email, mensagens de chat, marcações de captura de tela), as consequências se agravam: tempo de entrada no mercado mais lento, perda de feedback, confusão de versão e tempo gasto gerenciando arquivos em vez de criar conteúdo.

A revisão e aprovação unificadas aborda isso substituindo a colcha de retalhos de ferramentas de revisão desconectadas por um sistema moderno — uma única fonte de verdade que vive onde o trabalho já acontece.

**Quais são os requisitos para usar esta integração?**

Para usar a revisão e aprovação unificadas, as seguintes condições devem ser atendidas:

* O Workfront e o Frame.io devem ser implantados na mesma organização do Adobe Identity Management System (IMS).

* Os usuários podem pertencer a apenas uma instância do Workfront na organização IMS.

* A instância do Workfront deve ser ativada no armazenamento corporativo da Adobe Unified Experience e do Adobe.

* A integração deve ser configurada pelo Adobe Professional Services.

* Os clientes da Workfront devem estar em uma SKU V2 (isso pode exigir um evento de contratação — entre em contato com o representante de conta da Adobe).

**Preciso de uma licença Frame.io para usar esta integração?**

Não. O visualizador Frame.io é incluído automaticamente para todos os usuários do Workfront com uma licença paga sem custo adicional. Você não precisa de uma licença Frame.io separada para revisar e aprovar ativos por meio do Workfront.

Se a sua organização quiser acessar recursos adicionais do Frame.io, como fazer upload de ativos diretamente em projetos no Frame.io, você poderá comprar uma licença do Frame.io Enterprise. Entre em contato com o representante de conta da Adobe para obter mais informações.

**Isso substitui o Workfront Proof?**

Sim. Quando a revisão e aprovação unificadas são ativadas, o visualizador Frame.io se torna a superfície de revisão principal no Workfront, substituindo o Workfront Proof.

Os clientes existentes manterão acesso à funcionalidade de provas do Workfront para todos os projetos criados antes da integração ser habilitada.

**Como faço para obter acesso à Revisão e Aprovação Unificadas?**

**O que preciso fazer para obter acesso?**

Para acessar a revisão e aprovação unificadas, sua organização deve estar em uma SKU Workfront V2. Se você não estiver atualmente em uma SKU V2, será necessário um evento de contratação com a Adobe. Para começar:

* Entre em contato com seu representante de conta da Adobe para confirmar se seu plano atual da Workfront oferece suporte à revisão e aprovação unificadas.

* Se for necessária uma atualização do SKU, seu representante de conta o guiará pelo processo de contratação.

* Assim que sua conta estiver na SKU correta, a Adobe Professional Services configurará a integração para sua organização.

   * Se não tiver certeza de quem é o representante de conta da Adobe, entre em contato com o portal de suporte da Adobe ou visite o Experience League para obter opções de contato.

+++

### Como a revisão e a aprovação unificadas funcionam

+++ Expanda para visualizar as perguntas frequentes sobre como a revisão e a aprovação unificadas funcionam.

**Como funciona o fluxo de trabalho de revisão e aprovação?**

O workflow segue estas etapas gerais:

1. Um coordenador de projeto cria um projeto no Workfront e carrega ou vincula ativos.

1. Quando um ativo está pronto para revisão, o coordenador cria um fluxo de trabalho de aprovação, seja uma aprovação de uso único ou aplicando um modelo de aprovação reutilizável.

1. Os revisores e aprovadores atribuídos são notificados por email e podem abrir o ativo diretamente no visualizador Frame.io.

1. Os revisores podem adicionar comentários e marcação. Os aprovadores devem tomar uma decisão formal.

1. O coordenador rastreia o status em tempo real do Workfront.

**Qual é a diferença entre um revisor e um aprovador?**

Os revisores podem adicionar comentários e marcar ativos no visualizador Frame.io. Quando terminam, marcam sua revisão como concluída. No entanto, a ação não é necessária para que o fluxo de trabalho de aprovação avance.

Para avançar o fluxo de trabalho de aprovação, os aprovadores devem tomar uma das seguintes decisões:

* **Aprovar**: o ativo está pronto para ser usado como está.

* **Precisa trabalhar**: o ativo requer alterações e deve ser reenviado como uma nova versão para reaprovação.

**Que tipos de fluxos de trabalho de aprovação posso criar?**

* **Aprovações de uso único**: você pode criar uma aprovação de uso único diretamente em um documento em um projeto, tarefa ou problema. Atribua revisores e aprovadores, defina prazos e configure vários estágios, se necessário. Os lembretes de email automatizados são enviados 72 horas antes, 24 horas antes e dentro do prazo.

* **Modelos de aprovação**: você pode criar modelos reutilizáveis na Instalação do Workfront. Um modelo define os revisores, aprovadores e um período de conclusão relativo. Você pode criar vários estágios, se necessário. Depois que um modelo é aplicado a um ativo, o prazo é calculado automaticamente.

**Como os usuários externos participam das revisões?**

Os usuários externos do Workfront são notificados por email quando são atribuídos a uma revisão ou aprovação. Eles serão solicitados a criar um logon Frame.io para acessar o visualizador e participar do processo de revisão.

**Como rastrear o progresso da revisão e da aprovação?**

Os coordenadores de projetos podem monitorar todas as aprovações em andamento de várias maneiras:

* O widget Minhas aprovações na área Página inicial do Workfront fornece um resumo em tempo real das aprovações pendentes e vencidas.

* O widget Métricas de aprovação de documento exibe os tempos médios de aprovação e detalhamentos de decisão.

* Painéis de relatório personalizados podem ser criados nos Painéis do Canvas para maior visibilidade sobre as atividades de revisão e aprovação.

+++


### Revisar e aprovar ativos e vídeos

+++ Expanda para visualizar as perguntas frequentes sobre revisão e aprovação de ativos e vídeos.

**Há limites para as análises de vídeo?**

Sim. Há um limite anual de solicitações de prova de vídeo definido em 10% do total de licenças pagas de usuário do Workfront da sua organização (Standard e Light). Esse limite se aplica no nível da organização.

Os administradores do Workfront receberão notificações no aplicativo quando o uso atingir 80% e 100% do limite.

Esse limite não se aplica a clientes do Frame.io Enterprise. Se sua organização analisa regularmente grandes volumes de conteúdo de vídeo, entre em contato com o representante de conta da Adobe para saber mais sobre o licenciamento Frame.io Enterprise.

**O mesmo usuário pode aparecer em vários estágios de um fluxo de trabalho de aprovação?**

Sim. Um usuário pode ser atribuído a vários estágios no mesmo fluxo de trabalho de aprovação.

**É possível adicionar estágios para criar um fluxo de trabalho de aprovação de vários estágios?**

Sim. Os workflows de aprovação em vários estágios são compatíveis, permitindo rotear ativos por meio de rodadas sequenciais de revisão e aprovação com diferentes participantes em cada estágio.

<!--
**Can I modify the trigger for a later stage---for example, based on all approved versus the due date ending?**

Stages in a multi-stage approval workflow proceed sequentially based on all required decisions being made in the current stage. When all assigned approvers in a stage have made their decisions, the next stage begins and the previous stage is locked. There is no option to trigger a stage based on the due date ending. If the "One decision required" toggle is enabled on a stage, the first approver decision completes that stage and advances the workflow.

**Can I remove the due date from an approval?**

Yes. Due dates are optional for both single-use approvals and approval templates. When creating a single-use approval, you can leave the deadline field empty. For approval templates, the relative completion timeframe is also optional.

**Can I change the default due date on new approval templates?**

Yes. When creating or editing an approval template, the timeframe (or "Workdays until due date" for multi-stage templates) can be adjusted per stage or left empty. The deadline is calculated automatically from this timeframe when the template is applied to an asset, so updating the template changes the default for all future approvals that use it.

**What happens when the deadline is reached for a review stage?**

For both single-stage and multi-stage reviews, automated reminder emails are sent at 72 hours, 24 hours, and on the deadline. However, reaching the deadline does not automatically reject the asset, lock the stage, or advance the workflow. Approvers and reviewers can still make decisions or complete their review after the deadline has passed. In a multi-stage workflow, each stage has its own independent deadline, and stages still advance based on all required decisions being made---not based on the deadline.
-->

**Os modelos de aprovação podem incluir grupos ou equipes, ou apenas usuários individuais?**

Atualmente, os modelos de aprovação oferecem suporte a usuários e equipes individuais.

**Os aprovadores são notificados por email quando têm algo para revisar?**

Sim. Os aprovadores e revisores recebem notificações por email quando são atribuídos a uma revisão ou aprovação. Os emails de lembrete automatizados também são enviados 72 horas antes do prazo, 24 horas antes e no próprio prazo.

A capacidade de personalizar mensagens de notificação por email não está disponível no momento, mas está no roteiro do produto.

<!--
**Can I change the notification frequency for a unified approver or reviewer (for example, all comments, replies to my comments, or daily summaries)?**

No. Notification frequency settings such as receiving all comments, only replies to your comments, or daily digest summaries are not currently available for unified review and approval. The system sends email notifications automatically when a user is assigned as a reviewer or approver, and automated reminder emails are sent at 72 hours, 24 hours, and on the deadline. The ability to customize notification messages and frequency is on the product roadmap.
-->

**Posso manter um estágio de revisão privado de outros participantes?**

No momento, não há nenhum recurso de estágio privado. Para manter uma revisão privada de outros participantes, a abordagem recomendada é criar uma cópia separada do ativo especificamente para esse grupo de revisão. Atualmente, os comentários não são segmentados por grupo de participantes em um único ativo.

Observe que o histórico de versões, incluindo versões anteriores e atuais, está sempre visível para qualquer pessoa com acesso para visualizar esse ativo.

**Os comentários podem ser marcados como resolvidos?**

Sim. Os comentários podem ser marcados como resolvidos no visualizador Frame.io.

**Que ferramentas de marcação e anotação estão disponíveis no visualizador Frame.io?**

O visualizador Frame.io inclui um conjunto completo de ferramentas de marcação visual, incluindo desenho à mão livre e formas padrão, como círculos, setas e quadrados. Para ativos de vídeo, os comentários recebem carimbo de data e hora com precisão de quadro, de modo que o feedback é sempre vinculado ao momento exato no clipe e não apenas ao carimbo de data e hora geral.

**Os comentários feitos no visualizador Frame.io aparecerão no projeto Workfront?**

Comentários e anotações permanecem no visualizador Frame.io para que mantenham seu contexto completo, incluindo carimbos de data e hora e marcações visuais. Isso pode evoluir em versões futuras.

**É possível adicionar comentários a uma versão baixada de um ativo (por exemplo, uma PDF)?**

No momento, isso não é compatível, mas é um recurso solicitado com frequência que está sendo considerado para uma versão futura.

**Posso revisar vários ativos juntos como um grupo?**

As opções aprimoradas de revisão em massa serão disponibilizadas em breve. Enquanto isso, ativos de diferentes tipos de arquivos, como um vídeo e um documento do Word, podem ser incluídos juntos em uma revisão de ativo agrupada.

**A revisão e aprovação unificadas são apenas para vídeo ou são compatíveis com outros tipos de arquivos?**

A análise e a aprovação unificadas foram projetadas para todos os tipos de ativos, não apenas para vídeo. O visualizador do Frame.io foi significativamente atualizado para suportar imagens, documentos, PDFs e outros formatos de arquivo comuns, além do vídeo.

Para obter uma lista completa dos tipos de arquivos compatíveis, consulte a documentação dos tipos de arquivos suportados Frame.io no Experience League.

**É possível compartilhar ativos externamente com participantes que não têm acesso ao Workfront?**

Sim. O Assets pode ser compartilhado externamente. Os usuários externos são notificados por e-mail e serão solicitados a criar um login no Frame.io para acessar o visualizador e participar da revisão.

<!--
**Before unified review and approval, is a reviewer just directed to a proof?**

Yes. In the legacy proofing workflow (prior to unified review and approval), when a user was assigned as a reviewer they were directed to the Workfront Proof viewer (ProofHQ) to review the proof. With unified review and approval, reviewers are instead directed to the Frame.io viewer, which replaces the Workfront Proof viewer as the primary review surface.

**When I upload a document and not a proof, a proof gets generated. Will a proof always be generated?**

No. With unified review and approval enabled and Adobe enterprise storage active, uploading a document does not automatically generate a proof. Documents are stored in Adobe enterprise storage and are reviewed using the Frame.io viewer. A proof is only generated if you explicitly create one using the legacy proofing workflow. The Frame.io viewer serves as the primary review surface, so a separate proof is not needed for standard review and approval workflows.

**What is the difference between uploading a document and a proof after the 26.2 release?**

With unified review and approval enabled, uploading a document stores it in Adobe enterprise storage and makes it available for review in the Frame.io viewer. A unified approval workflow can be created directly on the document. Uploading a proof, by contrast, uses the legacy Workfront Proof viewer (ProofHQ) and its own proofing workflow. Both options are available for projects created before the integration was enabled, but the Frame.io viewer is the primary review surface going forward. The key difference is that a document uses the unified approval workflow and Frame.io viewer, while a proof uses the legacy proofing workflow and viewer.

**Reviews under My Approvals only show a "Complete my review" button and no link to the proofing viewer or the document. Is this intended?**

For unified review and approval, the My Approvals widget provides an "Open review" button that opens the asset in the Frame.io viewer, as well as action buttons to approve, request changes, or complete a review. Reviewers can complete their review directly from the widget. If you are only seeing a "Complete my review" button without a link to the viewer, this may reflect the reviewer role behavior---reviewers are not required to open the asset to mark their review as complete, though they can choose to open it in the Frame.io viewer to provide feedback before completing.

**Before unified review and approval, if a user is both an approver in a document approval and a reviewer/approver on a proof, both show up in the proof window. How do these work together?**

When using unified approvals alongside legacy proofing on the same document, the two workflows operate independently. Document approval participants are shown in the Document Summary panel, while proof participants are shown in the proofing workflow. The SOCD (Sent, Opened, Comment, Decision) indicators in the document list are proofing-related and do not reflect the unified approval decision status. These two workflows do not automatically sync---a decision made in one does not carry over to the other.

**If you upload a new version, the document approval users do not get repopulated. Is that intended?**

Yes. When a new version is uploaded, previous approval participants are not automatically repopulated. The previous version's approval process is closed and any outstanding approvals are marked as "Withdrawn." The document owner must manually add participants to the new version's approval workflow. An "Add all" button is available to quickly repopulate all participants from the previous version, and you can also selectively add previous participants or add new ones.
-->

+++

### Gerenciamento de arquivos e armazenamento

+++ Expanda para exibir as perguntas frequentes sobre armazenamento e gerenciamento de arquivos.

**O que é armazenamento corporativo Adobe e como ele se relaciona a essa integração?**

O armazenamento corporativo da Adobe é a camada de armazenamento comum que conecta o Workfront, Frame.io e Adobe Creative Cloud. O Assets fica em um único local e pode ser acessado por meio de ferramentas sem transferências manuais de arquivos. Os recursos de criação podem funcionar no local e os revisores sempre veem a versão mais recente.

Os principais benefícios do armazenamento corporativo da Adobe incluem:

* Uma única camada de armazenamento para todos os ativos de trabalho em andamento no Workfront e no Frame.io

* Controle de acesso centralizado gerenciado pelo Adobe Identity Management System (IMS)

* Visibilidade completa de ativos — sem perda de versão e de metadados

* Gerenciamento de armazenamento dimensionável de nível empresarial

**Há requisitos de nomenclatura ou estrutura para arquivos e projetos?**

Sim. Como a integração usa o armazenamento corporativo Adobe, as seguintes convenções se aplicam:

* Os nomes de objetos e documentos devem ser exclusivos dentro do mesmo pai na hierarquia de pastas.

* Documentos dentro do mesmo projeto não podem compartilhar um nome.

* Programas, portfólios, projetos, modelos, tarefas, problemas, documentos, pastas de documentos não podem conter os seguintes caracteres especiais: `\\ / : \* ? \" \| \< \>` e são limitados a 255 caracteres.

O Workfront renomeia automaticamente objetos ou documentos conforme necessário para evitar conflitos.

**Que tipos de arquivos são suportados no visualizador Frame.io?**

O visualizador Frame.io suporta mais de 40 formatos de arquivo, incluindo todos os tipos comuns de vídeo, imagem, áudio, PDF e Microsoft Office. O suporte de vídeo inclui reprodução nativa para formatos profissionais, como ProRes, H.265 e DNxHD, com suporte para arquivos de até 500 GB.

O Frame.io foi criado especificamente para revisão criativa, o que significa que ele lida com a gama completa de tipos de ativos com os quais as equipes de marketing e criativas trabalham.

+++

### Permissões e acesso

+++ Expanda para exibir as perguntas frequentes sobre permissões e acesso.

**Como as permissões de usuário são gerenciadas?**

As permissões do usuário são definidas e controladas no Workfront e fluem automaticamente para o Frame.io. Não é possível convidar usuários ou modificar permissões diretamente no Frame.io para essa integração. Todo o gerenciamento de acesso deve ser feito usando o modal de compartilhamento de projeto no Workfront.

A tabela abaixo mostra como as permissões do Workfront são mapeadas para permissões de Frame.io:

<table>
  <thead>
    <tr>
      <th>Permissão do Workfront</th>
      <th>Permissão Frame.io</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Gerenciar</td>
      <td>Editar e compartilhar</td>
    </tr>
    <tr>
      <td>Contribuir</td>
      <td>Editar e compartilhar</td>
    </tr>
    <tr>
      <td>Exibir</td>
      <td>Somente comentário</td>
    </tr>
  </tbody>
</table>

+++


### Integrações e recursos avançados

+++ Expanda para exibir as perguntas frequentes sobre integrações e recursos avançados.

**Como isso afeta as integrações existentes de plug-ins do Creative Cloud com o Adobe Express e o GenStudio?**

As integrações que oferecem suporte à experiência de visualizador Frame.io estão atualmente em desenvolvimento para o Marketing de desempenho do Adobe Express e do GenStudio. As novas integrações serão criadas no mesmo sistema unificado de revisão e aprovação, de modo que aproveitarão o visualizador Frame.io para obter uma experiência de revisão consistente em todos os três produtos.

**O Frame.io está integrado no Workfront ou os usuários navegam para uma interface separada?**

Os usuários podem iniciar o visualizador Frame.io diretamente do Workfront. Todas as atividades de revisão e aprovação ocorrem no visualizador Frame.io e são sincronizadas automaticamente com o Workfront.

**Posso enviar ativos aprovados para o Adobe Experience Manager (AEM)?**

Sim. Depois que um ativo conclui o ciclo de revisão e aprovação, você pode transferi-lo para a Adobe Experience Manager Assets para armazenamento e distribuição finais. Isso conecta o Workfront para gerenciamento de trabalho, Frame.io para revisão e AEM para gerenciamento de ativos digitais em um supply chain de conteúdo unificado.

Para obter mais informações, consulte. Para obter mais informações, consulte [Usar o Adobe Experience Manager com a integração do Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

**Como a revisão e aprovação unificadas se encaixam no Adobe GenStudio?**

A análise e a aprovação unificadas são um componente fundamental do Adobe GenStudio — a visão mais ampla da Adobe para um supply chain de conteúdo conectado. O GenStudio conecta o Workfront, Frame.io, Creative Cloud, Adobe Express, Adobe Experience Manager Assets e GenStudio for Performance Marketing em um fluxo de trabalho unificado, desde o resumo da campanha até a entrega de conteúdo.

Dentro desse ecossistema, a análise e a aprovação servem como ponto de transferência crítico entre a criação e o delivery. É onde o trabalho criativo encontra os contributos das partes interessadas, a qualidade é validada e o conteúdo é limpo para publicação. Quando a entrega é rápida, visível e confiável, ela libera velocidade em todo o supply chain de conteúdo — a IA pode acelerar a criação, a automação pode lidar com a distribuição, mas um gargalo na revisão limita os ganhos de ambos os lados. Conectar o Workfront e o Frame.io remove esse gargalo.

**Qual é o recurso de Revisor de IA?**

A revisão e aprovação unificadas incluem um recurso de Revisor de IA que automatiza as verificações de conformidade da marca como parte do processo de revisão. O Revisor de IA pode avaliar os ativos em relação às diretrizes da marca e sinalizar possíveis problemas antes que os revisores humanos estejam envolvidos, ajudando as equipes a detectar problemas mais cedo e a se mover mais rápido.

Para obter mais informações sobre como configurar e usar o AI Reviewer, consulte a documentação do Workfront no Experience League.

+++

### Contratos, SKUs e armazenamento

+++ Expanda para visualizar as perguntas frequentes sobre contratos, SKUs e armazenamento.

**Quando a revisão e aprovação unificadas estarão disponíveis para mim?**

A revisão e aprovação unificadas estão disponíveis agora. O Access exige uma atualização para um SKU do Workfront V2. Se seu contrato foi assinado antes dos SKUs V2 estarem disponíveis, você poderá obter acesso de uma das duas formas a seguir:

* Na renovação: o acesso será ativado na próxima data de renovação do contrato.

* Recontrato antecipado: sua equipe de conta da Adobe pode recontratar você antecipadamente para adicionar os novos direitos de SKU, mantendo a data de término do contrato existente. Não há aumento de preço ao mudar para um pacote equivalente.

Entre em contato com seu representante de conta da Adobe para determinar o melhor caminho para sua organização.

<!--
**Before we sign the contract, what changes will we see in Workfront?**

Before signing the V2 SKU contract, your Workfront instance will continue to operate using the existing document and proofing experience. No unified review and approval features---such as the Frame.io viewer, Adobe enterprise storage, or multi-stage approval templates---will be available until the V2 SKU is contracted and Adobe Professional Services configures the integration for your organization.
-->

**A atualização para o V2 SKU oferece mais armazenamento?**

Sim. Com o SKU V2, cada usuário licenciado recebe 60 GB de armazenamento, antes 30 GB na versão anterior.

**Como escolher entre o armazenamento corporativo da Adobe e o armazenamento herdado do Workfront?**

O armazenamento corporativo permite a experiência do visualizador Frame.io e é necessário para análise e aprovação unificadas. O Armazenamento herdado continua usando o visualizador do Workfront Proof (ProofHQ) como padrão.

Se sua organização tiver uma combinação de workflows simples e workflows de prova mais complexos, você poderá priorizar quais workflows migrar primeiro.

O armazenamento corporativo oferece flexibilidade para implantar a nova experiência de forma incremental, começando pelos fluxos de trabalho que mais se beneficiarão.

**Como as licenças do Frame.io são gerenciadas?**

Após assinar o SKU V2, todos os usuários do Workfront terão acesso ao visualizador do Frame.io para fluxos de trabalho de revisão e aprovação — nenhuma licença separada do Frame.io Enterprise é necessária para isso.

Se sua organização precisar de recursos adicionais do Frame.io Enterprise, como

* Marcas d&#39;água avançadas (dinâmica e forense)
* Gerenciamento de direitos digitais com exclusão automática de ativos
* Credenciais de conteúdo para conteúdo gerado pela IA
* Metadados criativos personalizados
* Integrações da câmera com a nuvem
* Seu próprio espaço de trabalho para trabalho criativo em andamento

você pode trabalhar com a equipe de conta da Adobe para determinar o número apropriado de licenças Frame.io Enterprise. Todas as licenças são gerenciadas por meio da Adobe Admin Console.

+++

### Sandbox e implantação

+++ Expandir para exibir as perguntas frequentes sobre sandbox e implantação.

**Posso testar a revisão e aprovação unificadas em um ambiente de sandbox?**

Parcialmente. Os fluxos de trabalho de aprovação podem ser testados em um ambiente de sandbox da Workfront. No entanto, a experiência do visualizador Frame.io não está disponível na sandbox. O teste da própria superfície de revisão requer um ambiente de produção.

Para limitar a exposição durante a implantação, você pode habilitar a revisão e a aprovação unificadas para um grupo específico no ambiente de produção do Workfront. Isso permite executar um piloto direcionado com um conjunto menor de usuários antes de lançar o de forma mais ampla.

<!--
**How should we test future quarterly releases involving unified review and approval if the Frame.io viewer is not available in sandbox?**

Because the Frame.io viewer experience is not available in the Workfront sandbox environment, testing future quarterly releases should be done using a controlled pilot group in your production environment. You can enable unified review and approval for a specific group within your Workfront production instance, allowing a smaller set of users to validate new features as they release. Approval workflow configuration and template setup can still be tested in sandbox, but the full review experience---including the Frame.io viewer---must be validated in production.
-->

+++

### Provas interativas e HTML

+++ Expanda para visualizar as perguntas frequentes sobre provas interativas e o HTML.

**A revisão unificada e a aprovação suportam provas interativas ou URLs do HTML?**

Atualmente, os arquivos Zip HTML são compatíveis com a revisão interativa. O suporte a URLs do HTML (revisão ao vivo do URL na Web) está no roteiro e será previsto para o terceiro trimestre.

Verifique as notas de versão do Workfront no Experience League para obter atualizações.

+++

### Fusão e automação

+++ Expanda para visualizar as perguntas frequentes sobre o Fusion e a automação.

**Preciso do Workfront Fusion para usar a revisão e aprovação unificadas?**

Não. A revisão e a aprovação unificadas são uma integração nativa de produto e não exigem o Fusion. O fluxo de trabalho é incorporado diretamente ao Workfront.

**Os conectores do Fusion estarão disponíveis para revisão e aprovação unificadas?**

Sim. As ações de fusão para a revisão e aprovação unificadas estão atualmente em desenvolvimento e deverão estar disponíveis no terceiro trimestre. Verifique as notas de versão do Workfront no Experience League para obter as atualizações que estiverem disponíveis.

**O Fusion pode ser usado para disparar automaticamente uma revisão quando um documento é carregado?**

Sim. Esse tipo de automação é possível usando webhooks do Workfront em combinação com o Fusion.

**Como os workflows de Fusão existentes criados no Workfront Proof serão afetados?**

O impacto varia dependendo de como cada workflow é criado. Em geral:

* **Editar ou atualizar**: fluxos de trabalho nos quais a ação relacionada à prova existente tem um equivalente direto em aprovações unificadas podem ser atualizados para usar a nova ação.

* **Recompilar**: fluxos de trabalho nos quais as etapas subjacentes foram alteradas significativamente ou nos quais existem novos recursos, talvez precisem ser recompilados do zero.

Uma imagem mais clara surgirá assim que as APIs do Fusion para aprovações unificadas estiverem disponíveis. É recomendável auditar seus workflows existentes do Fusion e avaliá-los em relação aos novos recursos de aprovações unificadas nesse momento.

+++






