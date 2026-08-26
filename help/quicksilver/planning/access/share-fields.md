---
title: Compartilhar campos do Workfront Planning
description: Você pode compartilhar o campo de um registro do Workfront Planning com outras pessoas para garantir a colaboração ao usar o Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 2d26437c69b3c36366938952d426532934f55c52
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 3%

---


# Compartilhar campos do Workfront Planning

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Você pode compartilhar o campo de um registro do Workfront Planning com outras pessoas para garantir a colaboração ao usar o Adobe Workfront Planning.

O compartilhamento de campo permite que os administradores de espaço de trabalho controlem o acesso a um campo individual. Cada campo em um tipo de registro tem seu próprio diálogo de compartilhamento, em que o acesso pode ser definido como Sem acesso, Exibir valores de campo ou Gerenciar valores de campo.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->



<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<p>Qualquer Workfront ou Fluxo de trabalho com um pacote do Planning</p> 
Ou
<p>Qualquer pacote de produto do Workfront Planning como independente</p> 
 </tr> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Qualquer</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>licença do Adobe Planning</p></td> 
   <td><p>Qualquer</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Você deve adicionar um Workflow e um tipo de licença do Planning ao nível de acesso quando tiver um Workflow e um pacote do Planning</p>   
</td> 
  </tr>  
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td><p>Gerenciar permissões em um campo para alterar valores do campo</p>  
   <p>Contribuir com ou mais permissões para um tipo de registro para herdar Gerenciar permissões para o campo</p>  
   </td> 
  </tr>
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações sobre o compartilhamento de campos

* Você pode compartilhar campos com usuários, funções de trabalho, grupos, equipes ou empresas.
* O acesso a um campo vem da combinação das seguintes configurações:

  * **Permissões herdadas**: por padrão, um campo herda o mesmo acesso que alguém tem no tipo de registro (as permissões do tipo Exibir registro dão ao usuário permissões para exibir valores de campo; as permissões do tipo Contribute ou Gerenciar registro dão ao usuário permissões para gerenciar valores de campo). Você pode desativar as Permissões herdadas e conceder aos usuários um acesso ao campo menor do que eles têm para o tipo de registro.
  * O **Todos no espaço de trabalho podem exibir** ou **Somente pessoas convidadas podem acessar** a seleção. Você pode permitir que qualquer pessoa com permissões para o espaço de trabalho exiba o campo ou conceder permissões somente a entidades individuais.

  Se várias regras se aplicarem à mesma pessoa, ela receberá a permissão mais alta disponível de uma das regras.

* Somente os proprietários e gerentes de espaços de trabalho podem ajustar as permissões de campo; os gerentes de espaços de trabalho sempre mantêm o acesso Gerenciar a todos os campos e isso não pode ser reduzido.
* O compartilhamento de campos controla o acesso a valores, não a configurações de campo. Somente gerentes de espaço de trabalho podem alterar a configuração de um campo.
* Adicionar alguém a uma lista de compartilhamento de campo não concede a ele acesso de espaço de trabalho ou tipo de registro. Se não tiverem esse acesso, um ícone de aviso indicará que a permissão só terá efeito depois que forem adicionadas ao tipo de registro.
* Os campos do sistema (por exemplo, Criado por, ID de registro) e os campos primários não podem ter compartilhamento restrito.
* Campos restritos são aplicados em qualquer lugar onde o campo é exibido. Isso inclui todas as exibições, páginas de detalhes de registro, formulários de solicitação, conexões e campos de pesquisa, painéis do Canvas, a API e ferramentas do MCP.
* Os campos de pesquisa herdam as permissões do campo de origem.
* As visualizações públicas permanecem totalmente visíveis e somente leitura para qualquer pessoa que possa acessá-las.
* Quando você duplica um registro, os valores restritos não são copiados para os novos registros.
* As alterações de valor de campo restrito não são registradas no Histórico de um registro.
* As alterações de permissão para campos não acionam notificações.
* Para tipos de registros globais, as permissões de campo se aplicam a todos os espaços de trabalho secundários e não podem ser ajustadas localmente.


De Claude:
Permissões adicionais para campos — pode ser adicionado ao artigo Visão geral para todo o compartilhamento? - help/quicksilver/planning/access/sharing-permissions-overview.md

Veja como o tipo de registro/acesso ao espaço de trabalho mapeia para o acesso em nível de campo no documento:

Níveis de permissão de campo (somente dois, mais nenhum):

Sem acesso - o campo está completamente oculto
Exibir valores do campo - pode ver o valor, não pode editar
Gerenciar valores de campo - pode exibir e editar

Herança padrão da função do tipo de registro

Tipo de registro/acesso ao espaço de trabalho Permissão de campo padrão
Exibir valores do campo de exibição
Valores de campo do Contribute Manager
Gerenciar (gerenciador de espaço de trabalho) Gerenciar valores de campo (bloqueado — não pode ser reduzido)

Por padrão, um campo simplesmente reflete qualquer função que uma pessoa tenha no tipo de registro: os visualizadores são somente leitura, os Colaboradores e Gerentes recebem direitos de edição. Os gerentes de Workspace são um caso especial: sempre que são adicionados à lista de compartilhamento de um campo, a opção &quot;Gerenciar valores de campo&quot; é pré-selecionada e a opção &quot;Exibir valores de campo&quot; está desativada, já que o acesso de edição nunca pode ser removido.

Configuração de curinga (fallback)
Separado da herança, cada campo tem um padrão curinga:

Todos no espaço de trabalho podem visualizar (padrão)
Somente pessoas convidadas podem acessar

Como a permissão final é calculada

Se as permissões herdadas estiverem ativadas: o acesso de uma pessoa = o mais alto de (herdado do tipo de registro, curinga, permissão concedida individualmente).
Se as permissões herdadas estiverem desativadas: o acesso de uma pessoa = o mais alto de (curinga, permissão concedida individualmente) — a função do tipo de registro não é mais considerada no.
Se a herança estiver desativada, o curinga é &quot;Somente pessoas convidadas podem acessar&quot;, e a pessoa não é adicionada individualmente → ela não recebe Acesso.

Outras notas de permissão

Conceder acesso individualmente a alguém não concede acesso ao espaço de trabalho/tipo de registro — ele fica inativo (com um ícone de aviso) até que seja adicionado separadamente ao espaço de trabalho.
Para Tipos de registro globais, as permissões de campo são definidas uma vez e se aplicam a todos os espaços de trabalho secundários; os gerentes de espaço de trabalho secundários/da equipe não podem substituí-los localmente.

## Compartilhar campos

