---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configurar informações básicas do seu sistema
description: Como parte da configuração do seu sistema Adobe Workfront, você pode gerenciar detalhes sobre sua organização na seção Informações básicas da página Informações do cliente.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bad5e700-79a6-49ed-bcf9-f0b5b3eaa909
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 2%

---

# Configurar informações básicas do sistema

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

Como parte da configuração do seu sistema Adobe Workfront, você pode gerenciar detalhes sobre sua organização na seção Informações básicas da página Informações do cliente.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Novo: Padrão</p>
   Ou
   <p>Atual: Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Acessar informações do cliente

O cliente representa a instância do Workfront da sua organização. As opções nessa área são exclusivas para você, como cliente da Workfront.

Para acessar a página Informações do cliente:

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Sistema** > **Informações do cliente**.

   Dependendo do plano Workfront adquirido, algumas seções podem estar ausentes na página Informações do cliente. Entre em contato com o Representante de conta se precisar descobrir qual plano da Workfront sua organização usa.

   As seções disponíveis na área Informações do cliente são:

   * **Informações Básicas**

     Para obter informações sobre como configurar informações básicas no Workfront, consulte [Configurar Informações Básicas](#configure-basic-info).

   * **Configurações da Chave de API**

     Para obter informações sobre as configurações da chave de API, consulte [Gerenciar chaves de API](../../administration-and-setup/manage-workfront/security/manage-api-keys.md).

   * **Inclui na lista de permissões IP**

     Incluir na lista de permissões Para obter informações sobre como adicionar os endereços IP ao seu arquivo para o qual os usuários podem acessar o Workfront incluir na lista de permissões, consulte [Configurar o arquivo do seu firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   * **Licença**

     Para obter informações sobre licenças, consulte [Gerenciar licenças disponíveis em seu sistema](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

## Configurar informações básicas {#configure-basic-info}

Na área Informações básicas da página Informações do cliente, alguns detalhes sobre o cliente são configurados pela Workfront e exibidos em modo somente leitura. Você pode configurar outros detalhes. Qualquer opção editada nesta área tem um efeito global em todos os usuários no Workfront.

Para configurar a seção Informações básicas na área Informações do cliente:

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Sistema** > **Informações do cliente**.

1. Na seção **Informações básicas**, na parte superior da página **Informações do cliente**, localize as seguintes informações sobre a sua instância com o Workfront:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td>O nome da sua organização, que também corresponde ao nome da sua empresa. Ele é adicionado pelo Workfront e não pode ser editado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ajuste do Cluster </td> 
      <td>O número do cluster da sua instância.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Email do Admin</td> 
      <td> <p>O endereço de email do administrador do Workfront. É possível editar esse campo para corresponder ao endereço de email de um dos administradores do Workfront. O usuário associado a esse endereço de email é considerado o principal administrador do Workfront em seu sistema Workfront. Qualquer comunicação em todo o site do Workfront é direcionada a este endereço de email, portanto, é importante mantê-la atualizada.</p> <p><b>OBSERVAÇÃO</b>: não é possível desativar, excluir ou alterar o Nível de Acesso do usuário associado ao Email do Administrador.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Domínio</td> 
      <td> <p>O domínio é definido pela Workfront quando sua conta é criada.</p> <p>O domínio identifica o subdomínio exclusivo do URL usado para acessar o Workfront.<p>Por exemplo, se o domínio "mycompany" foi atribuído à sua organização, a URL usada para acessar o Workfront é <i>https://mycompany.my.workfront.com.</i></p><p>Você não pode editar o domínio sozinho. Se quiser alterar o domínio, entre em contato com o Suporte ao cliente da Workfront. Para obter mais informações sobre como entrar em contato com o Suporte ao Cliente da Workfront, consulte <a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contatar o Suporte ao Cliente</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fuso horário</td> 
      <td> <p>Esse é o fuso horário padrão da sua instância do Workfront. Você pode editar esse campo para corresponder ao fuso horário de seu local principal do Workfront. O fuso horário selecionado determina o seguinte: </p> 
       <ul> 
        <li>A data e a hora exibidas nos emails de saída</li> 
        <li>O fuso horário padrão para novos usuários quando eles são criados</li> 
       </ul> <p>Os usuários podem modificar o fuso horário de sua instância do Workfront em seu perfil. Quando os usuários modificam o fuso horário, a data e a hora em seus emails do Workfront correspondem às preferências de perfil. Para obter mais informações sobre como modificar as preferências do perfil de usuário, consulte <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurar minhas configurações</a>. Ele é selecionado como fuso horário padrão ao criar um novo agendamento. Para obter mais informações sobre como criar agendas, consulte <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Criar uma agenda</a>.</p> <p>Para obter informações sobre como usar agendas para ajudar usuários a colaborar na Workfront entre fusos horários, consulte <a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Trabalhando entre fusos horários</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Localidade</td> 
      <td>Controla o idioma, a data e o formato do número usados nas mensagens de email de saída. A localidade selecionada aqui é o padrão quando novos usuários são criados. Os usuários podem modificar o local no perfil do usuário. Quando os usuários modificam seu local, o idioma, a data e o formato do número em seus emails do Workfront correspondem às preferências de perfil. Para obter mais informações sobre como modificar suas preferências de perfil, consulte <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurar minhas configurações</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cota de armazenamento</td> 
      <td> <p>Essa é a quantidade de espaço de armazenamento de documentos disponível na instância do Workfront.<br>A cota contém documentos que você carregou diretamente no Workfront.<br>Não inclui:</p> 
       <ul> 
        <li>Documentos vinculados ao Workfront por qualquer outro provedor de serviços de terceiros (SharePoint, Google Drive, Webdam, Box, Dropbox, qualquer outro provedor de gerenciamento de ativos de documentos).</li> 
        <li>Seus dados do Workfront (projetos, tarefas, problemas, usuários e assim por diante).</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Versão do Produto</td> 
      <td>Esse é o tipo de instância do Workfront atribuída a você. A versão do produto para a maioria dos clientes do Workfront é a <strong>Enterprise</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.
