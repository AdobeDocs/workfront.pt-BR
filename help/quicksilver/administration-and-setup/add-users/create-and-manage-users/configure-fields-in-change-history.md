---
user-type: administrator
product-area: system-administration;setup
title: Configurar campos para rastrear no histórico de alterações
description: Como administrador do Workfront, você pode configurar quais campos de objeto e ações o Workfront rastreia.
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 71bd341da0b506429ab25726ae3be82829034f9f
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 9%

---

# Configurar campos para rastrear no histórico de alterações

{{highlighted-preview-article-level}}

O Adobe Workfront gera atualizações automáticas do sistema para registrar os seguintes eventos:

* Alterações feitas pelos usuários em um campo de objeto
* Ações executadas por usuários em um objeto

Essas atualizações do sistema incluem o seguinte tipo de informação:

* A alteração que foi feita
* O nome do usuário que fez a alteração
* A hora e a data da alteração

Como administrador do Workfront, você pode configurar quais campos de objeto e ações o Workfront rastreia.

Por exemplo, você pode fazer com que o Workfront rastreie todas as alterações que os usuários fazem nos nomes de problemas em todo o sistema. Qualquer alteração no nome do problema será exibida como uma entrada no log de histórico de alterações. Para obter mais informações, consulte [Exibir e gerenciar o histórico de alterações](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacote</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Padrão]</td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Administrador do sistema</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Limites para rastreamento de campo

Os limites para o número de campos que você pode rastrear são definidos pelo seu pacote do Workfront.

| Pacote do Workfront | Número máximo de campos rastreados |
|---------|----------|
| Selecionar | 700 |
| Prime | 3000 |
| Ultimate | 5000 |
| Workflow Select | 1000 |
| Workflow Prime | 5000 |
| Workflow Ultimate | Ilimitado |

## Adicionar campos que você deseja rastrear

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Controle de alterações > Configuração**.
1. Na tela Configuração, clique em **Adicionar campo**.
1. Na caixa **Adicionar campos**, selecione um objeto. Você pode começar a digitar o nome do objeto e, em seguida, selecioná-lo quando ele aparecer na lista.
1. Em seguida, selecione os nomes de campo que deseja rastrear para esse objeto. Você pode começar a digitar o nome do campo e, em seguida, selecioná-lo quando ele aparecer na lista.

   Tanto os campos personalizados quanto os campos nativos estão disponíveis para o objeto.
   Os campos que já estão sendo rastreados são mostrados como selecionados na lista.

   ![Adicionar campos para controle de alterações](assets/change-history-config-add-fields.png)

1. Depois de selecionar todos os campos que deseja rastrear, clique em **Adicionar**.

   Os campos são adicionados à lista Campos rastreados.

## Remova os campos que não deseja mais rastrear

Você pode remover campos que não deseja que o sistema rastreie para um tipo específico de objeto em toda a interface do Workfront.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Controle de alterações > Configuração**.
1. Na tela Configuração, selecione o campo ou os campos que deseja interromper o rastreamento.

   Você pode ver o mesmo nome de campo mais de uma vez. Os campos são agrupados por objeto para que você possa localizar o campo correto. Você também pode usar a caixa de pesquisa na parte superior da tela.

1. Selecione **Excluir** na barra de ações na parte inferior da tela.
1. Clique em **Remover** na mensagem de confirmação.

   Os campos são removidos da lista Campos rastreados.


