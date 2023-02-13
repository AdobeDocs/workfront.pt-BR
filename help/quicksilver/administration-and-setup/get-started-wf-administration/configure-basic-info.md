---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configurar informações básicas para seu sistema
description: Como parte da configuração do seu sistema Adobe Workfront, você pode gerenciar os detalhes da sua organização na seção Informações básicas da sua página Informações do cliente .
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bad5e700-79a6-49ed-bcf9-f0b5b3eaa909
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 2%

---

# Configurar informações básicas para seu sistema

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

Como parte da configuração do seu sistema Adobe Workfront, você pode gerenciar os detalhes da sua organização na seção Informações básicas da sua página Informações do cliente .

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront. Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Acessar informações do cliente

O cliente representa a instância do Workfront para sua organização. As opções nessa área são exclusivas para você, como cliente da Workfront.

Para acessar a página Informações do cliente :

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Sistema** > **Informações do cliente**.

   Dependendo do plano da Workfront adquirido, algumas seções podem estar faltando na página Informações do cliente . Entre em contato com seu Representante de conta, caso precise descobrir qual plano da Workfront sua organização usa.

   As seções disponíveis na área Informações do cliente são:

   * **Informações básicas**

      Para obter informações sobre como configurar informações básicas no Workfront, consulte [Configurar informações básicas](#configure-basic-info).

   * **Configurações da Chave de API**

      Para obter informações sobre as configurações da chave de API, consulte [Gerenciar chaves de API](../../administration-and-setup/manage-workfront/security/manage-api-keys.md).

   * **Lista branca de IPs**

      Para obter informações sobre como adicionar endereços IP à sua lista de permissões de onde os usuários podem acessar o Workfront, consulte [Configurar a  lista de permissões do firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   * **Licença**

      Para obter informações sobre licenças, consulte [Gerencie as licenças disponíveis em seu sistema](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

## Configurar informações básicas {#configure-basic-info}

Dentro da área Informações básicas da página Informações do cliente, alguns detalhes sobre o cliente são configurados pela Workfront e são exibidos em um modo somente leitura. Você pode configurar outros detalhes. Qualquer opção que você possa editar nessa área terá um efeito global em todos os usuários no Workfront.

Para configurar sua seção Informações básicas na área Informações do cliente :

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Sistema** > **Informações do cliente**.

1. No **Informações básicas** na parte superior do **Informações do cliente** localize as seguintes informações sobre sua instância com o Workfront:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td>O nome da sua organização, que também corresponde ao nome da sua empresa. Isso é adicionado pelo Workfront e não pode ser editado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ajuste do Cluster </td> 
      <td>O número do cluster da sua instância.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Email do Admin</td> 
      <td> <p>O endereço de email do administrador do Workfront. É possível editar esse campo para corresponder ao endereço de email de um dos administradores do Workfront. O usuário associado a esse endereço de email é considerado o administrador principal do Workfront do sistema Workfront. Qualquer comunicação do Workfront em todo o site é direcionada a esse endereço de email, portanto, é importante mantê-lo atualizado.</p> <p><b>OBSERVAÇÃO</b>: Não é possível desativar, excluir ou alterar o Nível de acesso do usuário associado ao Email de administrador.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Domínio</td> 
      <td> <p>O domínio é definido pela Workfront quando a conta é criada.</p> <p>O domínio identifica seu subdomínio exclusivo do URL que você usa para acessar o Workfront.<p>Por exemplo, se sua organização recebeu o domínio "mycompany", o URL que você usa para acessar o Workfront é <i>https://mycompany.my.workfront.com.</i></p><p>Você mesmo não pode editar o domínio. Se quiser alterar seu domínio, entre em contato com o Suporte ao cliente da Workfront. Para obter mais informações sobre como entrar em contato com o Suporte ao cliente da Workfront, consulte <a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Entre em contato com o Suporte ao cliente</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fuso Horário</td> 
      <td> <p>Esse é o fuso horário padrão da sua instância do Workfront. É possível editar esse campo para corresponder ao fuso horário do local principal do Workfront. O fuso horário selecionado determina o seguinte: </p> 
       <ul> 
        <li>A data e a hora exibidas em emails de saída</li> 
        <li>O fuso horário padrão para novos usuários quando eles são criados</li> 
       </ul> <p>Os usuários podem modificar o fuso horário de sua instância do Workfront em seu perfil. Quando os usuários modificam seu fuso horário, a data e a hora em seus emails do Workfront correspondem às preferências do perfil. Para obter mais informações sobre como modificar as preferências do perfil do usuário, consulte <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Definir minhas configurações</a>. Ele é selecionado como fuso horário padrão quando você cria uma nova programação. Para obter mais informações sobre como criar programações, consulte <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Criar um agendamento</a>.</p> <p>Para obter informações sobre como usar agendamentos para ajudar usuários a colaborar no Workfront em vários fusos horários, consulte <a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Trabalhar em vários fusos horários</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Localidade</td> 
      <td>Controla o idioma, a data e o formato do número usados nas mensagens de email de saída. A localidade selecionada aqui é o padrão quando novos usuários são criados. Os usuários podem modificar o local, no perfil do usuário. Quando os usuários modificam sua localidade, o idioma, a data e o formato do número em seus emails do Workfront correspondem às preferências do perfil. Para obter mais informações sobre como modificar suas preferências de perfil, consulte <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Definir minhas configurações</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cota de armazenamento</td> 
      <td> <p>Essa é a quantidade de espaço de armazenamento de documentos disponível em sua instância do Workfront.<br>A cota contém documentos carregados diretamente no Workfront.<br>Não inclui:</p> 
       <ul> 
        <li>Documentos que você vincula ao Workfront de qualquer outro provedor de serviços de terceiros (SharePoint, Google Drive, Webdam, Box, Dropbox, qualquer outro provedor de Gerenciamento de ativos de documentos).</li> 
        <li>Seus dados do Workfront (projetos, tarefas, problemas, usuários e assim por diante).</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Versão do Produto</td> 
      <td>Esse é o tipo de instância do Workfront atribuído a você. A versão do produto para a maioria dos clientes do Workfront é <strong>Empresa</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.
