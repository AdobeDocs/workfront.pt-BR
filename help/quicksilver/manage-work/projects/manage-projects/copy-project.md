---
product-area: projects
navigation-topic: manage-projects
title: Copiar um projeto
description: Você pode copiar um projeto em vez de criá-lo do zero. Você pode copiar apenas um projeto por vez. Não é possível copiar projetos em massa.
author: Alina
feature: Projects, Work Management
role: User
exl-id: 1bb133a8-eb76-46b8-969f-37f57f9453b4
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 7%

---

# Copiar um projeto

<!--
<(LINKED TO THE PRODUCT IN THE COPY PROJECT BOX)</p>
-->

<!-- Audited: 5/2025 -->

Você pode copiar um projeto de um existente, em vez de criar um do zero, o que ajuda a economizar seu tempo.

Observe que não é possível copiar projetos em massa.

>[!IMPORTANT]
>
>Os seguintes itens nunca são copiados de um projeto existente para um novo:
>
>* Problemas
>* Taxas de cobrança
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
> As datas das tarefas do projeto original serão copiadas para o novo projeto. Você deve alterar a data de início ou de conclusão do projeto (dependendo de seu modo de cronograma) para atualizar as datas da tarefa. As restrições de tarefa podem impedir que você altere as datas no projeto.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.
Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Pacote do Adobe Workfront</p> </td>  
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td> <p>Licença do Adobe Workfront</p> </td> 
   <td> <p>Padrão</p> 
   <p>Plano</p>
      </td> 
  </tr> 
     <td>Configurações de nível de acesso </td> 
   <td> <p>Editar acesso aos Projetos com capacidade para Criar e Copiar projetos</p> </td> 
  </tr>

<td> <p>Permissões de objeto </p> </td> 
   <td> <p>Exibir permissões ou superiores para o projeto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
 
 <table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license</p> </td> 
   <td> <p>New: Standard </p> 
   <p>Or</p>
   <p>Current: Plan </p>
   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level configurations </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Copy</span> projects</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>View permissions or higher to the project</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Copiar um único projeto

Copiar um projeto também copia algumas informações do projeto original para o novo projeto. Você também pode especificar quais itens não devem ser copiados para o novo projeto durante o processo de cópia.

Para copiar um projeto:

{{step1-to-projects}}

1. Selecione o projeto que você deseja copiar da lista de projetos e clique no ícone **Mais** ![Mais menu](assets/more-icon.png) à direita do nome do projeto.

   Ou

   Vá para uma lista de projetos ou relatório, selecione um projeto e clique no ícone **Mais** ![Mais menu](assets/more-icon.png) na parte superior da lista.

1. No menu suspenso **Mais**, clique em **Copiar**. A caixa de diálogo **Cópia de [Nome do Projeto]** é exibida.

1. (Opcional) Atualize o **Nome do Projeto**. Por padrão, o novo nome é **Cópia do [Nome do projeto original]**.

   ![Copiar caixa de projeto](assets/copy-of-project-box.png)

1. Selecione um **Status**. Por padrão, o status do projeto original é selecionado.

1. (Opcional) Desmarque os itens que você não quer copiar para o novo projeto. A tabela a seguir descreve o que acontece quando você desmarca os itens:


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Selecionar tudo</td> 
      <td> <p>Seleciona todas as opções e limpa todos os campos e objetos listados do novo projeto. </p>

   <p> Desmarcar essa opção desmarca todos os itens. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Atribuições</td> 
      <td>Remove todas as atribuições de projeto e tarefa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progresso</td> 
      <td>Remove o progresso de todas as tarefas, exibindo-as como Novas. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dados personalizados</td> 
      <td> <p>Remove as informações do formulário personalizado no projeto, bem como as informações nos formulários personalizados associados aos seguintes itens:</p> 
       <ul> 
        <li>Tarefas</li> 
        <li>Despesas</li> 
        <li> Documentos</li> 
       </ul> 
      <p>Os formulários personalizados permanecem anexados às tarefas, despesas, documentos e projetos, mas as informações nos campos personalizados do formulário não são copiadas para o novo projeto. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td> <p>Remove tudo na guia Documentos, incluindo versões de documentos, documentos vinculados e pastas.</p> <p>Por padrão, provas e aprovações de documentos não podem ser copiadas para outro projeto. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Todos os predecessores</td> 
      <td> <p>Remove todas as relações predecessoras entre as tarefas do projeto. </p> <p>

   Predecessoras entre projetos nunca são transferidas para o novo projeto, independentemente de isso estar selecionado ou não. </p> </td>
   </tr>

<tr> 
      <td role="rowheader">Horas orçadas</td> 
      <td> <p>Remove as horas orçadas na área Planejamento de recursos do Business Case do projeto copiado.</p> 
    <p>
   Horas orçadas usando o Planejador de cenários nunca são copiadas para o novo projeto porque o novo projeto não está vinculado a uma iniciativa no Planejador de cenários. Para obter mais informações, consulte <a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md">Recursos de orçamento no Business Case usando o Planejador de cenários</a></p>
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

1. Clique em **Copiar projeto**. O projeto copiado é criado.
