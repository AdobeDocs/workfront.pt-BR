---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Listar objetos com um processo de aprovação pendente usando um determinado status
description: Se você tentar excluir um status, uma mensagem de erro poderá informar que ele não pode ser excluído porque está sendo usado em processos de aprovação pendentes em objetos do sistema. Se você quiser localizar e revisar esses objetos para decidir o que precisa fazer, poderá executar um relatório que os liste.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 52dd8750-9a6f-4ac6-9779-ba4ea9b6f4e0
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# Listar objetos com um processo de aprovação pendente usando um determinado status

Se você tentar excluir um status, uma mensagem de erro poderá informar que ele não pode ser excluído porque está em pelo menos um processo de aprovação pendente no sistema. Você pode executar um relatório para listar os objetos onde ele está em um processo de aprovação pendente e, em seguida, decidir o que precisa ser feito para cada um deles.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td>
     <p>Standard</p>
     <p>Plano</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td><p>Editar acesso a relatórios, painéis, calendários</p><p>Editar acesso a Filtros, Visualizações, Agrupamentos</p></td>
  </tr>
  <tr> 
   <td>Permissões de objeto</td> 
   <td>Você obtém permissões de Gerenciamento para os relatórios que criar.</td>
  </tr>
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## No modo Padrão

{{step1-to-reports}}

1. Clique em **Novo Relatório** e selecione **Relatório do Projeto**, **Relatório de Tarefas** ou **Relatório de Problemas**.
1. Abra a guia **Filtros**.
1. Clique em **Adicionar uma Regra de Filtro** e faça o seguinte para configurar a regra:
   1. Comece a digitar `status` e selecione **Status** quando for exibido.
   1. Deixe **Igual** no segundo campo.
   1. Selecione o nome do status no terceiro campo.
1. Clique em **Adicionar uma Regra de Filtro** novamente e faça o seguinte para configurar a regra
   1. Comece a digitar `pending status` e selecione esse item quando ele for exibido sob o tipo de objeto que você está procurando (**Projeto**, **Tarefa** ou **Problema**).
   1. Deixe **Igual** no segundo campo.
   1. Digite `in` no terceiro campo.
1. Clique em **Adicionar uma Regra de Filtro** novamente e faça o seguinte para configurar a regra
   1. Comece a digitar o processo de aprovação e selecione **ID do Grupo** quando ele for exibido em **Processo de Aprovação**.
   1. Selecione **Está em Branco** no segundo campo.
1. Clique em **Salvar + Fechar** para executar o relatório e listar todos os objetos do tipo especificado com processos de aprovação em estado pendente com base no status especificado (**Projeto**, **Tarefa** ou **Problema**).
1. Repita essas etapas para localizar as mesmas informações para os outros dois tipos de objeto.


## No modo de texto

{{step1-to-reports}}

1. Clique em **Novo Relatório** e selecione **Relatório do Projeto**, **Relatório de Tarefas** ou **Relatório de Problemas**.
1. Abra a guia **Filtros**.
1. Selecione **Alternar para Modo de Texto**.
1. Copie e cole o seguinte na janela de edição, substituindo XXX pela chave de 3 letras do status:

   `status=XXX`

   `status_Mod=in`

   `approvalProcess:groupID_Mod=isblank`

   Você pode visualizar a chave na lista de status, conforme mostrado nestes artigos:
   * [Acessar a lista de status de projeto do sistema](project-statuses.md)
   * [Acessar a lista de status de tarefas do sistema](task-statuses.md)
   * [Acessar a lista de status de problemas do sistema](issue-statuses.md)

1. Clique em **Salvar + Fechar** para executar o relatório e listar todos os objetos do tipo especificado com processos de aprovação em estado pendente com base no status especificado (**Projeto**, **Tarefa** ou **Problema**).
1. Repita essas etapas para localizar as mesmas informações para os outros dois tipos de objeto.
