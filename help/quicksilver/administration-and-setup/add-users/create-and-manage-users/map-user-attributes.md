---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Mapear Atributos de Usuário
description: Usando o logon único (SSO), você pode passar atributos do Ative Diretory do seu provedor de identidade para seus usuários do Adobe Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 1%

---

# Mapear atributos do usuário

<!--Audited 2/2024-->

Usando o logon único (SSO), você pode passar atributos do Ative Diretory do seu provedor de identidade para seus usuários do Adobe Workfront.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p><p>Ou</p><p>Atual: Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Dicas para mapear atributos

Lembre-se do seguinte ao mapear atributos:

* Sempre teste em uma sandbox de Visualização ou uma sandbox de Atualização de cliente (CR).
* Teste com contas de administrador e não-administrador para confirmar se você está mapeando os atributos corretamente.
* Os atributos mapeados são aplicados sempre que um usuário faz logon único.

  Exemplo: se você estiver mapeando o &quot;sobrenome&quot; e atualizar o nome no Workfront sem atualizar o valor no Provedor de identidade, o sobrenome será substituído para corresponder ao valor do que estiver no Provedor de identidade na próxima vez que o usuário fizer logon.

## Mapear atributos de usuário para sua organização

O procedimento para mapear atributos difere dependendo se sua organização está na experiência unificada de Adobe.

Para determinar se sua organização está na experiência unificada de Adobe, examine o URL que você usa para acessar o Workfront.

| URL | Experiência do Adobe |
|---|---|
| (NomeEmpresa).my.workfront.com | Experiência clássica |
| experience.adobe.com | experiência unificada do Adobe |

* [Mapear atributos do usuário na experiência clássica](#map-user-attributes-in-the-classic-experience)
* [Mapear atributos do usuário na experiência unificada do Adobe](#map-user-attributes-in-the-adobe-unified-experience)

### Mapear atributos do usuário na experiência clássica

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu Principal** no canto superior direito do Adobe Workfront e em **Configurar** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema** > **Logon Único (SSO)**.

1. No menu suspenso **Tipo**, clique em **SAML 2.0**.

1. Clique em **Mapear atributos de usuário**.

   ![](assets/map-user-attributes.png)

1. Na linha de opções exibida, mapeie os atributos necessários para os usuários do Workfront.

   Você pode mapear atributos como Endereço, Gerente, Função, Grupo padrão e assim por diante.

   Os mapeamentos de atributos funcionam em uma proporção de 1:1. Por exemplo, não é possível definir cada grupo ao qual um usuário pertence; você pode definir apenas um por usuário.

   >[!IMPORTANT]
   >
   >Não recomendamos mapear Níveis de Acesso nos Mapeamentos de Atributo. Se você fizer isso, tenha cuidado ao definir o valor padrão para garantir que não remova o Acesso de administrador inadvertidamente.

   A tabela a seguir explica os campos que podem ser usados para mapear atributos:

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader">Workfront atributo de usuário</td> 
      <td>Escolha o nome do atributo que você está mapeando</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Diretório de Atributo</td> 
      <td>Digite o rótulo do atributo SSO que deseja usar.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Valor Padrão</td> 
      <td> <p>Depois de escolher um Atributo de Usuário do Workfront, se o valor for NULL durante a conexão, este campo será preenchido com o valor default correspondente no sistema. Digite um valor aqui somente se planeja aplicar regras de mapeamento de atributos (consulte a etapa 7). O valor padrão atua como uma exceção a essas regras.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Clique em **Regras** para adicionar uma regra ao atributo.

   1. Na lista suspensa, escolha o modificador de atributo que deseja usar.
   1. Nos 2 campos à direita, digite o valor do atributo de diretório e o valor com o qual você deseja substituí-lo.

      ![](assets/rule-fields.png)

   Você pode clicar em **Adicionar regra** para adicionar mais regras ao atributo.

1. (Opcional) Para mapear mais atributos de usuário, clique em **Adicionar mapeamento** e repita as etapas de 6 a 7.
1. Clique em **Salvar**.

### Mapear atributos do usuário na experiência unificada do Adobe

1. Clique no ícone ![](assets/main-menu-left.png) do **Menu Principal** no canto superior esquerdo do Adobe Workfront e em **Configurar** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema** > **Logon Único (SSO)**.

1. Selecione a guia **Adobe**.

1. (Opcional e condicional) Se sua organização tiver o mapeamento de atributos configurado na experiência clássica e você quiser copiar esse mapeamento de atributos para a experiência unificada de Adobe, clique em **Migrar Mapeamentos**. Em seguida, você pode descartar, excluir ou editar esses mapeamentos.

   >[!NOTE]
   >
   >Recomendamos migrar mapeamentos na primeira vez que você configurar mapeamentos na experiência unificada de Adobe. Não há mal em migrá-los novamente mais tarde, mas a migração de mais de uma vez é desnecessária.

1. Para criar um novo mapeamento de atributo, clique em **Adicionar Mapeamento**.

1. Clique na seta ao lado do nome do campo do Workfront e selecione o campo [!DNL Workfront] para o qual você deseja mapear.

1. (Opcional) Se quiser criar mais de uma regra para um determinado campo, clique na seta ao lado de **Sempre** e selecione o operador que deseja que a regra use.

1. (Condicional) Se você tiver selecionado um operador além de Sempre, selecione o campo e o valor do Workfront aos quais o operador se aplica.

   >[!NOTE]
   >
   >Os operadores `Is Truthy` e `Is Falsy` não exigem valores.

1. Selecione se deseja aplicar o valor de um atributo no gerenciador de identidades ao campo Workfront ou se deseja aplicar um valor de constante específico.

1. Informe o nome do campo do gerenciador de identidades que deseja aplicar ou informe o texto do valor constante que deseja aplicar.

1. (Opcional) Para adicionar mais regras para o mesmo campo do Workfront, clique em **Adicionar nova regra** e siga as etapas 4 a 9.

   >[!IMPORTANT]
   >
   > * Qualquer regra abaixo de Sempre será ignorada. Se você tiver uma regra Sempre, mova-a para a parte inferior da lista de regras. Você pode mover regras na lista clicando no menu de três pontos à direita da regra e mover a regra para cima ou para baixo.
   > * Para criar uma regra no meio da lista, clique no menu de três pontos ao lado da regra que você deseja que esteja acima ou abaixo da nova regra e selecione **Adicionar regra acima** ou **Adicionar regra abaixo**.

1. Para excluir uma regra, clique no menu de três pontos ao lado da regra que você deseja excluir e selecione **Excluir**.
1. Para excluir um mapeamento, clique no ícone **Excluir** que está no cartão para esse mapeamento.

1. Para salvar, role até a parte superior da página e clique em **Salvar**.


