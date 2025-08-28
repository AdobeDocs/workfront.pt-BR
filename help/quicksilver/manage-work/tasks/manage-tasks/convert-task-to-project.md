---
product-area: projects
navigation-topic: manage-tasks
title: Converter uma tarefa em um projeto
description: Quando uma tarefa em um projeto requer uma quantidade maior de esforço para ser concluída do que o planejado originalmente, é possível convertê-la em um projeto.
author: Alina
feature: Work Management
exl-id: a45f0af4-1768-4f20-80d4-912e6fe0fc03
source-git-commit: 7f719c903ad4079470a6dbd046dce445ba227a5b
workflow-type: tm+mt
source-wordcount: '1244'
ht-degree: 2%

---

# Converter uma tarefa em um projeto

<div class="preview">

As informações destacadas nesta página se referem a funcionalidades ainda não disponíveis no geral. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Os mesmos recursos também estarão disponíveis no ambiente de Produção para todos os clientes após uma semana da versão de Pré-visualização.

Para obter mais informações, consulte [Modernização da interface](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>

Quando uma tarefa em um projeto requer uma quantidade maior de esforço para ser concluída do que o planejado originalmente, é possível convertê-la em um projeto.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

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
   <td> <p>Editar acesso a tarefas e projetos</p> <p>Acesso de visualização ou superior aos Modelos ao converter em um projeto usando um modelo</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para uma tarefa</p> <p>Exibir permissões em um modelo, se estiver convertendo em um projeto usando um modelo</p> <p>Depois de criar o projeto, você tem Gerenciar permissões do projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações para converter tarefas em projetos

* Você pode converter uma tarefa em um projeto em branco ou em um projeto usando um modelo.
* A tarefa original é excluída.
* Todas as subtarefas, problemas e notas são acumulados no novo projeto.
* Documentos, versões de documentos e provas são movidos para o novo projeto.
* Há um limite de processamento de 5 minutos ao converter uma tarefa em um projeto. Se a tarefa tiver um grande número de documentos anexados a ela e não for convertida, talvez seja necessário remover alguns dos documentos e tentar novamente.
* O status e o percentual concluído de todas as subtarefas e problemas são preservados.
* Os atribuídos à tarefa e o usuário que converte a tarefa no projeto se tornam usuários compartilhados no projeto.
* A data de início do projeto é definida como a data de início da tarefa.
* A tabela a seguir lista informações do projeto e se ele é transferido do modelo ou da tarefa:

  <table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td>Descrição</td> 
    <td> <p>A Descrição da tarefa é transferida para o novo projeto. </p> <p> Se não houver descrição na tarefa, a Descrição do modelo será transferida para o projeto. </p> <p>Se o campo Descrição estiver vazio para a tarefa e para o modelo, o campo estará vazio no projeto. </p> </td> 
    </tr> 
    <tr> 
    <td>Status</td> 
    <td> Status padrão selecionado para o grupo no modelo. Se o modelo não estiver associado ao grupo, o status do projeto será definido como o status padrão definido pelo administrador do Workfront na área Preferências do projeto da Configuração. Para obter informações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md">Configurar preferências de projeto do sistema</a>

  Existem os seguintes cenários para atualizar o Status do projeto:
  <ul>
    <li> Se o status da tarefa for 'Novo', o status do projeto será definido como 'Planejamento'.</li>
    <li> Se o status da tarefa for 'Em andamento', o status do projeto será definido como 'Atual'.</li>
    <li> Se o status da tarefa for 'Concluída' o status do projeto será definido como 'Concluída'.</li></ul>

  </td> 
    </tr> 
    <tr> 
    <td>Prioridade</td> 
    <td>Transferências da tarefa para o projeto ou transferências do modelo, se você usar uma na conversão. </td> 
    </tr> 
    <tr> 
    <td>URL</td> 
    <td> <p>O URL da tarefa é transferido para o novo projeto. </p> <p> Se não houver um URL especificado na tarefa, o URL do modelo será transferido para o projeto. </p> <p>Se o campo URL estiver vazio para o problema e para o modelo, o campo estará vazio no projeto. </p> </td> 
    </tr> 
    <tr> 
    <td>Tipo de Condição do Projeto</td> 
    <td>Transferências do modelo.</td> 
    </tr> 
    <tr> 
    <td>Condição do projeto</td> 
    <td>Corresponde à preferência padrão em nível de sistema, conforme determinado pelo administrador do Workfront na área Configuração. Para obter informações, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md">Definir uma condição personalizada como padrão para projetos</a>
    </td> 
    </tr> 
    <tr> 
    <td>Cronograma de</td> 
    <td>Transferências do modelo.</td> 
    </tr> 
    <tr> 
    <td>Datas do projeto</td> 
    <td> 
      <ul> 
      <li> <p><b>Data de Início Planejada</b>: o horário de trabalho mais próximo baseado no horário de trabalho do agendamento do modelo deve ser pré-selecionado, de acordo com o fuso horário do agendamento do modelo. Este campo ficará desativado se o campo Agendar de estiver definido como Conclusão de. </p> </li> 
      <li> <p><b>Data de conclusão planejada</b>: o horário de trabalho mais próximo baseado no horário de trabalho do agendamento do modelo deve ser pré-selecionado, de acordo com o fuso horário do agendamento do modelo. Este campo estará desativado se o campo Agendar de estiver definido como Do início. </p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td>Portfólio</td> 
    <td>Transferências do modelo. Caso contrário, esse campo estará vazio.</td> 
    </tr> 
    <tr> 
    <td>Programa</td> 
    <td>Transferências do modelo. Caso contrário, esse campo estará vazio.</td> 
    </tr> 
    <tr> 
    <td>Grupo</td> 
    <td><p> Existem os seguintes cenários:</p>
      <ul><li>Se um grupo for especificado durante a conversão, ele será o grupo do projeto</li>
      <li>Se você converter em um projeto usando um modelo e houver um grupo no modelo e, durante a conversão, não especificar um grupo, o grupo do modelo se tornará o grupo do novo projeto</li>
      <li> Se não houver um grupo no modelo e você não especificar um grupo durante a conversão, o grupo do projeto original do problema se tornará o grupo do novo projeto</li> </ul>
        </td> 
    </tr> 
    <tr> 
    <td>Empresa</td>    
    <td>  Transferências do modelo. Caso contrário, esse campo estará vazio.</td>

  </tr> 
    <tr> 
    <td>Proprietário do projeto</td> 
    <td>Transferências do campo Proprietário do modelo no modelo. Caso contrário, será definido como o usuário conectado que está executando a conversão. </td> 
    </tr> 
    <tr> 
    <td>Patrocinador do Projeto</td> 
    <td>Transferências do campo Patrocinador do modelo no modelo. Caso contrário, esse campo estará vazio.</td> 
    </tr> 
    <tr> 
    <td>Gerenciador de Recursos</td> 
    <td>Transferências do modelo. Caso contrário, esse campo estará vazio.</td> 
    </tr> 
    <tr> 
    <td>Configurações da tarefa</td> 
    <td>Transferir a partir do modelo.</td> 
    </tr> 
    <tr> 
    <td>Configurações do problema</td> 
    <td>Transferir a partir do modelo. </td> 
    </tr> 
    <tr> 
    <td>Acesso</td> 
    <td> <p>Transferências da seção Acesso no modelo. </p> </td> 
    </tr> 
    <tr> 
    <td>Aprovações</td> 
    <td>Transferir a partir do modelo. As aprovações associadas à tarefa são removidas durante a conversão. </td> 
    </tr> 
  </tbody> 
  </table>


## Converter uma tarefa em um projeto

1. Vá para a tarefa que deseja converter em um projeto.
1. Clique no ícone **Mais** ![](assets/more-icon.png) e em **Converter para Projeto**.
1. Escolha uma das opções a seguir:

   * **Novo projeto**, para criar um projeto sem usar um modelo
   * Um modelo na seção **Selecionar nos Modelos**

     ![](assets/convert-task-to-project-template-option-dropdown-nwe-350x209.png)

1. Clique em **Continuar** na notificação exibida.
1. Na caixa **Converter em Projeto**, especifique o seguinte:

   * **Nome**: nomeie seu projeto. O nome padrão é o nome da tarefa. Este campo é obrigatório.
   * **Descrição**: descreva a finalidade deste projeto.
   * (Condicional) Se você optou por criar um projeto a partir de um modelo, atualize os campos disponíveis na caixa **Converter em projeto**.

     Para obter mais informações sobre a edição de campos em projetos, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

     >[!TIP]
     >
     >Para atualizar os campos na seção Finanças da caixa Converter em Projeto, você deverá ter o acesso para Editar aos Dados Financeiros no seu nível de acesso. Se você tiver o acesso de Visualização de Dados Financeiros no seu nível de acesso, todas as informações financeiras do modelo serão transferidas para o novo projeto e você não poderá editá-las enquanto converter o problema. Para obter informações, consulte [Conceder acesso aos dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) e [Compartilhar um modelo](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * (Opcional) Adicione o **Forms personalizado** ao novo projeto.

     >[!TIP]
     >
     >Se um formulário personalizado de vários objetos anexado à tarefa for configurado para uso com tarefas e projetos, todas as informações salvas no formulário serão retidas quando você fizer a conversão.
     >
     >
     >Se você estiver usando um modelo para a conversão e um formulário personalizado anexado ao modelo contiver um campo personalizado também encontrado em um formulário personalizado anexado à tarefa, o valor do campo da tarefa será usado para o novo projeto. No entanto, se o campo personalizado estiver vazio na tarefa, o valor do modelo será usado.

1. Clique em **Salvar alterações** <span class="preview">ou **Converter em projeto**.</span>
