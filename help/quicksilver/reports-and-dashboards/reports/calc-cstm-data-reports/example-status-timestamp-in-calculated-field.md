---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: "Exemplo de campo personalizado calculado: exibir um carimbo de data e hora de Status em um Formulário personalizado"
description: O campo calculado a seguir exibe a data em que o status do objeto é marcado como Em Andamento (INP.) É possível usar as mesmas informações para campos personalizados calculados para problemas, tarefas ou projetos.
author: Nolan
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: ecafbd693237427d727b15dd22afd485b4e59c72
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# Exemplo de campo personalizado calculado: exibir um carimbo de data e hora de Status em um formulário personalizado

O campo calculado a seguir exibe a data em que o status do objeto é marcado como Em Andamento (INP.) É possível usar as mesmas informações para campos personalizados calculados para problemas, tarefas ou projetos.

>[!NOTE]
>
>Se o status do objeto mudar para INP, ele mudar para outro status e, em seguida, de volta para INP, o Adobe Workfront capturará somente o carimbo de data e hora da primeira alteração para INP.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>plano do Adobe Workfront*</p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td> <p>Licença da Adobe Workfront*</p> </td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Configurações de nível de acesso*</strong> </td> 
   <td> <p>Editar acesso para Criar relatórios, painéis e calendários</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Permissões de objeto</strong> </p> </td> 
   <td> <p>Gerenciar permissões no objeto ao qual o formulário está anexado</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.<br>Para obter mais informações sobre permissões para painéis, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">Compartilhar relatórios, painéis e calendários </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Pré-requisito

Para adicionar um campo calculado que exibe o histórico de edição de um campo a um formulário personalizado, primeiro crie o formulário personalizado.

## Exibir carimbo de data e hora de status em um formulário personalizado

1. Vá para um formulário personalizado no qual deseja adicionar o campo.
1. Clique em **Calculado** para adicionar um campo personalizado calculado ao formulário.
1. Digite um **Rótulo** para o campo personalizado. Por exemplo, &quot;Campo personalizado do carimbo de data e hora do status&quot;.
1. Clique em **Salvar+Fechar**.
1. Reabra o formulário personalizado e selecione o novo **Campo Personalizado de Carimbo de Data/Hora de Status** no formulário.
1. Na caixa **Cálculo**, copie e cole o seguinte cálculo para o seu campo personalizado:

   ```
   IF({status}='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})  
   ```

   >[!NOTE]
   >
   >Esse cálculo é idêntico para todos os objetos e status. Você sempre deve usar a chave de três letras, e não o nome do status para o status do objeto neste cálculo.
   >
   >Para obter mais informações sobre as chaves para Status, consulte [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Clique em **Salvar+Fechar**.

   Agora é possível relatar o Campo Personalizado Carimbo de Data e Hora do Status ou usá-lo em outros cálculos, em relatórios ou em campos personalizados.
