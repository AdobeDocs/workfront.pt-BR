---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Listar objetos com processos de aprovação pendentes usando um determinado status
description: Se você tentar excluir um status, uma mensagem de erro talvez informe que ele não pode ser excluído porque está sendo usado em processos de aprovação pendente em objetos do sistema. Se quiser encontrar e revisar esses objetos para decidir o que precisa fazer, execute um relatório que os liste.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 52dd8750-9a6f-4ac6-9779-ba4ea9b6f4e0
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Listar objetos com processos de aprovação pendentes usando um determinado status

Se você tentar excluir um status, uma mensagem de erro talvez informe que ele não pode ser excluído, pois está em pelo menos um processo de aprovação pendente no sistema. Você pode executar um relatório para listar os objetos em que ele está em um processo de aprovação pendente e decidir o que precisa fazer para cada um.

## No modo Padrão

1. Vá para o **Relatório** na Barra de Navegação Global, em seguida, selecione o **Relatórios** guia .
1. Clique no ícone do Menu principal ![](assets/main-menu-icon.png) no canto superior direito, em seguida, clique em **Relatórios**.
1. Clique em **Novo relatório**, em seguida selecione **Relatório de projeto**, **Relatório de tarefa** ou **Relatório de problemas**.
1. Abra o **Filtros** guia .
1. Clique em **Adicionar uma regra de filtro** e faça o seguinte para configurar a regra:
   1. Comece a digitar `status`, em seguida selecione **Status** quando exibido.
   1. Sair **Igual** no segundo campo.
   1. Selecione o nome do status no terceiro campo .
1. Clique em **Adicionar uma regra de filtro** novamente, faça o seguinte para configurar a regra
   1. Comece a digitar `pending status`, em seguida, selecione esse item quando ele for exibido abaixo do tipo de objeto que você está procurando (**Projeto**, **Tarefa** ou **Problema**).
   1. Sair **Igual** no segundo campo.
   1. Tipo `in` no terceiro campo.
1. Clique em **Adicionar uma regra de filtro** novamente, faça o seguinte para configurar a regra
   1. Comece digitando o processo de aprovação e selecione **ID do grupo** quando exibido em **Processo de aprovação**.
   1. Selecionar **Está em Branco** no segundo campo.
1. Clique em **Salvar + Fechar** para executar o relatório e listar todos os objetos do tipo especificado com processos de aprovação em estado pendente com base no status especificado (**Projeto**, **Tarefa** ou **Problema**).
1. Repita essas etapas para encontrar as mesmas informações para os outros dois tipos de objeto.


## No modo de texto

1. Clique no ícone do Menu principal ![](assets/main-menu-icon.png) no canto superior direito, em seguida, clique em **Relatórios**.
1. Clique em **Novo relatório**, em seguida selecione **Relatório de projeto**, **Relatório de tarefa** ou **Relatório de problemas**.
1. Abra o **Filtros** guia .
1. Selecionar **Alternar para o modo de texto**.
1. Copie e cole o seguinte na janela de edição, substituindo XXX pela chave de 3 letras do status:

   `status=XXX`

   `status_Mod=in`

   `approvalProcess:groupID_Mod=isblank`

   Você pode exibir a chave na lista de status, conforme mostrado nestes artigos:
   * [Acessar a lista de status de projeto do sistema](project-statuses.md)
   * [Acessar a lista de status de tarefas do sistema](task-statuses.md)
   * [Acesse a lista de status de problemas do sistema](issue-statuses.md)

1. Clique em **Salvar + Fechar** para executar o relatório e listar todos os objetos do tipo especificado com processos de aprovação em estado pendente com base no status especificado (**Projeto**, **Tarefa** ou **Problema**).
1. Repita essas etapas para encontrar as mesmas informações para os outros dois tipos de objeto.
