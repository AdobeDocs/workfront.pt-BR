---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Listar objetos com um processo de aprovação pendente usando um determinado status
description: Se você tentar excluir um status, uma mensagem de erro poderá informar que ele não pode ser excluído porque está sendo usado em processos de aprovação pendentes em objetos do sistema. Se você quiser localizar e revisar esses objetos para decidir o que precisa fazer, poderá executar um relatório que os liste.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 52dd8750-9a6f-4ac6-9779-ba4ea9b6f4e0
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Listar objetos com um processo de aprovação pendente usando um determinado status

Se você tentar excluir um status, uma mensagem de erro poderá informar que ele não pode ser excluído porque está em pelo menos um processo de aprovação pendente no sistema. Você pode executar um relatório para listar os objetos onde ele está em um processo de aprovação pendente e, em seguida, decidir o que precisa ser feito para cada um deles.

## No modo Padrão

1. Vá para a área **Relatórios** na Barra de Navegação Global e selecione a guia **Relatórios**.
1. Clique no ícone Menu Principal ![](assets/main-menu-icon.png) no canto superior direito e em **Relatórios**.
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

1. Clique no ícone Menu Principal ![](assets/main-menu-icon.png) no canto superior direito e em **Relatórios**.
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
