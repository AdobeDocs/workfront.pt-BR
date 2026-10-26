---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: Planejar a implantação do armazenamento em nuvem do Adobe
description: Escolha como o armazenamento em nuvem do Adobe é exibido para seus usuários, teste um piloto com um único grupo e sequencie o trabalho para que não haja surpresas para revisores, aprovadores e proprietários de projetos.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
exl-id: b4413742-c250-4110-9097-6d38842355a4
source-git-commit: 2b5d95ed0a5c72062700bf026a18b8301e4be421
workflow-type: tm+mt
source-wordcount: '832'
ht-degree: 0%

---
# Planejar a implantação do armazenamento em nuvem do Adobe

Você decide como e quando o armazenamento em nuvem do Adobe chega aos usuários. Nada é alterado até que um administrador do Workfront defina o Adobe Cloud Storage como a opção de armazenamento padrão na área de configuração, para que você tenha tempo para testar a experiência e preparar suas equipes antes que qualquer pessoa trabalhe nela.

Este artigo aborda as configurações de implantação que você pode escolher, como realizar o piloto com um único grupo e uma ordem de trabalho sugerida.

## Escolha como o armazenamento em nuvem do Adobe é implantado

Há duas configurações, e você pode aplicar uma a toda a organização ou a grupos específicos da Workfront. Todos os projetos criados no Adobe Cloud Storage usam Aprovações unificadas e o visualizador Frame.io por padrão.

Para obter instruções passo a passo, consulte [Habilitar o Adobe Cloud Storage para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

### Opções de configuração

* **Somente armazenamento em nuvem do Adobe**: novos projetos usam o armazenamento em nuvem do Adobe por padrão. Os usuários não podem criar projetos herdados.
* **Armazenamento em nuvem do Adobe e armazenamento herdado do Workfront**: quando os usuários criam um projeto, eles escolhem entre o armazenamento em nuvem do Adobe (rotulado como &quot;Novo projeto&quot;) e o armazenamento herdado do Workfront (rotulado &quot;Armazenamento herdado&quot;). Para habilitar esta opção, marque a caixa de seleção **Permitir que o usuário selecione o provedor de armazenamento** na área de configuração.

>[!TIP]
>
>Para colocar o armazenamento em nuvem do Adobe na frente de uma equipe menor primeiro, aplique qualquer configuração a um único grupo do Workfront. Isso permite executar um piloto direcionado antes de lançar o projeto de forma mais ampla. Recomendamos começar com uma implantação em nível de grupo para um ritmo controlado e, em seguida, expandir para toda a organização depois que o grupo piloto tiver validado a experiência.

Os objetos existentes mantêm o modelo de armazenamento com o qual foram criados. A alteração da preferência de armazenamento padrão não altera nenhum objeto existente.

![preferências de armazenamento na configuração](assets/storage-preference-groups.png)

## Planejar a implantação

Cada ambiente do Workfront é diferente. Antes de definir o Adobe Cloud Storage como padrão para seus usuários, reserve um tempo para planejar a aparência de uma implantação bem-sucedida para sua organização. As sugestões abaixo não são uma lista de verificação exata, mas um ponto de partida para seu próprio plano.

### Escolher um grupo piloto

Uma implantação com escopo de grupo permite que você coloque o armazenamento em nuvem do Adobe na frente de uma equipe menor primeiro, colete feedback e ajuste antes de uma implantação mais ampla. Escolha um grupo cujos padrões de trabalho sejam representativos o suficiente para exibir problemas que você deseja saber antecipadamente.

<!--
>[!IMPORTANT]
>
>Only members of the pilot group can convert an Adobe cloud storage object, such as a request or a task, into a project. Users outside the group, including Workfront administrators, see the error "User is not eligible for this operation."
-->

### Teste antes de entrar em funcionamento

O armazenamento na nuvem do Adobe está disponível em ambientes de sandbox da Workfront, para que você possa validar grande parte da experiência antes da produção. O visualizador Frame.io não está disponível na sandbox, portanto, você valida a experiência de revisão e aprovação completa na produção com seu grupo piloto. Para obter mais informações, consulte [Habilitar o armazenamento na nuvem do Adobe para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

### Comunicar a alteração aos usuários finais

A maior alteração visível para revisores, aprovadores e proprietários de projetos é a nova área Documentos e o visualizador Frame.io que possibilita a revisão e a aprovação de projetos de armazenamento na nuvem do Adobe. Planeje a apresentação para que os usuários saibam o que esperar quando encontrarem seu primeiro projeto de armazenamento na nuvem da Adobe. O artigo [Introdução à revisão e aprovação unificadas](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md) é um ponto de partida útil para material voltado para o usuário final.

### Revisar suas permissões e governança

Em projetos de armazenamento na nuvem do Adobe, Gerenciar e Contribute mapeiam para Editar e Compartilhar no Frame.io, que inclui compartilhamento externo. Analise seus padrões de compartilhamento e decida se isso se encaixa em seu modelo de governança antes de trazer equipes para o armazenamento em nuvem da Adobe. Para obter mais informações, consulte [O que há de diferente no armazenamento na nuvem da Adobe](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md#object-permissions-mapping).

### Nomeação e modelos de auditoria

O armazenamento na nuvem do Adobe aplica regras de nomenclatura rigorosas, e o Workfront renomeia automaticamente os objetos que entram em conflito com elas. Se você criar projetos a partir de modelos, revise esses modelos para que os nomes e a estrutura gerados se encaixem nas regras. Para obter mais informações, consulte [O que há de diferente no armazenamento na nuvem da Adobe](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md#object-naming-rules).

### Planejar o Workfront Fusion

Os cenários de Fusão baseados em prova existentes continuam a funcionar em projetos herdados, mas não funcionam automaticamente em projetos de armazenamento em nuvem do Adobe. Antes de trazer equipes que dependem desses cenários para o armazenamento na nuvem da Adobe, classifique cada cenário como Editar, Reconstruir ou Desativar. Para obter mais informações, consulte [Atualizar cenários do Workfront Fusion para revisão e aprovação unificadas](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).

### Plano para reportar alterações

Os dados e relatórios do fluxo de trabalho de aprovação unificados são exibidos nos Painéis do Canvas. Os relatórios de aprovação herdados não são transferidos automaticamente, portanto, configure um painel de substituição antes que suas equipes piloto precisem. Para obter mais informações, consulte [Criar um painel de relatório para revisão e aprovações](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).

## Sequência sugerida

Use essa ordem como um modelo, ajustando-a ao seu ambiente:

1. Teste a experiência em uma sandbox e com um grupo piloto em produção.
2. Classifique e atualize seus cenários do Fusion e crie seus relatórios de Painéis do Canvas.
3. Faça a auditoria de modelos e revise suas permissões e o modelo de compartilhamento.
4. Comunique a alteração aos revisores, aprovadores e proprietários do projeto que a usarão.
5. Defina o armazenamento em nuvem da Adobe como padrão para o grupo piloto e expanda para mais grupos ou toda a organização depois que o piloto validar a experiência.
