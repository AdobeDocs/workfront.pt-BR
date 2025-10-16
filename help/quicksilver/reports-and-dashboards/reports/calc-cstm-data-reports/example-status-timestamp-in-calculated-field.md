---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 'Exemplo de campo personalizado calculado: exibir um carimbo de data e hora de Status em um Formulário personalizado'
description: O campo calculado a seguir exibe a data em que o status do objeto é marcado como Em Andamento (INP). É possível usar as mesmas informações para campos personalizados calculados para problemas, tarefas ou projetos.
author: Jenny
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Exemplo de campo personalizado calculado: exibir um carimbo de data e hora de Status em um formulário personalizado

O campo calculado a seguir exibe a data em que o status do objeto é marcado como Em Andamento (INP). É possível usar as mesmas informações para campos personalizados calculados para problemas, tarefas ou projetos.

>[!NOTE]
>
>Se o status do objeto mudar para INP, ele mudar para outro status e, em seguida, de volta para INP, o Adobe Workfront capturará somente o carimbo de data e hora da primeira alteração para INP.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Pacote do Adobe Workfront</p> </td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td> <p>Licença do Adobe Workfront</p> </td> 
   <td>
      <p>Standard</p>
      <p>Plano</p></td>
  </tr> 
  <tr> 
   <td><p>Configurações de nível de acesso</p></td> 
   <td> <p>Editar acesso para Criar relatórios, painéis e calendários</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permissões de objeto</p> </td> 
   <td> <p>Gerenciar permissões no objeto ao qual o formulário está anexado</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
