---
content-type: overview
product-area: templates
keywords: substituir,campo,substituído
navigation-topic: templates-navigation-topic
title: Visão geral da anexação de um modelo a um projeto
description: Ao anexar um modelo a um projeto existente, você está modificando algumas informações do projeto de acordo com as do modelo. Algumas das informações sobre o projeto permanecem inalteradas.
author: Alina
feature: Work Management
exl-id: 7f0137b6-ce8e-4b66-ad55-e6dc2aae09d9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 5%

---

# Visão geral da anexação de um modelo a um projeto

Ao anexar um modelo a um projeto existente, você está modificando algumas informações do projeto de acordo com as do modelo. Algumas das informações sobre o projeto permanecem inalteradas.

Para obter informações sobre como anexar um modelo a um projeto, consulte [Anexar um modelo a um projeto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Considerações ao adicionar modelos a projetos

Considere o seguinte ao adicionar modelos a projetos:

* Você pode anexar somente modelos ativos a projetos.
* Você pode anexar um modelo a um projeto quando o projeto está com o status Concluído, Inativo ou Pendente de Aprovação, somente quando o administrador do Adobe Workfront ou um administrador de grupo ativou essa funcionalidade na área Preferências do projeto. Para obter informações sobre como definir preferências de projeto, consulte [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* A menos que você exclua a adição de tarefas de modelo específicas no processo de anexo, todas as tarefas de modelo são adicionadas ao projeto existente.
* A maioria das configurações do modelo é adicionada ao projeto. Algumas configurações do projeto são preservadas. Para obter informações, consulte a seção [Entender as alterações nos campos do projeto ao anexar um modelo](#understand-changes-to-project-fields-when-attaching-a-template) neste artigo.

## Entender as alterações nos campos do projeto ao anexar um modelo {#understand-changes-to-project-fields-when-attaching-a-template}

>[!IMPORTANT]
>
>Anexar um modelo a um projeto não é o mesmo que criar um projeto a partir de um modelo. Ao criar um projeto a partir de um modelo, todos os campos do modelo são transferidos para o novo projeto. Anexar um modelo deixa alguns dos campos do projeto existentes inalterados.

Algumas configurações do modelo são transferidas automaticamente para o projeto, a menos que você as marque especificamente para serem excluídas durante o processo de anexação do modelo. Quando você os marca para serem excluídos, os valores do campo de projeto são preservados.

No entanto, nem todos os campos do projeto estão disponíveis para gerenciamento no processo de anexar um modelo a um projeto. Para obter informações, consulte [Anexar um modelo a um projeto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

A tabela a seguir descreve o padrão para o que acontece com os campos do projeto quando você anexa um modelo e quais campos você pode gerenciar durante o processo de anexação para substituir o comportamento padrão:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Campo</td> 
   <td>O que acontece no processo de anexação de um modelo, por padrão</td> 
   <td>Capacidade de gerenciar as atualizações de campo no processo de anexo </td> 
  </tr> 
  <tr> 
   <td>Descrição</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Status</p> </td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td>Transferido do modelo, se o campo estiver vazio no projeto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Prioridade</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo de condição</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modo de cronograma</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Datas Planejadas</td> 
   <td>Pode mudar com base nas tarefas adicionadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Datas Efetivas</td> 
   <td>Pode mudar com base nas tarefas adicionadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfólio</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programa</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Grupo</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Empresa</td> 
   <td>Transferido do modelo, se o campo estiver vazio no projeto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Horas planejadas</td> 
   <td>Pode mudar com base nas tarefas adicionadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Proprietário do projeto</td> 
   <td>Transferido do modelo, se o campo estiver vazio no projeto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Patrocinador do Projeto</td> 
   <td>Transferido do modelo, se o campo estiver vazio no projeto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gerenciador de Recursos</td> 
   <td>Adicionado à lista de gerentes de recursos existentes no projeto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Forms personalizado</td> 
   <td>Adicionado ao projeto, além dos formulários que já estão no projeto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Orçamento</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Moeda</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>MID</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>EAC</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Benefício Planejado</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Benefício efetivo</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Caminho de Etapas</td> 
   <td>Transferido do modelo, se o campo estiver vazio no projeto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modelo de Término</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modo de conclusão em resumo</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo de atualização</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Agendar</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tempo de folga do usuário</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modo de Nivelamento de Recursos</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risco (campo Projeto)</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Conjuntos de Recursos</td> 
   <td>Adicionado à lista de conjuntos de recursos existentes no projeto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipos de Hora</td> 
   <td> <p>Se essa opção for desmarcada durante o processo de anexação, a configuração de Tipos de horas no projeto permanecerá inalterada. </p> <p>Se selecionada, a configuração do modelo é transferida para o projeto. Se a filtragem de Tipo de Hora estiver definida como Sim no projeto e no modelo, os tipos de hora do modelo serão adicionados aos do projeto.</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p>✓ µ</p> </td> 
  </tr> 
  <tr> 
   <td>Notificações de Lembrete</td> 
   <td> <p>Adicionado à lista de lembretes existentes no projeto. </p> <p>Se desmarcada durante o processo de anexação, as notificações de lembrete do projeto permanecerão inalteradas. </p> </td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Processo padrão de aprovação de tarefas</td> 
   <td>As informações do projeto são preservadas</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Forms Personalizado Padrão de Tarefa</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Esforço do trabalho</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>Permitir que usuários adicionem problemas em linha</span> </td> 
   <td><span>As informações do projeto são preservadas</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Todas as configurações</td> 
   <td>As configurações do modelo substituem as do projeto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tarefas</td> 
   <td>Adicionadas à parte inferior da lista de tarefas, além das tarefas existentes do projeto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Documentos</td> 
   <td>Adicionado ao projeto, além dos documentos existentes do projeto</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Riscos (objetos na área Riscos do projeto)</td> 
   <td>Adicionado ao projeto, além dos riscos existentes do projeto </td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Processo de aprovação</td> 
   <td>Transferido do modelo</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Preços</td> 
   <td> <p>Transferido do modelo, além das taxas de cobrança existentes no projeto. </p> <p>Se houver uma taxa diferente para a mesma função de trabalho no projeto e no modelo, a taxa no projeto permanecerá inalterada. </p> </td> 
   <td> <p> </p> <p>✓ µ</p> </td> 
  </tr> 
  <tr> 
   <td>Registro de cobrança</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Despesas</td> 
   <td>Transferido do modelo, além das despesas existentes no projeto</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Informações financeiras</td> 
   <td> <p>Quando selecionado no processo de anexo, os seguintes campos são transferidos ou adicionados ao projeto: </p> 
    <ul> 
     <li> <p>Custo Fixo</p> <p>Quando a opção é selecionada, o Custo Fixo atualizado do projeto é calculado usando a seguinte fórmula:</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li> 
     <li> <p>Receita com Valor Fixo</p> <p>Quando a opção é selecionada, a Receita fixa atualizada do projeto é calculada usando a seguinte fórmula:</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li> 
     <li> <p>Tipo de custo em tarefas</p> <p>Transferido do modelo</p> </li> 
     <li> <p>Tipo de receita em tarefas</p> <p>Transferido do modelo</p> </li> 
    </ul> <p>Se esse campo for desmarcado durante o processo de anexação, ocorrerá o seguinte:</p> 
    <ul> 
     <li> <p>O custo fixo e a receita fixa do projeto são preservados.</p> </li> 
     <li> <p>Os Tipos de Custo e Receita nas tarefas adicionadas do modelo são definidos como Sem Custo e Não Faturável</p> </li> 
    </ul> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓ µ</p> </td> 
  </tr> 
  <tr> 
   <td>Horas</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Detalhes da Fila, Grupos de Tópicos, Tópicos da Fila, Regras de Encaminhamento</td> 
   <td> <p>Transferido do modelo</p> <p>Se você selecionar a opção <strong>Propriedades da fila e configuração de problemas</strong> durante o processo de anexo, os Detalhes da fila do modelo substituirão os do projeto. Nesse caso, as Regras de Encaminhamento, os Tópicos de Fila e os Grupos de Tópicos do modelo são adicionados àqueles do projeto. <br>Se o projeto estiver configurado como uma fila de solicitações e o modelo anexado ao projeto não estiver configurado como uma fila de solicitações, as informações da fila do projeto serão removidas se você deixar marcada a caixa <strong>Propriedades da fila e Configuração de problemas</strong>. <br>Se você desmarcar a caixa <strong>Propriedades da fila e Configuração de problemas</strong>, todas as configurações da fila do projeto serão preservadas e nenhuma configuração da fila do modelo será anexada.</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓ µ</p> </td> 
  </tr> 
  <tr> 
   <td>Restrições de Tarefa</td> 
   <td> <p>Transferido do modelo </p> <p>Se desmarcada durante o processo de anexação, as restrições da tarefa serão definidas como Assim que possível ou O Mais Tarde Possível, dependendo da configuração Agendar de do projeto. </p> </td> 
   <td> <p> </p> <p> </p> <p style="text-align: center;">✓ µ</p> </td> 
  </tr> 
  <tr> 
   <td>Predecessoras da Tarefa</td> 
   <td> <p>Transferido do modelo</p> <p>Se essa opção for desmarcada durante o processo de anexação, todas as conexões de predecessoras entre as tarefas de modelo serão removidas.</p> </td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Opções de compartilhamento</td> 
   <td> <p>Se essa opção for desmarcada durante o processo de anexação, as permissões do projeto permanecerão inalteradas.</p> <p>Se selecionado durante o processo de anexação, as permissões do modelo são adicionadas ou substituem as do projeto. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Se o Usuário A tiver permissão de Exibição para o projeto, mas tiver permissões de Gerenciamento no modelo, o Usuário A obterá acesso de Gerenciamento ao projeto após anexar o modelo.</p> </td> 
   <td>✓ µ</td> 
  </tr> 
 </tbody> 
</table>

 

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h2> </h2>
<h2>Understand changes to project fields when attaching a template</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and replaced with the table above, per Anna)</p>
-->
<!--
<p>Some template settings automatically transfer to the project, unless you specifically mark them to be excluded during the template attachment process. When you mark them to be excluded, the project field values are preserved. </p> <note type="important">
Not all project fields are available to manage in the process of attaching a template to a project. For information, see
<a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md" class="MCXref xref">Attach a template to a project</a>.
</note>
<p>The following scenarios exist when attaching a template to an existing project: </p>
<ul>
<li> <p><a href="#project-fields-that-are-empty-and-the-template-information-updates-them" class="MCXref xref">Project fields that are empty and the template information updates them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-the-template-information-overwrites-them" class="MCXref xref">Project fields that are populated and the template information overwrites them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-they-remain-unchanged-after-attaching-the-template" class="MCXref xref">Project fields that are populated and they remain unchanged after attaching the template</a> </p> </li>
</ul> <note type="important">
Attaching a template to a project is not the same as creating a project from a template. When you create a project from a template all template fields transfer to the new project. Attaching a template leaves some of the existing project's fields unchanged.
</note>
<p><strong>Project fields that are empty and the template information updates them</strong></p>
<p>Most project fields that are empty are populated with template information when attaching the template to an existing project. </p>
<p><strong>Project fields that are populated and the template information overwrites them</strong></p>
<p>The following fields always overwrite or update existing project information with template information when you attach a template to the project and they cannot be managed during attaching the template: </p>
<ul>
<li> <p><b>Resource manager</b>: The template Resource Managers are added to the list of existing resource managers on the project.</p> </li>
</ul>
<ul>
<li> <p><b>Financial Information</b>: You can indicate whether you want financial information to transfer from the template or to keep the existing financial information on the project in the process of attaching a template. However, when the Financial Information option is selected to indicate that you intend to keep the information from the template, the following fields are updated on the project: </p>
<ul>
<li> <p> The updated Fixed Cost of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li>
<li> <p>The updated Fixed Revenue of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li>
</ul> </li>
</ul>
<ul>
<li> <p><b>Filter Hour Types</b> </p> </li>
</ul>
<ul>
<li> <p><b>Access settings</b> </p> </li>
</ul>
<ul>
<li> <p><b>Custom&nbsp;Forms</b>:&nbsp;Template custom forms are added to the project, in addition to existing project custom forms. If the fields from the template custom forms already exist on the project and contain information, they preserve the information already on the project. You cannot edit them during attaching the template. </p> </li>
</ul>
<ul>
<li> <p><b>Start&nbsp;From</b> </p> </li>
</ul>
<p><strong>Project fields that are populated and they remain unchanged after attaching the template</strong></p>
<p>The following fields remain unchanged on the project, even if they are also populated on the template, and they cannot be managed during attaching the template: </p>
<ul>
<li> <p style="font-weight: bold;">URL</p> </li>
<li> <p style="font-weight: bold;">Project Owner</p> </li>
<li> <p style="font-weight: bold;">Project&nbsp;Sponsor</p> </li>
<li> <p style="font-weight: bold;">Group</p> </li>
<li> <p style="font-weight: bold;">Company</p> </li>
<li> <p style="font-weight: bold;">Currency</p> </li>
<li> <p style="font-weight: bold;">Milestone Path</p> </li>
<li> <p><b>Completion Mode</b> </p> </li>
<li> <p style="font-weight: bold;">Resource Pool</p> </li>
<li> <p style="font-weight: bold;">Tasks Settings fields</p> </li>
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p style="font-weight: bold;">Issue Settings fields</p> </li>
</ul>
</div>
<p>&nbsp;</p>
</div>
-->

 
