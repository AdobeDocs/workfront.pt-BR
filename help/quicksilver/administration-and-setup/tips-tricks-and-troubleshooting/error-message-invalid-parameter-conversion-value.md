---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Mensagem de erro: Parâmetro inválido: valor de conversão'
description: "Você recebe a seguinte mensagem de erro ao tentar alterar o Formato de um Campo Personalizado em um Formulário Personalizado existente: 'Parâmetro inválido: valor de conversão `&lt;..&gt;`'"
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 1%

---

# Mensagem de erro: Parâmetro inválido: valor de conversão

## Problema

Você recebe a seguinte mensagem de erro ao tentar alterar o Formato de um Campo Personalizado em um Formulário Personalizado existente: &quot;Parâmetro inválido: valor de conversão &quot;&lt;..>&quot;&quot;\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## Causa

Essa mensagem ocorre no seguinte cenário:

Por exemplo, você tem um Campo personalizado formatado como Texto.  Agora, é necessário alterar o Formato do campo personalizado para Moeda. Em algum lugar do seu [!DNL Adobe Workfront] , esse campo já está anexado a um objeto e tem informações já especificadas nele. As informações existentes em pelo menos um desses campos já estão formatadas como Texto. Portanto, o Formato do campo não pode ser alterado para Moeda.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans" target="_blank">[!DNL Workfront] plano</a>*</p> </td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] visão geral das licenças</a>*</p> </td> 
   <td>Plano</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Nível de acesso*</strong> </td> 
   <td> <p>Editar acesso a:</p> 
    <ul> 
     <li> <p>Criar relatórios, painéis e calendários</p> </li> 
     <li> <p>Criar filtros, visualizações e agrupamentos</p> </li> 
    </ul> <p><b>OBSERVAÇÃO</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solução

Faça o seguinte:

1. Crie relatórios para todos os objetos que podem ter esse campo associado ao Forms personalizado.\
   Para obter informações sobre como criar um relatório, consulte [Criar um relatório personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Inclua o Campo personalizado que você está tentando editar na visualização do relatório para que você possa ver qual objeto tem esse campo preenchido com um valor de texto.
1. Corrija os valores do Campo personalizado dos objetos que são exibidos em um formato de texto e atribua a eles um valor formatado como Moeda; em seguida, tente alterar o campo Formato no Formulário personalizado novamente.\
   Ou\
   Se você tiver muitos valores de campo já preenchidos com informações formatadas em texto, considere adicionar um novo Campo personalizado ao seu Formulário personalizado e formatá-lo como Moeda.
