---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Alterações na taxa de push de projetos
description: Um cartão de taxa representa o contrato com seu cliente no qual as taxas horárias são definidas para as funções de trabalho que concluirão o trabalho. Em um cartão de taxa, você pode definir várias taxas de cobrança por função de trabalho, com base nos atributos.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c38e60dd-7fb2-4afc-976a-b0966398c162
source-git-commit: 22e8acb748ddc4768dc1724aaa2f515b863ab0cf
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 8%

---

# Alterações na taxa de push em projetos

Quando um cartão de taxas é anexado a um projeto<!--or a staffing plan-->, as taxas no cartão de taxas ainda podem ser ajustadas. Em seguida, você pode enviar essas taxas para os projetos aos quais o cartão de taxa está anexado. Se você não aumentar as novas taxas, as taxas originais permanecerão no projeto.
<!-- and staffing plans -->
<!-- or staffing plan -->

>[!NOTE]
>
>Se uma função de trabalho ou taxa de cobrança do usuário for manualmente substituída no nível do projeto, essa taxa permanecerá no projeto quando as alterações no cartão de taxa forem enviadas para o projeto. Somente as taxas vinculadas ao cartão de taxa são atualizadas.

Para obter informações sobre como anexar um cartão de taxa a um projeto, consulte [Anexar um cartão de taxa a um projeto](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacote</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Padrão]</td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Editar acesso a [!UICONTROL Rate Cards]</td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td>Para editar um cartão de taxa compartilhado com você, é necessário ter permissões de gerenciamento para o cartão de taxa.</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Alterações na taxa de push em projetos

{{step-1-to-setup}}

1. No painel esquerdo, clique em [!UICONTROL **Classificar cartões**].
1. Clique no nome do cartão de taxa na lista Cartões de taxa.
1. Na tela Cartão de tarifa > Funções e taxas de trabalho, verifique se as taxas estão corretas e edite as taxas conforme necessário.
1. Clique em [!UICONTROL **Enviar alterações**].
1. Na caixa de diálogo [!UICONTROL **Aplicar a todos os projetos**], todos os projetos que usam esse cartão de taxa são selecionados por padrão. Se você não quiser que um projeto aplique as alterações de taxa, deverá desmarcá-lo.

   <!--/staffing plans-->
   <!--and staffing plans -->
   <!--or staffing plan -->

   >[!NOTE]
   >
   >Somente projetos com taxas de cartão de taxa desatualizadas são exibidos na caixa de diálogo. Se um projeto usar esse cartão de taxa e as taxas forem atuais no projeto, ele não será exibido.

1. Clique em [!UICONTROL **Salvar**].

   As novas taxas agora são refletidas nos projetos <!--and staffing plans --> que usam o cartão de taxa.
