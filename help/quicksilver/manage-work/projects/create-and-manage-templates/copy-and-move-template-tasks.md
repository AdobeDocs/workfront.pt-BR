---
product-area: templates
navigation-topic: templates-navigation-topic
title: Copiar e mover tarefas de modelo
description: Você pode copiar ou mover uma tarefa de modelo para o mesmo modelo ou para outro modelo.
author: Alina
feature: Work Management
exl-id: a2e09e63-5c88-460c-9996-3a39fbb82150
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '2140'
ht-degree: 3%

---

# Copiar e mover tarefas de modelo

Você pode copiar uma tarefa de modelo de um modelo para outro modelo ou movê-la para outro modelo ou para outro local no mesmo modelo.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a modelos</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um modelo e para a tarefa de modelo </p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront.

## Considerações para copiar ou mover tarefas de modelo

Considere o seguinte ao copiar tarefas de modelo:

* As seguintes informações não são transferidas para a tarefa copiada:

   * Etapas

* Você tem a chance de optar por copiar alguns itens associados à tarefa de modelo para a tarefa copiada durante o processo de cópia. No entanto, por padrão, os seguintes objetos não são transferidos para a tarefa copiada:

   * Comentários do usuário

* Formulários personalizados são copiados com a tarefa de modelo quando você copia uma tarefa de modelo. As informações nos campos personalizados são transferidas para a nova tarefa de modelo somente quando você seleciona copiar Dados personalizados.

* Os itens a seguir são transferidos para a tarefa de modelo copiada por padrão:

   * Subtarefas

Considere o seguinte ao mover tarefas de modelo:

* As seguintes informações são transferidas para a tarefa movida, por padrão:

   * Formulários personalizados e informações de campos personalizados
   * Subtarefas
   * Comentários do usuário

* As seguintes informações não são transferidas para a tarefa movida:

   * Etapas.

## Copiar modelos de tarefa

Você pode copiar uma única tarefa de modelo ou pode copiar várias tarefas de modelo em massa.

1. Vá para o modelo que contém a tarefa de modelo ou as tarefas de modelo que você deseja copiar.
1. Clique em **Tarefas de modelo** no painel esquerdo.
1. Siga um destes procedimentos:
   * Clique no nome de uma tarefa de modelo para abri-la.
   * Selecione uma ou várias tarefas de modelo na lista.
1. (Condicional) Clique no ícone ![Mais **do menu** Mais](assets/more-icon.png) na parte superior da lista de tarefas de modelo ou à direita do nome da tarefa de modelo, se você tiver aberto a tarefa. Em seguida, clique em **Copiar para** ou **Copiar**, dependendo de onde você está acessando a opção Copiar.
A caixa Copiar Modelo de Tarefa é aberta.
   ![Caixa de tarefa de modelo de CPU](assets/copy-template-task-box-unshimmed.png)
1. (Opcional) Renomeie a tarefa de modelo no campo **Nome da Tarefa de Modelo**.

   >[!TIP]
   >
   >Este campo fica esmaecido e não pode ser editado ao selecionar para copiar várias tarefas de modelo em uma lista. Você pode passar o mouse sobre o campo Nome do Modelo de Tarefa e uma lista de todas as tarefas de modelo selecionadas é exibida.

1. Comece digitando o nome do **Modelo de Destino** para o qual você deseja copiar a tarefa de modelo no campo **Selecionar Modelo de Destino** e selecione-o quando ele for exibido na lista.

   O nome do modelo atual é exibido por padrão. Se quiser copiar a tarefa de modelo no mesmo modelo, deixe esse campo inalterado.

   >[!TIP]
   >
   >Você também pode começar a digitar o Número de referência ou inserir a ID do modelo. Isso pode ajudá-lo a distinguir entre modelos com nomes idênticos.

1. (Condicional) Clique em **solicitar acesso** para solicitar acesso ao modelo de destino, caso não tenha acesso ao modelo selecionado.
1. (Condicional) Continue a copiar a tarefa de modelo para o modelo de destino selecionado sem solicitar acesso se tiver acesso para adicionar tarefas de modelo a uma das tarefas de modelo no modelo de destino.

1. Clique em **Opções** no painel esquerdo e desmarque os atributos de tarefa de modelo que você não deseja copiar com a tarefa de modelo. Todas as opções são selecionadas por padrão.

   >[!TIP]
   >
   >Desmarcar **Selecionar tudo** desmarca todas as opções.

   Desmarque as opções a seguir para não transferi-las para a tarefa de modelo copiada. A tabela a seguir descreve o que acontece quando as opções são desmarcadas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Selecionar tudo</td> 
      <td>Desmarque essa opção para remover todas as informações da tarefa de modelo ao copiá-las para seu novo local. </td> 
     </tr>
     <tr> 
      <td role="rowheader">Dt Restr</td> 
      <td> <p>A restrição da tarefa de modelo é definida como O Mais Breve Possível ou O Mais Tarde Possível com base na configuração do Modo de Agendamento do modelo.</p> <p> Quando selecionada, a restrição atual da tarefa de modelo é transferida para a tarefa de modelo copiada. </p> 
      <p><b>Nota</b>

   Ao copiar uma tarefa de modelo com restrições específicas de data para outro modelo e as datas de restrição da tarefa de modelo estiverem fora das datas do novo modelo, a Restrição da tarefa de modelo será alterada para O Mais Breve Possível ou O Mais Tarde Possível ou as datas de Início Planejado ou de Conclusão Planejada dos modelos serão ajustadas.

   Veja a seguir exemplos de restrições específicas de data:
   <ul>
      <li> Precisa Iniciar Em</li>
      <li> Precisa Terminar Em</li>
      <li> Não Iniciar Antes De</li>
      <li> Não Iniciar Depois De</li>
      </ul>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Atribuições</td> 
      <td> <p>Todas as atribuições são removidas da tarefa de modelo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Processo de aprovação</td> 
      <td>Todos os processos de aprovação são removidos da tarefa de modelo.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Todos os predecessores</td> 
      <td> <p>Isso significa que as dependências não continuarão para as tarefas de modelo copiadas. </p> <p>Quando selecionada, as predecessoras dentro do grupo de tarefas de modelo copiadas são preservadas, outras são excluídas.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Dados personalizados</td> 
      <td> <p>Os valores dos campos personalizados são apagados e os formulários personalizados são transferidos para a tarefa de modelo copiada. </p> <p>Quando selecionados, os formulários e os valores dos campos personalizados são transferidos para a tarefa de modelo copiada. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Informações financeiras</td> 
      <td>As informações financeiras da tarefa de modelo copiada são removidas e o Workfront atualiza o Tipo de Custo da tarefa de modelo para Sem Custo e o Tipo de Receita da tarefa de modelo como Não Faturável.
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td> <p>Os documentos anexados à tarefa de modelo não são transferidos para a tarefa de modelo copiada. Isso inclui versões, provas e documentos vinculados.</p> <p><b>Nota</b></p>

   <p>Isso não inclui aprovações de documentos. Aprovações de documentos nunca podem ser copiadas quando uma tarefa de modelo é copiada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificações de Lembrete</td> 
      <td>Os lembretes de tarefas de modelo não são transferidos para a tarefa de modelo copiada. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Despesas</td> 
      <td>As despesas registradas na tarefa de modelo não são transferidas para a tarefa de modelo copiada. </td> 
     </tr>  
    </tbody> 
   </table>


1. (Opcional) Clique em **Selecionar pai** no painel esquerdo e selecione a tarefa de modelo no modelo de destino que você deseja que se torne a principal da tarefa de modelo copiada.

   >[!TIP]
   >
   >Ao selecionar para copiar várias tarefas de modelo em uma lista, todas as tarefas de modelo selecionadas se tornam as tarefas filho do pai selecionado e são adicionadas após as tarefas filho existentes.

   Selecione um pai seguindo um destes procedimentos:

   * Na lista de tarefas de modelo, selecione um dos pais no plano de modelo.
   * Clique no ícone de pesquisa ![Ícone de pesquisa](assets/search-icon.png) e procure uma tarefa de modelo pai por nome.

   A tarefa de modelo deve aparecer na lista.

1. Selecione o botão de opção do pai depois de encontrá-lo.

   Se você não selecionar uma tarefa de modelo pai, as tarefas de modelo serão copiadas como tarefas de modelo principais em vez de subtarefas e serão colocadas no final da lista de tarefas de modelo no modelo de destino.

1. Clique em **Copiar Tarefa de Modelo**.

   As tarefas de modelo copiadas agora estão no modelo especificado e são subtarefas da tarefa de modelo pai selecionada ou as últimas tarefas de modelo no modelo.


## Mover tarefas de modelo

Você pode mover uma tarefa de modelo para outra tarefa de modelo no mesmo modelo ou para outro modelo. Você pode mover uma ou várias tarefas de modelo em massa.

1. Vá para o modelo que contém a tarefa de modelo ou as tarefas de modelo que você deseja mover.
1. Clique em **Tarefas de modelo** no painel esquerdo.
1. Siga um destes procedimentos:
   * Clique no nome de uma tarefa de modelo para abri-la.
   * Selecione uma ou várias tarefas de modelo na lista.
1. (Condicional) Clique no menu **Mais** ![Ícone Mais](assets/more-icon.png) na parte superior da lista de tarefas de modelo ou à direita do nome da tarefa de modelo, se você tiver aberto a tarefa, e clique em **Mover para** ou **Mover**, dependendo de onde você está acessando a opção Mover.
A caixa Mover Modelo de Tarefa é aberta.
   ![Mover caixa de tarefa de modelo](assets/move-template-task-box-unshimmed.png)

1. (Opcional) Renomeie a tarefa de modelo no campo **Nome da Tarefa de Modelo**.

   >[!TIP]
   >
   >Este campo fica esmaecido e não pode ser editado ao selecionar para mover várias tarefas de modelo em uma lista. Você pode passar o mouse sobre o campo Nome da tarefa de modelo e uma lista de todas as tarefas de modelo selecionadas é exibida.

1. Comece digitando o nome do **Modelo de Destino** para onde você deseja mover a tarefa de modelo no campo **Selecionar Modelo de Destino** e selecione-o quando ele for exibido na lista.

   >[!TIP]
   >
   >Você também pode começar a digitar o Número de referência ou inserir a ID do modelo. Isso pode ajudá-lo a distinguir entre modelos com nomes idênticos.

1. (Condicional) Clique em **solicitar acesso** para solicitar acesso ao modelo, caso não tenha acesso ao modelo de destino.
1. (Condicional) Continue movendo a tarefa de modelo para o modelo de destino selecionado sem solicitar acesso se tiver acesso para adicionar tarefas de modelo a uma das tarefas de modelo no modelo de destino.

1. Clique em **Opções** no painel esquerdo e desmarque os atributos de tarefa de modelo que você não deseja copiar com a tarefa de modelo. Todas as opções são selecionadas por padrão.

   >[!TIP]
   >
   >* A seção Opções estará disponível somente após selecionar um modelo de destino.
   >* Desmarcar **Selecionar tudo** desmarca todas as opções.

   Desmarque entre as opções a seguir para não transferir as informações para a tarefa de modelo movida. A tabela a seguir descreve o que acontece quando as opções são desmarcadas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Selecionar tudo</td> 
      <td>Desmarque essa opção para remover todas as informações da tarefa de modelo ao movê-la para seu novo local. </td> 
     </tr>
     <tr> 
      <td role="rowheader">Dt Restr</td> 
      <td> <p>A restrição da tarefa de modelo é definida como O Mais Breve Possível ou O Mais Tarde Possível com base na configuração do Modo de Agendamento do modelo.</p> <p> Quando selecionada, a restrição atual da tarefa de modelo é transferida para a tarefa de modelo movida. </p>

   <p><b>Nota</b>

   Ao mover uma tarefa de modelo com restrições específicas de data para outro modelo e as datas de restrição da tarefa de modelo estiverem fora das datas do novo modelo, a Restrição da tarefa de modelo será alterada para O Mais Breve Possível ou O Mais Tarde Possível ou as datas de Início Planejado ou de Conclusão Planejada dos modelos serão ajustadas.

   Veja a seguir exemplos de restrições específicas de data:
   <ul>
      <li> Início em</li>
      <li> Precisa Terminar Em</li>
      <li> Não Iniciar Antes De</li>
      <li> Não Iniciar Depois De</li>
      </ul>


   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Atribuições</td> 
      <td> <p>Todas as atribuições são removidas da tarefa de modelo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Processo de aprovação</td> 
      <td>Todos os processos de aprovação são removidos da tarefa de modelo.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Todos os predecessores</td> 
      <td> <p>Isso significa que as dependências não continuarão com as tarefas de modelo movidas. </p> <p>Quando selecionada, as predecessoras dentro do grupo de tarefas de modelo movidas são preservadas, outras são excluídas.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Dados personalizados</td> 
      <td> <p>Os valores dos campos personalizados são apagados e os formulários personalizados são transferidos com a tarefa de modelo movida. </p> <p>Quando selecionados, os formulários e os valores dos campos personalizados são transferidos com a tarefa de modelo movida. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Informações financeiras</td> 
      <td>As informações financeiras da tarefa de modelo movida são removidas e o Workfront atualiza o Tipo de Custo da tarefa de modelo para Sem Custo e o Tipo de Receita da tarefa de modelo como Não Faturável.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td> <p>Os documentos anexados à tarefa de modelo não são transferidos com a tarefa de modelo movida. Isso inclui versões, provas e documentos vinculados.</p>

   <p><b>Nota</b></p>

   <ul><li>
      <p>Isso não inclui aprovações de documentos. Aprovações de documentos nunca podem ser movidas quando uma tarefa de modelo é movida.</p> </li>
      <li>Se você optar por não mover os documentos com a tarefa de modelo, os documentos serão excluídos e colocados na Lixeira por 30 dias. Um administrador pode restaurá-los e eles serão restaurados na tarefa de modelo movida.

   Se a tarefa de modelo for excluída depois de movida, os documentos restaurados serão colocados na área Documentos da página do usuário do administrador que os restaura. </li> </ul>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificações de Lembrete</td> 
      <td>Os lembretes de tarefas de modelo não são transferidos para a tarefa de modelo movida. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Despesas</td> 
      <td>As despesas registradas na tarefa de modelo não são transferidas com a tarefa de modelo movida. </td> 
     </tr>  
    </tbody> 
   </table>


1. (Opcional) Clique em **Selecionar pai** no painel esquerdo e selecione a tarefa de modelo no modelo de destino que você deseja que se torne a principal da tarefa de modelo movida.

   >[!TIP]
   >
   >Ao selecionar para mover várias tarefas de modelo em uma lista, todas as tarefas de modelo selecionadas se tornam as tarefas filhas da tarefa pai selecionada e são adicionadas após as tarefas filhas existentes.

   Selecione um pai seguindo um destes procedimentos:

   * Na lista de tarefas de modelo, selecione um dos pais no plano de modelo.
   * Clique no ícone de pesquisa ![Ícone de pesquisa](assets/search-icon.png) e procure uma tarefa de modelo pai por nome.

   A tarefa de modelo deve aparecer na lista.

1. Selecione o botão de opção do pai depois de encontrá-lo.

   Se você não selecionar uma tarefa de modelo pai, as tarefas de modelo serão movidas como tarefas de modelo principais em vez de subtarefas e serão colocadas no final da lista de tarefas de modelo no modelo de destino.

1. Clique em **Mover Tarefa de Modelo**.

   As tarefas de modelo movidas agora estão no modelo especificado e são subtarefas da tarefa de modelo pai selecionada ou as últimas tarefas de modelo no modelo.
