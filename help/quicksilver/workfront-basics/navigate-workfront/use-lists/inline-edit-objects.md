---
product-area: projects
navigation-topic: use-lists
title: Itens de edição em linha em uma lista em [!DNL Adobe Workfront]
description: É possível editar objetos em linha ao exibi-los em uma lista ou relatório. Quando você edita as informações sobre objetos exibidos em uma lista ou relatório, o objeto é atualizado imediatamente.
feature: Get Started with Workfront
author: Lisa
exl-id: a94b5aaf-71de-4fcd-946b-459ca3edf7e4
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# Itens de edição em linha em uma lista em [!DNL Adobe Workfront]

É possível editar objetos em linha ao exibi-los em uma lista ou relatório. Quando você edita as informações sobre objetos exibidos em uma lista ou relatório, o objeto é atualizado imediatamente.

Ao editar em linha um campo contido em um formulário personalizado que não está anexado ao objeto, o formulário personalizado é adicionado automaticamente ao objeto. Se o campo existir em vários formulários personalizados, o formulário personalizado que foi atualizado recentemente será anexado ao objeto.

Para obter mais informações sobre listas, consulte [Introdução a listas em [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

Enquanto a maioria dos objetos exibidos em listas ou relatórios é editável em linha no [!DNL Adobe Workfront], há algumas limitações, que incluem:

* Não é possível editar campos calculados ou [!DNL Workfront] campos incorporados que são cálculos.
* Só é possível editar campos associados diretamente aos objetos na lista. Não é possível editar campos que pertencem a objetos associados aos objetos na lista.\
   Por exemplo, você pode editar o status de uma tarefa em um relatório de Tarefa, mas não pode editar o nome do projeto ao qual a tarefa está associada no mesmo relatório. É possível editar o nome do projeto somente em um relatório de Projeto .
* Não é possível editar campos em linha quando a exibição de uma lista não está exibindo a moeda padrão.\
   Para obter informações sobre como exibir a moeda padrão, consulte a seção [Editar relatórios com moedas exclusivas](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md#editing-reports-with-unique-currencies) no artigo [Criar relatórios de dados financeiros com taxas de câmbio exclusivas](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

* Não é possível editar sinalizadores e ícones exibidos em uma lista.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Review] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Acesso à [!UICONTROL Editar] para a área em que a lista está</p> <p>Por exemplo, para embutir tarefas de edição em um projeto, é necessário ter acesso ao [!UICONTROL Editar] para Projetos.</p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso.<br>Para obter informações sobre como uma [!DNL Workfront] administrador pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>[!UICONTROL Gerenciar]</p> <p>Você também deve ter permissões para editar determinados campos, como campos personalizados, status, etc.</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Editar objetos em linha

1. Vá para uma lista de objetos que deseja editar em linha.

   A lista deve exibir campos que pertencem aos objetos ou campos que pertencem aos objetos associados aos objetos na lista.

1. Localize o objeto que deseja editar e clique em qualquer campo da lista.

   >[!TIP]
   >
   >Se você tiver várias páginas, poderá localizar um objeto usando:
   >
   >   
   >   
   >   * **Paginação**: Clique nas setas para trás e para a frente para navegar entre as páginas.\
      >     Localizada no canto inferior direito da lista, a variável [!UICONTROL paginação] A área permanece aderente à medida que você percorre a lista.
   >   * **Filtro rápido**: Clique no ícone de filtro ou digite Alt+F para abrir o filtro rápido, em seguida, insira o texto para exibir somente os itens que contêm o texto inserido.\
      >     O filtro rápido está localizado na barra de ferramentas da lista. Para obter mais informações, consulte [Aplicar o filtro rápido a uma lista](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).



   Se o campo puder ser editado, isso transformará o campo e todos os outros campos exibidos na lista em células editáveis.

   ![](assets/nwe-editable-cells-350x131.png)

1. Edite as informações dentro desta célula e pressione [!UICONTROL Enter].

   >[!NOTE]
   >
   >Se um campo personalizado tiver sido configurado para permitir a formatação, é possível negrito, itálico ou sublinhado ao editar o campo em linha em uma lista atualizada.\
   >Para obter informações sobre como configurar a formatação de um campo personalizado, consulte [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).\
   >Para obter informações sobre listas atualizadas, consulte a seção &quot;A diferença entre as listas atualizadas e herdadas&quot; no artigo [Introdução a listas em [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. Press [!UICONTROL Tabulação] para mover para a próxima célula editável.
1. (Condicional) Se não conseguir salvar suas edições e a célula estiver contornada em vermelho, clique dentro do campo para revisar a mensagem de validação que é exibida ao lado da célula e fazer as atualizações apropriadas.

   Geralmente, isso acontece quando o formato incorreto é usado ou um campo obrigatório é deixado em branco.

1. Depois de concluir a modificação de todas as células, prima [!UICONTROL Enter] para salvar as alterações.
