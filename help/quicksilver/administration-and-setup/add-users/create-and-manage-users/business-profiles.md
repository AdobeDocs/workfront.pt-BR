---
title: Visão geral dos perfis empresariais
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: add-users-to-workfront
description: Os perfis empresariais são um modelo de permissão aprimorado que permite que clientes como agências gerenciem com eficiência o acesso dos usuários e garantam controle preciso sobre permissões no nível do grupo. Em um perfil comercial, os usuários têm permissões distintas para objetos específicos do grupo. Objetos adicionais também podem ser compartilhados diretamente com o perfil comercial.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 7f62de33-e544-4be9-8dcf-03a2e09e8a05
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: b9e0747a58618353caf3ce1c7e8521d22d2b412d
workflow-type: tm+mt
source-wordcount: '1466'
ht-degree: 0%

---

# Visão geral dos perfis empresariais

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ele está disponível somente no ambiente de Pré-visualização para clientes específicos.</span>

Os perfis empresariais são um modelo de permissão aprimorado que permite que clientes como agências gerenciem com eficiência o acesso dos usuários e garantam controle preciso sobre permissões no nível do grupo. Em um perfil comercial, os usuários têm permissões distintas para objetos específicos do grupo. Objetos adicionais também podem ser compartilhados diretamente com o perfil comercial.

Um perfil de negócios de um usuário é semelhante àquele que tem uma função específica em um grupo, como um controlador financeiro ou gerente de projeto, e que recebe as permissões que acompanham essa função para o grupo especificado. O perfil de negócios pode ser temporário, permitindo as permissões por um período definido para expirar e mantendo restrições de dados para o grupo ou agência.

O administrador do sistema da Workfront:

* Cria os níveis de acesso e define campos restritos conforme necessário
* Atualiza o perfil do usuário com o grupo e o nível de acesso para esse grupo (esse é o perfil comercial)
* Define as datas de efetivação do perfil de negócios conforme necessário
* Atribui modelos de layout aos níveis de acesso

Qualquer usuário que tenha acesso para compartilhar objetos pode compartilhá-los com o perfil comercial, e todos os usuários com o perfil verão o objeto.

## Exemplo de perfil empresarial

>[!BEGINSHADEBOX]

A Sam precisa de diferentes acessos aos projetos para a Agência A e para a Agência B. Ambas as agências são configuradas como grupos na Workfront. (Para obter informações sobre grupos, consulte Visão geral sobre grupos.)

Para a Agência A, a Sam atua como controlador financeiro e precisa de acesso para ver todos os campos financeiros de seus projetos. Para a Agência B, o Sam atua como gerente de projeto e precisa gerenciar as tarefas e os problemas, mas não deve ser capaz de visualizar as informações financeiras.

O administrador do sistema Workfront cria novos níveis de acesso chamados de Controlador Financeiro e Gerente de Projeto. Esses níveis de acesso recebem o acesso correto para dados financeiros. Em seguida, o administrador abre o perfil de usuário do Sam e seleciona &quot;Agência A&quot; como o grupo com o nível de acesso &quot;Controlador financeiro&quot; para criar o primeiro perfil comercial, e &quot;Agência B&quot; como o grupo com o nível de acesso &quot;Gerente de projetos&quot; para criar o segundo perfil comercial.

Quando os perfis empresariais estiverem configurados, quando Sam acessar a lista de projetos, todos os projetos da Agência A e da Agência B serão exibidos (juntamente com quaisquer outros projetos para os quais o Sam tenha criado ou recebido permissões). Os campos financeiros dos projetos da Agência A são visíveis para a Sam tanto na exibição da lista quanto nos detalhes do projeto, mas os campos financeiros dos projetos da Agência B estão ocultos. Os nomes dos campos são exibidos, mas os dados dos campos ficam em branco.

Se outros usuários em qualquer uma das agências compartilharem projetos com os perfis de negócios &quot;Auditor Financeiro - Agência A&quot; ou &quot;Gerente de projetos - Agência B&quot;, esses projetos estarão visíveis para a Sam. Os campos financeiros dos projetos da Agência B permanecerão sempre ocultos, porque isso é definido no nível de acesso.

>[!ENDSHADEBOX]

## Como os perfis empresariais são definidos

O administrador do sistema do Adobe Workfront é responsável por definir todas as áreas de um perfil de negócios.

### Criar nível de acesso

O administrador do sistema do Workfront cria o nível de acesso com o acesso necessário e define quaisquer campos restritos conforme necessário.

Para obter mais informações, consulte [Criar e modificar níveis de acesso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

### Adicionar perfil empresarial ao usuário

O administrador do sistema do Workfront adiciona o perfil comercial a um perfil de usuário selecionando um grupo e nível de acesso. A combinação dos dois cria o perfil empresarial. Cada grupo só pode ser usado em um perfil empresarial por usuário. <!--how does this combine with more than one access level per group. As far as I can see a business profile is one level and one group-->

O perfil empresarial pode ter mais de um nível de acesso por grupo. O nível com o maior acesso tem prioridade.

O administrador pode atribuir datas de efetivação a um perfil comercial, de modo que o acesso do usuário expire em uma data futura. As datas de início e término indicam quando o usuário começa e termina mantendo o perfil nesse grupo. Usar datas efetivas para encerrar o acesso em vez de excluir o perfil permite que o perfil seja ativado novamente no futuro.

Vários perfis empresariais são permitidos para um usuário.

<!--image?-->

Para obter mais informações, consulte [Editar perfil de usuário](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md). <!--may be separate article now since it's not in the profile-->

### Atribuir modelos de layout ao nível de acesso

O administrador do sistema do Workfront pode, opcionalmente, atribuir um modelo de layout ao nível de acesso, para garantir que os usuários com o perfil de negócios relacionado vejam informações e ações relevantes com base em sua função no sistema.

Para obter mais informações, consulte [Atribuir usuários a um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

## Como os perfis empresariais funcionam

Quando um perfil empresarial é adicionado a um usuário, as permissões na combinação do grupo e do nível de acesso determinam o que o usuário verá no Workfront.

### Layout do Workfront

Quando o grupo no perfil comercial está associado a um projeto, o modelo de layout para o nível de acesso no perfil comercial é aplicado. Todos os usuários com o perfil empresarial verão os itens de menu, a Página inicial e outros elementos de layout incluídos no modelo. O modelo de layout do perfil de negócios tem prioridade sobre um modelo de layout atribuído ao usuário.

Se o perfil de negócios tiver vários níveis de acesso com o mesmo grupo, os modelos de layout para ambos os níveis de acesso serão combinados. Todos os elementos de layout disponíveis são exibidos. Se um item de menu for exibido em um modelo, mas oculto em outro, ele será exibido. Somente os itens ocultos em todos os modelos para o perfil comercial ficam ocultos.

Para situações em que os mesmos itens são exibidos em vários modelos de layout, mas a ordem dos itens é diferente (como a navegação à esquerda ou pinos), a ordem do modelo do nível de acesso listado primeiro no perfil comercial é usada.

### Projetos e outros objetos compartilhados

Quando um projeto é associado a um grupo, um usuário com um perfil comercial para esse grupo pode exibir o projeto. A visibilidade dos campos no projeto é baseada no nível de acesso no perfil empresarial. Se vários níveis de acesso forem atribuídos ao grupo no perfil comercial do usuário, o nível com as permissões mais altas será aplicado.

Por exemplo, um usuário tem dois perfis comerciais: o primeiro fornece acesso de controlador financeiro para um grupo (para ver campos financeiros) e o segundo fornece acesso de gerente de projeto em um grupo diferente (onde os campos financeiros não devem ser visualizados).

O usuário veria os projetos de ambos os grupos na lista de todos os projetos. Tanto na visualização de lista quanto nos detalhes do projeto, o usuário veria os dados financeiros apenas para o primeiro grupo. Os campos de financiamento nos projetos do segundo grupo ficariam em branco.

Qualquer usuário com acesso para compartilhar objetos pode compartilhá-los com um perfil comercial. Todos os usuários atribuídos ao perfil terão as permissões especificadas para o objeto. No entanto, se o acesso for restrito no nível de acesso atribuído pelo administrador no perfil de negócios, o nível de acesso terá prioridade sobre as permissões fornecidas no compartilhamento. Por exemplo, se o nível de acesso não permitir a criação de tarefas, o usuário não poderá adicionar tarefas a um projeto, mesmo que tenha permissões de Gerenciamento para um projeto quando ele for compartilhado com o perfil empresarial.

Se um usuário receber um perfil comercial depois que um objeto já tiver sido compartilhado com o perfil, ele verá o objeto com o acesso especificado.

Quando um perfil comercial tem vários níveis de acesso, o nível com a maior quantidade de acesso tem prioridade.

Para obter informações sobre compartilhamento, consulte [Compartilhar um objeto](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

Para obter informações sobre como os níveis de acesso e as permissões funcionam juntos, consulte [Visão geral dos níveis de acesso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

## Considerações sobre perfis empresariais

* Um usuário não precisa ser membro de um grupo para receber um perfil de negócios para esse grupo.
* O nível de acesso no perfil empresarial só pode atualizar o nível de acesso &quot;básico&quot; de um usuário. O perfil empresarial não pode remover as permissões básicas de nível de acesso.
* Em listas de objetos e relatórios, o usuário tem todas as permissões que estão disponíveis a ele em todos os perfis de negócios atribuídos nos grupos mesclados com seu nível de acesso básico. Em outras páginas, o usuário tem as permissões de nível de acesso básico.
* Quando um grupo é excluído do Workfront, todos os perfis de negócios atribuídos para esse grupo são removidos dos usuários associados.
* Se um nível de acesso fizer parte de um perfil de negócios e você deletar o nível de acesso, será solicitado que você escolha um novo nível de acesso para usar.
* As atualizações para perfis empresariais são rastreadas nos logs de auditoria do Workfront. Para obter mais informações, consulte Visão geral dos logs de auditoria.
