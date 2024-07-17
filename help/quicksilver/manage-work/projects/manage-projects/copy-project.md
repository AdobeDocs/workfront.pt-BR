---
product-area: projects
navigation-topic: manage-projects
title: Copiar um projeto
description: Você pode copiar um projeto em vez de criá-lo do zero. Você pode copiar apenas um projeto por vez. Não é possível copiar projetos em massa.
author: Alina
feature: Projects, Work Management
role: User
exl-id: 1bb133a8-eb76-46b8-969f-37f57f9453b4
source-git-commit: 79822d258642675331e1998dd3552e3078db41f8
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 4%

---

# Copiar um projeto

<!--
<(LINKED TO THE PRODUCT IN THE COPY PROJECT BOX)</p>
-->

Você pode copiar um projeto em vez de criá-lo do zero. Você pode copiar apenas um projeto por vez. Não é possível copiar projetos em massa.

>[!IMPORTANT]
>
>Os seguintes itens nunca são copiados de um projeto existente para um novo:
>
>* Problemas
>* Preços
>* Registro de cobrança
>* Notas
>* Horas
>* Predecessoras entre projetos
>* Horas orçadas
>
>Os seguintes itens são sempre copiados de um projeto existente para um novo:
>
>* Tarefas
>* Modelo
>* Riscos
>* Informações de Configuração da Fila
>* Portfolio e Programa
>* Scorecard
>* Informações Padrão de Tarefa (Processo de Aprovação Padrão de Tarefa, Forms Personalizado Padrão de Tarefa)
>
> As datas das tarefas originais no projeto copiam para o novo projeto. Você deve alterar a data de início ou de conclusão do projeto (dependendo de seu modo de cronograma) para atualizar as datas nas tarefas. As restrições de tarefa podem impedir que você altere as datas no projeto.

## Requisitos de acesso

<!-- drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Copy</span> projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>View permissions or higher to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>plano do Adobe Workfront*</p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td> <p>Licença da Adobe Workfront*</p> </td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurações de nível de acesso*</strong> </td> 
   <td> <p>Editar acesso aos Projetos com capacidade para Criar <span>e Copiar</span> projetos</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permissões de objeto</strong> </p> </td> 
   <td> <p>Exibir permissões ou superiores para o projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Copiar um único projeto

Copiar um projeto também copia algumas informações do projeto original para o novo projeto. Você também pode especificar quais itens não devem ser copiados para o novo projeto durante o processo de cópia.

Para copiar um projeto:

1. Vá para o projeto que você deseja copiar e clique no ícone **Mais** ![](assets/qs-more-menu.png) à direita do nome do projeto

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Ou

   Vá para uma lista de projetos ou relatório, selecione um projeto e clique no ícone **Mais** ![](assets/qs-more-menu.png) na parte superior da lista.

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. Clique em **Copiar**.

1. Atualize o nome do novo projeto.

   Por padrão, o novo nome é **Cópia de `<Original project name>`.**

   ![](assets/copy-project-box-nwe-350x276.png)

1. Selecione o **Status** do novo projeto.

   Por padrão, o **Status** corresponde ao do projeto original.

1. (Opcional) Desmarque os itens que você não quer copiar para o novo projeto. A tabela a seguir descreve o que acontece quando você desmarca os itens:


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Selecionar tudo</td> 
      <td> <p>Seleciona todas as opções e limpa todos os campos e objetos listados do novo projeto.</p> <p><b>DICA</b>

   Desmarcar <strong>Selecionar tudo</strong> desmarca todos os itens. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Atribuições</td> 
      <td>Remove todas as atribuições de projeto e tarefa</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progresso</td> 
      <td>Remove o progresso de todas as tarefas e elas são exibidas como Novas. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dados personalizados</td> 
      <td> <p>Remove as informações do formulário personalizado no projeto, bem como as informações nos formulários personalizados associados aos seguintes itens:</p> 
       <ul> 
        <li>Tarefas</li> 
        <li>Despesas</li> 
        <li> Documentos</li> 
       </ul> <p><b>Nota</b>

   Os formulários personalizados permanecem anexados às tarefas, despesas, documentos e ao projeto, mas as informações nos campos personalizados dos formulários não são copiadas para o novo projeto. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td> <p>Remove tudo na guia documentos, incluindo versões de documentos, documentos vinculados e pastas.</p> <p>Por padrão, provas e aprovações de documentos não podem ser copiadas para outro projeto. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Todos os predecessores</td> 
      <td> <p>Remove todas as relações predecessoras entre as tarefas do projeto. </p> <p><b>DICA</b>

   Predecessoras entre projetos nunca são transferidas para o novo projeto, independentemente de isso estar selecionado ou não. </p> </td>
   </tr>

<tr> 
      <td role="rowheader">Horas orçadas</td> 
      <td> <p>Remove as horas orçadas na área Planejamento de recursos do Business Case do projeto copiado.</p>

<b>OBSERVAÇÃO</b>

Horas orçadas usando o Planejador de cenários nunca são copiadas para o novo projeto porque o novo projeto não está vinculado a uma iniciativa no Planejador de cenários. Para obter mais informações, consulte <a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md">Recursos de orçamento no Business Case usando o Planejador de cenários</a>
</tr></td>
    <tr> 
      <td role="rowheader">Informações financeiras</td> 
      <td> <p>Remove as informações nas seguintes áreas: </p> 
       <ul> 
        <li>Subguia Finanças do projeto</li> 
        <li> Benefício planejado no Business Case</li> 
        <li>Informações financeiras de todas as tarefas<br></li> 
       </ul> <p>Para obter mais informações sobre a subguia Project Finance, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">Gerenciar informações na área Project Finance</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Processo de aprovação</td> 
      <td>Remove todas as aprovações associadas às tarefas ou ao projeto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificações de Lembrete</td> 
      <td> Remove as Notificações de Lembrete associadas às tarefas ou ao projeto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Despesas</td> 
      <td>Remove despesas associadas às tarefas ou ao projeto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permissões</td> 
      <td> Remove permissões para todos os usuários nas tarefas ou no projeto.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Copiar** para criar uma cópia do projeto.

   Isso cria um novo projeto semelhante ao projeto copiado.

   Você pode começar a fazer alterações no novo projeto copiado, como revisar atribuições de tarefas ou ajustar linhas do tempo.
