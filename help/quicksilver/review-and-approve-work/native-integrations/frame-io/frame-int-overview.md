---
product-area: documents
navigation-topic: approvals
title: Visão geral unificada de revisão e aprovação
description: Saiba mais sobre a revisão unificada e aprovações possibilitadas pelo Workfront e Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: b5f0150b-40b5-4386-98bc-374e7ca65b74
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 2b3e2ac00126facab9cc45ba8fb193d8951a37ec
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# Visão geral unificada de revisão e aprovação

A revisão e as aprovações unificadas possibilitadas pelo Workfront e Frame.io permitem que os coordenadores de projetos gerenciem projetos e planejem o trabalho no Workfront, enquanto os criadores, profissionais de marketing e partes interessadas podem revisar e aprovar ativos no Frame.io.

## Requisitos de integração

* O Workfront e o Frame.io devem ser implantados na mesma organização do Identity Management System (IMS).

* Os usuários podem pertencer a apenas uma instância do Workfront na organização IMS.

* A instância do Workfront deve ser ativada no armazenamento corporativo da Adobe Unified Experience e do Adobe.

* A integração deve ser configurada pelo Adobe Professional Services.


## Baseado em armazenamento corporativo Adobe

A análise e as aprovações unificadas são criadas com base no armazenamento corporativo Adobe — uma solução de armazenamento em nuvem que serve como repositório central para ativos em produtos corporativos da Adobe, incluindo Workfront e Frame.io. <!--, and Creative Cloud.-->

Os principais benefícios do armazenamento corporativo da Adobe incluem:

* Camada de armazenamento unificado para ativos criativos e de gerenciamento de trabalho
* Permissões centralizadas via Adobe Identity Management system (IMS) para controle de acesso seguro
* Visibilidade completa de ativos no Workfront e Frame.io <!--, and Creative Cloud apps -->
* Gerenciamento dimensionável de armazenamento e cotas para as necessidades corporativas

Para obter mais detalhes, consulte [visão geral do armazenamento corporativo da Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Revisão e aprovação unificadas

Com a revisão e as aprovações unificadas, você pode:

* Criar e gerenciar revisões e aprovações diretamente da Workfront
* Rastrear o status de revisões e aprovações em tempo real
* Centralizar feedback e aprovações em um único local
* Garantir que todas as partes interessadas tenham acesso às versões mais recentes dos ativos
* Utilizar revisores de conteúdo para automatizar as revisões de conformidade da marca
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

Os administradores do Workfront receberão notificações quando o uso atingir 80% e 100% do limite.

Esse limite não se aplica a clientes do Frame.io Enterprise.

#### Tipos de arquivo compatíveis no visualizador Frame.io

O visualizador Frame.io suporta todos os tipos comuns de vídeo, imagem, áudio, PDF e MS® Office. Para obter uma lista detalhada dos arquivos suportados, consulte [Tipos de arquivos suportados no Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Acesso e licenciamento para o visualizador Frame.io

O visualizador Frame.io é o visualizador padrão para todos os fluxos de trabalho de revisão e aprovação do Workfront. Ele é incluído automaticamente para todos os usuários do Workfront com uma licença paga. Nenhuma licença adicional do Frame.io é necessária para usar o visualizador do Frame.io para revisões e aprovações.

Se a sua organização quiser aproveitar a funcionalidade adicional do Frame.io disponível com essa integração, como carregar ativos diretamente para projetos no Frame.io, você pode comprar uma licença corporativa do Frame.io. Entre em contato com seu representante de conta da Adobe para agendar uma demonstração e explorar os benefícios da solução Frame.io completa.

A funcionalidade Workfront Proofing não está disponível com essa integração.

## Gerenciamento eficiente de projetos no Workfront

Os coordenadores de projetos podem aproveitar os poderosos recursos de gerenciamento de projetos da Workfront para planejar, acompanhar e gerenciar trabalho.

Para obter mais informações sobre como gerenciar projetos no Workfront, consulte [Projetos: índice do artigo](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

### Convenções de nomenclatura e estrutura impostas

Como a revisão e as aprovações unificadas são criadas usando o armazenamento corporativo Adobe, há algumas convenções de estrutura e nomenclatura aplicadas que devem ser levadas em conta ao gerenciar projetos e documentos.

* Os nomes dos objetos devem ser exclusivos e não podem ser duplicados
* O armazenamento corporativo da Adobe requer nomes exclusivos para objetos de mesmo nível com o mesmo pai na árvore hierárquica
* Os documentos não podem ter o mesmo nome se pertencerem ao mesmo projeto
* Os nomes de documento não podem conter nenhum dos seguintes caracteres especiais: \ / : * ? &quot; | &lt; >
* Os nomes de documentos são limitados a no máximo 255 caracteres

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

Os seguintes recursos do documento não devem ser incluídos:

<!--* External document providers-->
* Acesso à revisão no Workfront
* Visualizador de documentos no Workfront
* Documentos favoritos
* Solicitar documentos