---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Desativar ou reativar uma empresa
description: É possível desativar uma empresa que não é mais usada, mantendo todos os dados históricos associados a ela. Se você desativar uma empresa já em uso em algum lugar no sistema, ela continuará a funcionar da mesma forma que sempre funcionou. Ele não é removido ou bloqueado.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
TQID: https://experienceleague.adobe.com/GrxcFYKSrmJsaITu6twBnTZxfkMcvsnRdfn7-qoSXI4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 335
ht-degree: 12%

---

# Desativar ou reativar uma empresa

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

É possível desativar uma empresa que não é mais usada, mantendo todos os dados históricos associados a ela. Se você desativar uma empresa já em uso em algum lugar no sistema, ela continuará a funcionar da mesma forma que sempre funcionou. Ele não é removido ou bloqueado.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] pacote</p> </td> 
   <td><p>Qualquer</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licença</p> </td> 
   <td><p>[!UICONTROL Plan]</p>
   <p>[!UICONTROL Padrão]</p>
   </td> 
  </tr>
  <tr> 
   <td>Configurações de nível de acesso</td> 
  <td> <p>Você deve ter um dos seguintes:</p> 
    <ul> 
     <li> <p>O nível de acesso do [!UICONTROL System Administrator], que permite editar qualquer empresa no sistema.</p> </li> 
     <li> <p>Acesso administrativo para gerenciar empresas, que permite editar qualquer empresa no sistema.</p> </li> 
    </ul> <p><b>NOTA</b>:
     <ul> 
      <li> <p>Você também pode gerenciar empresas associadas a qualquer grupo ao qual esteja atribuído como administrador de grupo.</p> </li> 
      <li> <p>Para adicionar e remover usuários do sistema [!DNL Workfront], você deve ter um dos seguintes:</p> 
       <ul> 
        <li> <p>O nível de acesso do [!UICONTROL System Administrator]. </p> </li> 
        <li> <p>Configuração de <b>[!UICONTROL Usuários]</b> em seu nível de acesso configurada para <b>[!UICONTROL Editar]</b> acesso, com <b>[!UICONTROL Criar]</b> e pelo menos uma das duas opções <b>[!UICONTROL Administrador de Usuários]</b> habilitadas em <b>[!UICONTROL Ajustar suas configurações]</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Dessas duas opções, se <b>[!UICONTROL Usuário Admin (Usuários de Grupo)]</b> estiver habilitado, você deverá ser um administrador de grupo de um grupo do qual o usuário seja membro.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td>
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Desativar ou reativar uma empresa

{{step-1-to-setup}}

1. No painel esquerdo, clique no ícone **[!UICONTROL Empresas]** ![Empresas](assets/companies-icon-left-panel.png).

1. Selecione uma ou mais empresas para desativar ou reativar.
1. Clique em **[!UICONTROL Editar]**.<!--MAKE THIS A SEPARATE NUMBERED LINE<span class="preview">(Conditional) In the Preview environment, disable the **[!UICONTROL Is Active]** option to deactivate it, or enable the option to activate it.</span>-->
1. Para uma única empresa, desabilite a opção **[!UICONTROL Está ativo]** para desativá-lo ou habilite a opção para ativá-lo. <!--ADD TO THE FRONT OF THIS SENTENCE In the Production environment, -->

   Ou

   Para várias empresas, selecione **[!UICONTROL Não]** no menu suspenso **[!UICONTROL Está ativo]** para desativá-las ou **[!UICONTROL Sim]** para ativá-las.

1. Clique em **[!UICONTROL Salvar alterações]**.
