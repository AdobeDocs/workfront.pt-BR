---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Configurar o Adobe Workfront com o SAML 2.0 usando ADFS
description: Você pode habilitar a autenticação para o Workfront com o SAML 2.0.
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9bc5987b-6e32-47df-90c8-08ea4b1b7451
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '870'
ht-degree: 0%

---

# Configurar o Adobe Workfront com o SAML 2.0 usando ADFS

{{important-admin-console-onboard}}

Como administrador do Adobe Workfront, você pode integrar o Workfront com uma solução SAML (Security Assertion Markup Language) 2.0 para logon único ao usar os Serviços de Federação do Ative Diretory (ADFS).

Este guia tem como foco a configuração do ADFS sem provisionamento automático ou mapeamentos de atributos. Recomendamos que você conclua a configuração e a teste antes de configurar qualquer provisionamento automático.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
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
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Habilitar autenticação para o Workfront com SAML 2.0

Para habilitar a autenticação no aplicativo Web Workfront e no aplicativo móvel Workfront com SAML 2.0, complete as seguintes seções:

* [Recuperar o arquivo de metadados Workfront SSO](#retrieve-the-workfront-sso-metadata-file)
* [Configurar Confianças de Terceiros Confiantes](#configure-relying-party-trusts)
* [Configurar regras de solicitação](#configure-claim-rules)
* [Faça upload do arquivo de metadados e teste a conexão](#upload-the-metadata-file-and-test-the-connection)

### Recuperar o arquivo de metadados Workfront SSO {#retrieve-the-workfront-sso-metadata-file}

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).
1. No painel esquerdo, clique em **Sistema** > **Logon único (SSO)**.
1. No **Tipo** , clique em **SAML 2.0** para exibir informações e opções adicionais.
1. Copie o URL que é exibido depois de **URL de metadados**.
1. Prossiga para a seção a seguir, [Configurar Confianças de Terceiros Confiantes](#configure-relying-party-trusts).

### Configurar Confianças de Terceiros Confiantes {#configure-relying-party-trusts}

1. Abra o **Gerenciador do ADFS** usando o Windows Server 2008 R2 (a versão pode variar).
1. Ir para **Comece.**
1. Clique em **Ferramentas de administração.**
1. Clique em **Gerenciamento ADFS 2.0.**
1. Selecionar **ADFS** e expandir **Relacionamentos de Confiança**.
1. Clique com o botão direito do mouse **Confianças de terceiros confiáveis**, em seguida selecione **Adicionar Confiança da Entidade Confiadora** para iniciar o Assistente para Adicionar Confiança da Entidade Confiável.
1. No **Página de boas-vindas**, selecione **Iniciar**.
1. No **Selecionar Fonte da Data** cole o URL de metadados do Workfront.
1. Clique em **Próximo**.
1. Clique em **OK** para confirmar a mensagem de aviso.
1. No **Especificar o nome de exibição** , adicione uma **Nome de exibição** e **Notas** para distinguir a Confiança, clique em **Próximo**.
1. Selecionar **Permitir que todos os utilizadores acedam a esta entidade confiadora** (Ou **Nenhum** se quiser configurar isso mais tarde).
1. Clique em **Próximo**.

   Isso leva você ao **Pronto para Adicionar Confiança** seção.

1. Prossiga para a seguinte seção [Configurar regras de solicitação](#configure-claim-rules).

### Configurar regras de solicitação {#configure-claim-rules}

1. Clique em **Próximo** no **Pronto para Adicionar Confiança** , em seguida, verifique se a variável **Abra a caixa de diálogo Editar regras de afirmação** está selecionada.

   Isso permitirá que você edite as Regras de solicitação em uma etapa futura.

1. Clique em **Fechar**.
1. Clique em **Adicionar regra.**
1. Selecionar **Enviar Atributo LDAP como Solicitações**.
1. Clique em **Próximo** para exibir o **Configurar Regra de Reivindicação** etapa.
1. Especifique os seguintes requisitos mínimos para configurar a regra de solicitação: (Isso entrará no **ID de Federação** na configuração do usuário e é usado para distinguir quem está fazendo logon.)


   <table >                
      <tbody>
            <tr>
               <td>Nome da regra da solicitação
               </td>
               <td>Especifique um nome para a regra de afirmação. Por exemplo, "Workfront".</td>
            </tr>
            <tr>
               <td>Repositório de atributos</td>
               <td >Selecionar <b>Ative Diretory</b> no menu suspenso.</td>
            </tr>
            <tr>
               <td>Atributo LDAP</td>
               <td>Pode ser qualquer tipo de atributo. Recomendamos usar <b>SAM-Account-Name</b> para este atributo.</td>
            </tr>
            <tr>
               <td>Tipo de Declaração de Saída</td>
               <td>Você deve selecionar <b>ID do nome</b> como tipo de pedido de reembolso</td>
            </tr>
      </tbody>
   </table>

1. (Opcional) Para estabelecer o provisionamento automático, adicione as seguintes reivindicações adicionais no Atributo LDAP e no Tipo de Solicitação de Saída:

   * Nome
   * Apelido
   * Endereço de email

1. Clique em **Concluir**, depois clique em **OK** na próxima tela.
1. Clique com o botão direito do mouse no novo **Confiança da Entidade Confiadora**, em seguida selecione **Propriedades**.
1. Selecione o **Guia Avançado**. E debaixo **Algoritmo de hash seguro** selecione SHA-1 ou SHA-256.

   >[!NOTE]
   >
   >A opção selecionada em Algoritmo de hash seguro deve corresponder ao campo Algoritmo de hash seguro no Workfront em Configuração > Sistema > Logon único (SSO).

1. Prossiga para a seguinte seção [Faça upload do arquivo de metadados e teste a conexão](#upload-the-metadata-file-and-test-the-connection).

### Faça upload do arquivo de metadados e teste a conexão {#upload-the-metadata-file-and-test-the-connection}

1. Abra um navegador e acesse `https://<yourserver>/FederationMetadata/2007-06/FederationMetadata.xml` .

   Isso deve baixar um arquivo de metadados FederationMetadata.xml .

1. Clique em **Escolher arquivo** under **Preencher campos a partir dos metadados do fornecedor de identidade** e selecione o **FederationMetadata.xml** arquivo.

1. (Opcional) Se as informações do certificado não forem preenchidas com o arquivo de metadados, você poderá fazer upload de um arquivo separadamente. Selecionar **Escolher arquivo** no **Certificado** seção.

1. Clique em **Testar conexão**. Se configurado corretamente, você verá uma página semelhante à mostrada abaixo:

   ![](assets/success-saml-2.png)

   >[!NOTE]
   >
   >Se quiser configurar o mapeamento de atributos, certifique-se de copiar os atributos do Testar Conexão para o Atributo do Diretório. Para obter mais informações, consulte Mapeamento de atributos do usuário.

1. Selecionar **Isenção do administrador** para permitir que os administradores do Workfront façam logon usando credenciais do Workfront com o url de ignorar.

   Marcadores que apontam para `<yourdomain>`.my.workfront.com/login ignore o redirecionamento.

1. Selecione o **Habilitar** para ativar a configuração.
1. Clique em **Salvar**.

## Sobre a atualização de usuários para SSO

Seguindo este guia, a **Nome de Usuário SSO** será seu **Nome de Usuário do Ative Diretory**.

Como administrador do Workfront, você pode atualizar usuários em massa para SSO. Para obter mais informações sobre como atualizar usuários para SSO, consulte [Atualizar usuários para logon único](../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md).

Como administrador do Workfront, você também pode atribuir manualmente uma ID de Federação, editando o perfil do usuário e preenchendo o campo ID de Federação . Para obter mais informações sobre como editar um usuário, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>[!NOTE]
>
>Ao editar os perfis dos usuários para incluir uma ID de Federação, selecione **Permitir apenas a autenticação SAML 2.0** remove a capacidade de fazer logon no Workfront usando o url de ignorar (`<yourdomain>`.my.workfront.com/login).
