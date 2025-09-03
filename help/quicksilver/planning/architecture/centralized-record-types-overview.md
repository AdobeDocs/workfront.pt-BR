---
title: Visão Geral de Tipos de Registro Centralizados
description: Os tipos de registro centralizado podem ser adicionados a vários espaços de trabalho a partir de um espaço de trabalho central ou principal no Adobe Workfront Planning.
hidefromtoc: true
hide: true
source-git-commit: 4e295b4fdbbde7439567ef2a4f4383ad8dea738c
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Visão geral dos tipos de registro centralizado


Os tipos de registro centralizado podem ser adicionados a vários espaços de trabalho a partir de um espaço de trabalho central ou principal no Adobe Workfront Planning.

## Visão geral dos tipos de registros centralizados

Ao implementar o Workfront Planning para uma organização de várias equipes com workflows comuns, talvez seja necessário definir uma estrutura coesa e metadados para os principais tipos de registro (como Campanhas ou Materiais de entrega) que podem ser adicionados aos espaços de trabalho de cada equipe para capturar e gerenciar o trabalho.

Além disso, você pode precisar do trabalho de cada equipe para chegar a um nível central e mais global.

Nesse fluxo de trabalho, é possível garantir que as equipes capturem seu trabalho de forma consistente ao desbloquear a visibilidade entre equipes, sem a necessidade de adicionar todos na organização a um espaço de trabalho.

Para usar tipos de registro centralizados, faça o seguinte:

1. Configure um tipo de registro a ser centralizado.

   Para obter informações, consulte [Configurar recursos entre espaços de trabalho para tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Adicionar um tipo de registro existente a partir de um centralizado.

   Para obter informações, consulte [Adicionar tipos de registros existentes](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md).




· Uma nova configuração &quot;Permitir a adição do tipo de registro em outros espaços de trabalho&quot; está disponível em Configurações avançadas para tipos de registro.

· Se ativado, o gerenciador de espaço de trabalho pode selecionar usuários com licença Standard, equipes, grupos, funções ou empresas que podem adicionar o tipo de registro nos espaços de trabalho que gerenciam.

· O gerenciador de espaço de trabalho que está editando a configuração será adicionado automaticamente à lista de usuários selecionados por padrão

o O gerenciador de espaço de trabalho pode remover seu próprio nome depois de adicionar pelo menos 1 outra entidade

o É necessário selecionar pelo menos 1 usuário/equipe/... para salvar a configuração

o Depois que o tipo de registro for adicionado em pelo menos 1 outro espaço de trabalho, todos os usuários selecionados poderão ser removidos

§ Isso é feito para que seja possível evitar a adição do tipo de registro global em novos espaços de trabalho, mas mantê-lo nos espaços de trabalho que já o estão usando.

· Na fase 1, todos os registros dos tipos de registro conectados são compartilhados automaticamente com qualquer espaço de trabalho em que o tipo de registro foi adicionado.

· Quando o tipo de registro é ativado como espaço de trabalho cruzado, um campo &quot;Workspace&quot; gerado pelo sistema é adicionado ao tipo de registro

o Ele mostra o espaço de trabalho de onde cada registro foi criado.

o Este campo é somente leitura e não pode ser excluído.

o Pode ser ocultado nos campos de exibição.

o O campo do espaço de trabalho pode ser usado para filtragem, agrupamento e classificação, bem como em qualquer configuração de exibição, como em outros campos.


Tipos de registro entre Workspace em espaços de trabalho locais

· Ao tentar adicionar um novo tipo de registro ao espaço de trabalho, os gerentes de espaço de trabalho locais veem uma opção para selecionar na lista de tipos de registro global que estão disponíveis para eles

· Quando selecionam um dos tipos de registro global, ele é imediatamente adicionado ao espaço de trabalho

· É possível mover o tipo de registro global para qualquer seção e posição no espaço de trabalho local


Permissões para o tipo de registro global em espaços de trabalho locais

Nos espaços de trabalho locais, os membros obtêm o seguinte acesso ao tipo de registro global:

· Na Fase 1, os gerentes de espaço de trabalho locais obtêm permissão do Contribute. Isso significa:

o Os gerentes de espaços de trabalho locais podem:

§ Adicionar o tipo de registro global

§ Adicionar/editar/excluir quaisquer registros no tipo de registro global, independentemente do espaço de trabalho do qual o registro foi adicionado.

§ Excluir o tipo de registro global do espaço de trabalho local

o Os gerentes de espaços de trabalho locais não podem:

§ Adicionar, editar, excluir campos

§ Atualizar a aparência e o rótulo do tipo de registro

§ Consulte as configurações avançadas para o tipo de registro

§ Gerenciamento de automações

§ Gerenciar formulários de solicitação

§ Ajustar o compartilhamento do tipo de registro para o escopo do espaço de trabalho

§ Desabilitar a configuração do tipo de registro global nas configurações avançadas.

· Colaboradores de espaço de trabalho local obtêm permissão do Contribute para o tipo de registro global e podem adicionar e gerenciar registros nele

· Os visualizadores do espaço de trabalho local obtêm permissão de Exibição para o tipo de registro global

· Assim que um registro é adicionado ao tipo de registro global de qualquer um dos espaços de trabalho locais, o campo Workspace mostra esse nome de espaço de trabalho

o Por enquanto, não é possível editar e alterar o campo do espaço de trabalho

· Os registros adicionados aos espaços de trabalho locais são todos sumariados e exibidos no espaço de trabalho principal, e todos os membros desse espaço de trabalho obtêm acesso de visualização a ele.

· Os registros adicionados em espaços de trabalho locais não são exibidos em outros espaços de trabalho locais usando o mesmo tipo de registro global e seus membros não obtêm acesso aos registros.



Acesso a conexões:

· Escopo do MVP

o Os tipos de registro conectados ao tipo de registro global se tornarão visíveis para espaços de trabalho locais onde o tipo de registro global é adicionado para que eles possam usar os campos de conexão para marcar


Comportamento da API

Se o usuário tentar criar registros em um tipo de registro global por meio da API sem fornecer a ID do espaço de trabalho, o sistema verificará se o usuário tem acesso para criar registros no espaço de trabalho principal (onde o tipo de registro global é criado)

· Em caso afirmativo, o registro é criado no espaço de trabalho principal

· Se não, o usuário recebe um erro de validação de que não tem acesso ao espaço de trabalho principal e precisa fornecer a ID do espaço de trabalho onde tem acesso para criar.