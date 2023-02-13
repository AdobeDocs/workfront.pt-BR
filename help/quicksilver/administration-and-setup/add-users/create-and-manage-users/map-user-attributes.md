---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Mapear atributos do usuário e provisionar novos usuários automaticamente
description: Usando o logon único (SSO), você pode passar atributos do Ative Diretory do seu provedor de identidade para os usuários do Adobe Workfront. Você também pode adicionar novos usuários ao Workfront usando a opção Provisionamento automático (também chamada de Provisionamento just in time ou JIT).
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 3%

---

# Mapear atributos do usuário e provisionar novos usuários automaticamente

Usando o logon único (SSO), você pode passar atributos do Ative Diretory do seu provedor de identidade para os usuários do Adobe Workfront. Você também pode adicionar novos usuários ao Workfront usando a opção Provisionamento automático (também chamada de Provisionamento just in time ou JIT).

>[!NOTE]
>
>Isso não estará disponível se sua organização tiver sido integrada à Adobe Admin Console. Consulte seu administrador de rede ou de TI se precisar de mais informações.


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

## Dicas para mapear atributos

Lembre-se do seguinte ao mapear atributos:

* Sempre teste em uma sandbox de Visualização ou em uma sandbox de Atualização do cliente (CR).
* Teste com contas de administrador e não administrador para confirmar que você está mapeando atributos corretamente.
* Os atributos são mapeados sempre que um usuário entra no Workfront por SSO, não apenas durante o provisionamento automático.

## Mapear atributos do usuário e provisionar novos usuários automaticamente

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema** > **Logon único (SSO)**.

1. No **Tipo** , clique em **SAML 2.0**.

1. Clique em **Mapear atributos do usuário**.

   ![](assets/map-user-attributes.png)

1. (Opcional) Se quiser que o Workfront crie novos usuários a partir do seu Ative Diretory automaticamente, clique em **Provisionamento automático para o usuário**.

   Esse recurso requer mapeamento de atributo.

1. Na linha de opções exibida, mapeie os atributos necessários para os usuários do Workfront.

   Você pode mapear atributos como Endereço, Gerente, Função do trabalho, Grupo inicial e assim por diante.

   Os mapeamentos de atributo funcionam em uma Taxa 1:1. Por exemplo, não é possível definir todos os grupos aos quais um usuário pertence; você pode definir somente um por usuário.

   >[!IMPORTANT]
   >
   >Os atributos a seguir são necessários para cada usuário:
   >      
   >* Nome
   >* Sobrenome
   >* Endereço de email

   >      
   >Não recomendamos mapear Níveis de Acesso nos Mapeamentos de Atributo. Em caso afirmativo, tenha cuidado ao definir o valor padrão para garantir que você não remova o Acesso de administrador inadvertidamente.

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
      <td>Digite o rótulo do atributo SSO que deseja usar./td&gt; 
     </tr> 
     <tr> 
      <td role="rowheader">Valor Padrão</td> 
      <td> <p>Depois de escolher um Atributo de usuário do Workfront, se o valor for NULL durante a conexão, esse campo preencherá com o valor padrão correspondente no sistema. Digite um valor aqui somente se planeja aplicar as regras de mapeamento de atributos (consulte a etapa 7). O valor padrão atua como uma exceção para essas regras.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Clique em **Regras** para adicionar uma regra ao atributo.

   1. Na lista suspensa, escolha o modificador de atributo que deseja usar.
   1. Nos 2 campos à direita, digite o valor do atributo do diretório e o valor com o qual deseja substituí-lo.

      ![](assets/rule-fields.png)
   Você pode clicar em **Adicionar regra** para adicionar mais regras ao atributo.

1. (Opcional) Para mapear mais atributos de usuário, clique em **Adicionar mapeamento** e repita os passos 6-7.
1. Clique em **Salvar**.
