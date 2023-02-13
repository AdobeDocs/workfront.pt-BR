---
content-type: overview
product-area: templates
keywords: substituir,campo,substituído
navigation-topic: templates-navigation-topic
title: Visão geral de anexar um modelo a um projeto
description: Ao anexar um modelo a um projeto existente, você está modificando algumas das informações do projeto de acordo com as do modelo. Algumas informações sobre o projeto permanecem inalteradas.
author: Alina
feature: Work Management
exl-id: 7f0137b6-ce8e-4b66-ad55-e6dc2aae09d9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1247'
ht-degree: 5%

---

# Visão geral de anexar um modelo a um projeto

Ao anexar um modelo a um projeto existente, você está modificando algumas das informações do projeto de acordo com as do modelo. Algumas informações sobre o projeto permanecem inalteradas.

Para obter informações sobre como anexar um modelo a um projeto, consulte [Anexar um modelo a um projeto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Considerações ao adicionar modelos a projetos

Considere o seguinte ao adicionar modelos a projetos:

* Você pode anexar apenas modelos ativos a projetos.
* Você pode anexar um modelo a um projeto quando ele estiver com o status Concluído, Inativo ou Pendente de Aprovação, somente quando o administrador do Adobe Workfront ou um administrador de grupo tiver habilitado essa funcionalidade na área Preferências do projeto. Para obter informações sobre como definir preferências de projeto, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* A menos que você exclua tarefas de modelo específicas da adição no processo de anexo, todas as tarefas de modelo serão adicionadas ao projeto existente.
* A maioria das configurações de modelo é adicionada ao projeto. Algumas configurações de projeto são preservadas. Para obter mais informações, consulte a seção [Entender as alterações nos campos do projeto ao anexar um modelo](#understand-changes-to-project-fields-when-attaching-a-template) neste artigo.

## Entender as alterações nos campos do projeto ao anexar um modelo {#understand-changes-to-project-fields-when-attaching-a-template}

>[!IMPORTANT]
>
>Anexar um modelo a um projeto não é o mesmo que criar um projeto a partir de um modelo. Ao criar um projeto a partir de um modelo, todos os campos do modelo são transferidos para o novo projeto. Anexar um modelo deixa alguns dos campos do projeto existentes inalterados.

Algumas configurações do modelo são automaticamente transferidas para o projeto, a menos que você as marque especificamente para serem excluídas durante o processo de anexo do modelo. Quando você os marca para serem excluídos, os valores do campo do projeto são preservados.

No entanto, nem todos os campos do projeto estão disponíveis para gerenciamento no processo de anexar um modelo a um projeto. Para obter mais informações, consulte [Anexar um modelo a um projeto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

A tabela a seguir descreve o padrão do que acontece com os campos do projeto quando você anexa um modelo e quais campos você pode gerenciar durante o processo de anexo para substituir o comportamento padrão:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Campo</td> 
   <td>O que acontece no processo de anexação de um template, por padrão</td> 
   <td>Capacidade de gerenciar atualizações de campo no processo de anexo </td> 
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
   <td>Modo de Cronograma</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Datas Planejadas</td> 
   <td>Pode mudar com base nas tarefas adicionadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Datas reais</td> 
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
   <td>Forms personalizada</td> 
   <td>Adicionado ao projeto, além de formulários que já estão no projeto</td> 
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
   <td>Benefício Efetivo</td> 
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
   <td>Modo de conclusão do resumo</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo de Atualização</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Cronograma</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tempo do usuário desligado</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modo de Nivelamento de Recursos</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risco (campo do projeto)</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Conjuntos de Recursos</td> 
   <td>Adicionado à lista de pools de recursos existentes no projeto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipos de Hora</td> 
   <td> <p>Se essa opção for desmarcada durante o processo de anexo, a configuração Tipos de hora no projeto permanecerá inalterada. </p> <p>Se selecionada, a configuração do modelo será transferida para o projeto. Se a filtragem Tipo de hora estiver definida como Sim no projeto e no modelo, os tipos de hora do modelo serão adicionados aos tipos no projeto.</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Notificações de Lembrete</td> 
   <td> <p>Adicionado à lista de lembretes existentes no projeto. </p> <p>Se essa opção for desmarcada durante o processo de anexo, as notificações de lembrete do projeto permanecerão inalteradas. </p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Processo padrão de aprovação de tarefas</td> 
   <td>As informações do projeto são preservadas</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Forms personalizado padrão da tarefa</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Esforço do Trabalho</td> 
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
   <td>Adicionado à parte inferior da lista de tarefas, além das tarefas existentes do projeto</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Documentos</td> 
   <td>Adicionado ao projeto, além dos documentos existentes do projeto</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Riscos (objetos na área Riscos do projeto)</td> 
   <td>Adicionado ao projeto, além dos riscos existentes do projeto </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Processo de aprovação</td> 
   <td>Transferido do modelo</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Preços</td> 
   <td> <p>Transferido do modelo, além das taxas de faturamento existentes no projeto. </p> <p>Se houver uma taxa diferente para a mesma função de trabalho no projeto e no modelo, a taxa no projeto permanecerá inalterada. </p> </td> 
   <td> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Registro de cobrança</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Despesas</td> 
   <td>Transferido do modelo além das despesas existentes no projeto</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Informações financeiras</td> 
   <td> <p>Quando essa opção é selecionada no processo de anexo, os seguintes campos são transferidos ou adicionados ao projeto: </p> 
    <ul> 
     <li> <p>Custo Fixo</p> <p>Quando a opção é selecionada, o Custo Fixo atualizado do projeto é calculado usando a seguinte fórmula:</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li> 
     <li> <p>Receita com Valor Fixo</p> <p>Quando a opção é selecionada, a Receita fixa atualizada do projeto é calculada usando a seguinte fórmula:</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li> 
     <li> <p>Tipo de Custo em tarefas</p> <p>Transferido do modelo</p> </li> 
     <li> <p>Tipo de receita em tarefas</p> <p>Transferido do modelo</p> </li> 
    </ul> <p>Se esse campo for desmarcado durante o processo de anexo, ocorrerá o seguinte:</p> 
    <ul> 
     <li> <p>O Custo Fixo e a Receita Fixa do projeto são preservados.</p> </li> 
     <li> <p>Os Tipos de Custo e Receita nas tarefas adicionadas a partir do modelo são definidos como Sem Custo e Não Faturável</p> </li> 
    </ul> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Horas</td> 
   <td>As informações do projeto são preservadas</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Detalhes da fila, Grupos de tópicos, Tópicos da fila, Regras de roteamento</td> 
   <td> <p>Transferido do modelo</p> <p>Se você selecionar a variável <strong>Configuração de Propriedades e Problemas da Fila</strong> durante o processo de anexo, os Detalhes da fila do modelo substituem os do projeto. Nesse caso, as Regras de roteamento, Tópicos da fila e Grupos de tópicos do modelo são adicionados aos do projeto. <br>Se o projeto estiver configurado como uma fila de solicitações e o modelo anexado ao projeto não estiver configurado como uma fila de solicitações, as informações da fila do projeto serão removidas se você deixar a variável <strong>Configuração de Propriedades e Problemas da Fila</strong> caixa marcada. <br>Se você desmarcar a <strong>Propriedades da fila e configuração de ocorrência</strong> , todas as configurações de Configuração da fila do projeto são preservadas e nenhuma configuração de configuração da fila do modelo é anexada.</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Restrições de tarefa</td> 
   <td> <p>Transferido do modelo </p> <p>Se essa opção for desmarcada durante o processo de anexo, as restrições da tarefa serão definidas como Assim que possível ou Mais tarde possível, dependendo da configuração Agendar a partir do projeto . </p> </td> 
   <td> <p> </p> <p> </p> <p style="text-align: center;">✓</p> </td> 
  </tr> 
  <tr> 
   <td>Predecessoras da Tarefa</td> 
   <td> <p>Transferido do modelo</p> <p>Se essa opção for desmarcada durante o processo de anexo, todas as conexões do antecessor entre as tarefas do modelo serão removidas.</p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Opções de compartilhamento</td> 
   <td> <p>Se essa opção for desmarcada durante o processo de anexo, as permissões do projeto permanecerão inalteradas.</p> <p>Se selecionado durante o processo de anexo, as permissões do modelo são adicionadas ou substituídas às do projeto. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Se o Usuário A tiver permissão de Exibição para o projeto, mas tiver permissões de Gerenciamento no modelo, depois de anexar o modelo, o Usuário A obterá acesso de Gerenciar ao projeto.</p> </td> 
   <td>✓</td> 
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

 
