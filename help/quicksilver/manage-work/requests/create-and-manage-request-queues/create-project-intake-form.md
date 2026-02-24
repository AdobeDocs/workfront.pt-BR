---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Criar entrada de projeto no Forms
description: Você pode usar formulários de entrada de projetos para simplificar o processo de criação de projetos no Workfront
author: Becky
feature: Work Management, Requests
role: User, Admin
hide: true
hidefromtoc: true
source-git-commit: 5ff71313c550d949079e7426b657a0a4e19a656c
workflow-type: tm+mt
source-wordcount: '1329'
ht-degree: 4%

---

# Criar formulários de entrada de projeto

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Os formulários de entrada de projetos são um tipo de formulário de solicitação que permite aos usuários solicitar projetos. Os projetos são criados a partir do formulário, sem precisar criar um projeto a partir de um problema enviado.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

Você deve ter o seguinte acesso para realizar as etapas descritas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Nova licença: Standard </p>
   Ou
   <p>Licença atual: plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront para criar formulários de entrada de projetos. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outros produtos</td> 
   <td> <p>Sua organização deve ter adquirido o Workfront Planning para usar os recursos do Planning, como automações.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Recursos e limitações do Project Intake Forms

### Recursos

Os formulários de entrada de projeto incluem os seguintes recursos:

#### Automações do Workfront Planning

Os formulários de entrada de projetos do Workfront são compatíveis com o Workfront Planning Automations, para configurar as propriedades específicas do projeto criadas.

Para obter mais informações sobre automações do Planning, consulte [Configurar automações do Adobe Workfront Planning](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

### Configuração de aprovação

Os formulários de entrada de projeto incluem a capacidade de configurar aprovadores para solicitações enviadas.

### Limitações

#### Tipos de campo compatíveis

O Project Intake Forms pode incluir campos de qualquer formulário personalizado com o tipo de objeto Projeto.

Os seguintes tipos de campo não são suportados no momento no Project Intake Forms:

* Seção
* Fórmula
* Rollup
* Rollup de linha única
* Conexão do planejamento
* Referências de campos nativos que são referenciados para campos nativos do Project, que são somente leitura (por exemplo, `workRequiredExpression`)

#### Solicitando experiência

Os formulários de entrada de projeto podem ser usados somente com a nova experiência de solicitação.

Para obter informações sobre a nova experiência de solicitação, consulte [Criar e enviar solicitações](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

#### Compartilhamento

Os formulários de entrada de projetos não oferecem suporte ao compartilhamento público. As opções de compartilhamento incluem:

* **Qualquer um**: qualquer pessoa no sistema pode usar o formulário para enviar uma solicitação de projeto.
* **Usuários especificados**: é possível selecionar quais usuários específicos terão acesso ao formulário de solicitação do projeto.

## Criar um formulário de entrada de projeto

{{step1-to-requests}}

1. Habilite a configuração **Alternar para uma nova experiência**, no canto superior direito da tela.
1. Clique em **Solicitar formulários** no canto superior direito da tela.

   >[!NOTE]
   >
   >Como apenas administradores do Workfront podem criar formulários de entrada, o botão Formulários de solicitação só fica visível para administradores.

   Uma lista de formulários de solicitação atualmente disponíveis é exibida. Isso inclui formulários de solicitação do Workfront Planning.

1. Clique em **Novo formulário de solicitação** no canto superior direito da tela.
1. Insira um nome para o formulário de solicitação. O nome padrão do formulário é **Formulário sem título**.
1. Selecione o tipo de objeto **Projeto** próximo à parte superior da lista suspensa. Atualmente, esse é o único tipo de projeto do Workfront disponível. Outros itens na lista pertencem ao Workfront Planning.
1. (Opcional) Adicione uma **Descrição** para o formulário de solicitação.
1. Clique em **Criar**. O formulário de solicitação para o tipo de registro selecionado é aberto na guia Formulário.

   O construtor de formulários de entrada de projeto é aberto na guia Formulário.

   O formulário de entrada contém as seguintes informações, por padrão:

   * **Seção padrão**: esta é a quebra de seção padrão que o Workfront aplica ao formulário de solicitação. Todos os campos de registro são exibidos na área **Seção padrão**.
   * Campo **Assunto**: o campo que identificará a solicitação no Workfront. A configuração e o valor do campo Subject não são editáveis.
   * Todos os campos associados a projetos.

     Os campos contidos no formulário de solicitação estarão visíveis para todos que enviarem uma solicitação de projeto.

1. Para adicionar campos ao formulário, clique no tipo de campo na navegação à esquerda e selecione o campo.
1. (Opcional) Para remover um campo, passe o mouse sobre o campo no formulário que deseja remover, em seguida, clique no ícone **x** para removê-lo.
1. (Opcional) Para remover a **Seção padrão** do formulário, faça o seguinte:

   1. Remova todos os campos da Seção padrão.
   1. Clique na guia **Elementos de conteúdo**, adicione uma nova seção e adicione um nome para a seção.
   1. Adicione campos à nova seção.
   1. Clique no ícone **x** para remover a **Seção padrão**.
1. Clique em qualquer campo e use os controles no painel direito no formulário para definir seu tamanho ou qualquer uma das seguintes informações:

   * **Rótulo**: este é o nome do campo como ele aparecerá no formulário de solicitação. Isso não altera o nome do campo de registro.
   * **Instruções**: adicione mais informações sobre o campo.
   * **Criar um campo obrigatório**: quando selecionado, o campo deve ter um valor. Caso contrário, o formulário não poderá ser enviado.
   * **Adicionar lógica**: defina quais condições devem ser atendidas para que o campo seja exibido ou fique oculto.

   >[!TIP]
   >
   >   O tipo de campo de cada campo é exibido na parte superior do painel direito, depois que você seleciona o campo no formulário.
   >     

1. (Opcional) Clique na guia **Elementos de conteúdo** no lado esquerdo do formulário e adicione qualquer um dos seguintes elementos:

   * **Texto descritivo**
   * **Quebra de seção**

   Para obter mais informações sobre como criar um formulário personalizado, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Clique na guia **Automações** no lado esquerdo do formulário e siga um destes procedimentos:

   * Selecionar um modelo de projeto
   * Anexar qualquer formulário personalizado
   * Definir um proprietário de projeto
   * Adicionar o projeto a um portfólio ou programa

   Quaisquer seleções feitas aqui serão aplicadas aos projetos criados a partir deste formulário de entrada.

1. (Opcional) Clique em **Visualizar** para ver como o formulário será exibido para outros usuários quando eles o usarem para enviar um novo registro.

1. (Opcional) Clique na guia **Configuração** e adicione pelo menos um usuário ou equipe&lt; ao campo **Aprovadores** para aprovar novas solicitações para este formulário de entrada.

   * Quando você associa um formulário de entrada a aprovadores, qualquer nova solicitação deve ser aprovada primeiro por todos os aprovadores antes de gerar um projeto.
   * Você pode adicionar um ou vários aprovadores a um formulário de entrada.
   * Se pelo menos um aprovador rejeitar a solicitação, ela será rejeitada e o projeto não será criado.
   * Todos os aprovadores devem tomar uma decisão antes que um projeto seja aprovado ou rejeitado.
   * Se uma equipe estiver definida como um aprovador, somente uma decisão será necessária da equipe.

     Para obter mais informações sobre como adicionar aprovações a formulários de solicitação, consulte [Adicionar aprovação a um formulário de solicitação](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

1. (Opcional) Clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do formulário no cabeçalho e clique em **Editar** para atualizar o nome do formulário.

1. Clique em **Publicar** para publicar o formulário e obter um link exclusivo para ele.

   As seguintes situações ocorrem:

   * O botão **Publicar** foi removido.
   * O botão **Cancelar publicação** é adicionado ao formulário. Clicar nele impedirá que o formulário seja acessível.
   * Um botão **Compartilhar** é adicionado ao formulário.
   * O formulário fica disponível na área Solicitações do menu Principal do Workfront.

1. Clique em **Compartilhar** para compartilhar o formulário com outras pessoas.
1. Clique na seta à esquerda do nome do formulário no cabeçalho para fechar o formulário.

   A exibição de tabela **Formulários de solicitação** é aberta e o formulário é adicionado a ela.

1. (Opcional) Passe o mouse sobre o nome de um formulário de solicitação na exibição de tabela, em seguida, clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do formulário e clique em um dos seguintes:

   * **Editar formulário**: clique para editar mais informações sobre o formulário.
   * **Cancelar publicação**: clique para desfazer a publicação do formulário que o remove da área Solicitações no Workfront.
   * **Compartilhar**: clique aqui para modificar quem tem acesso ao formulário.
   * **Copiar link**: clique para copiar rapidamente o link do formulário de solicitação sem abrir o formulário.
   * **Excluir**: clique aqui para excluir o formulário. Todas as solicitações e registros adicionados usando o formulário não são excluídos. O formulário não pode ser recuperado.

   >[!NOTE]
   >
   >Você pode identificar formulários de entrada de projeto na exibição de tabela porque eles exibem &quot;Projeto&quot; na coluna Tipo de objeto.

1. Clique na seta à esquerda de **Formulários de solicitação** no cabeçalho para fechar a tabela de formulários de solicitação.

