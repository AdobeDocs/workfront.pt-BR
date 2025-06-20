---
navigation-topic: business-case-and-scorecards
title: Criar um Business Case para um projeto
description: Você pode usar o Business Case para solicitar um projeto e definir a finalidade, o orçamento e o benefício potencial para o projeto. O gerente do Portfolio ou o patrocinador do projeto usa as informações do Business Case para analisar e priorizar o projeto antes de aprová-lo.
author: Alina
feature: Work Management
exl-id: db69b3bf-04e3-49b4-ae0d-ab6145389db5
source-git-commit: f97c989f57d864252adf6e24f8e6b03f56d26901
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 0%

---

# Criar um Business Case para um projeto

<!--Audited: 6/2025-->

Você pode usar o Business Case para solicitar um projeto e definir a finalidade, o orçamento e o benefício potencial para o projeto. O gerente do Portfolio ou o patrocinador do projeto usa as informações do Business Case para analisar e priorizar o projeto antes de aprová-lo.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader"><p>plano do Adobe Workfront*</p></td> 
   <td> 
   <p>Atual: Prime ou superior</p> 
   <p>Herdados: Pro ou superior</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td> 
   <td> 
   <p>Atual: Padrão </p> 
   <p>Herdados: plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurações de nível de acesso</p></td> 
   <td> <p>Editar acesso ao Gerenciamento de Projetos, Dados Financeiros e Recursos</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td> <p>Gerenciar ou aumentar permissões no projeto</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Considere o seguinte ao solicitar um projeto por meio de um Business Case:

* O administrador do Adobe Workfront ou do grupo deve ativar as seções do Business Case antes que elas apareçam em seu projeto.\
  Para obter informações sobre como habilitar as seções no Business Case no nível do sistema, consulte o artigo [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  Para obter informações sobre as áreas do Business Case, consulte o artigo [Visão Geral das Áreas do Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* Você deve preencher todas as áreas do Business Case, exceto a área Metas, se quiser que o projeto receba uma Pontuação no Portfolio Otimizer. A conclusão da área Metas é opcional. O projeto recebe uma Pontuação no Portfolio Otimizer, mesmo se essa área não estiver concluída.

  Para obter informações sobre como trabalhar com Scorecards e com o Portfolio Otimizer, consulte o artigo [Aplicar um scorecard a um projeto e gerar uma Pontuação de Alinhamento](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

## Criar um Business Case

{{step1-to-projects}}

1. Clique em **Novo projeto** e selecione **Solicitar projeto** no menu suspenso exibido. O projeto é criado e o status **Ideia** é atribuído por padrão.

   >[!CAUTION]
   >
   >Se o status Ideia tiver sido excluído na instância do Workfront, o projeto será colocado no status padrão para novos projetos, conforme definido na área Preferências do projeto. Para obter informações sobre como configurar preferências de projeto, consulte [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. Insira um nome no campo de título do projeto.
1. (Opcional) Clique no ícone **Mais** ícone ![Mais](assets/qs-more-icon-on-an-object.png), em seguida **Anexar modelo** para criar a Estrutura de detalhamento de trabalho do seu projeto.

   Ou

   Comece a adicionar tarefas ao projeto manualmente.

1. (Condicional) Se você selecionou anexar um modelo, continue anexando o modelo ao projeto.
1. No painel esquerdo, clique em **Business Case**.
1. (Opcional) Para editar a seção **Informações do projeto**, clique em **Editar informações do projeto**. 

   Para obter mais informações sobre como editar os campos de seção **Informações do Projeto**, consulte a seção [Informações do Projeto](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) no artigo [Visão Geral das Áreas do Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Opcional) Para editar a seção **Metas**, clique em **Editar Metas**.

   Para obter mais informações sobre como editar a seção **Metas** do Business Case, consulte a seção [Metas](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#goals) no artigo [Visão Geral das Áreas do Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Opcional) Para editar a seção **Despesas**, clique em **Editar Despesas**.

   Para obter mais informações sobre como editar a seção **Despesas** do Business Case, consulte a seção [Despesas](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#expenses) no artigo [Visão Geral das Áreas do Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Opcional) Clique em **Editar orçamento de recursos** para fazer um orçamento de seus recursos e obter o Custo de mão de obra orçado associado às funções de trabalho no projeto. Para obter mais informações, consulte [Recursos de orçamento no Business Case](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

   >[!TIP]
   >
   >As informações exibidas aqui são as mesmas informações exibidas nas ferramentas de orçamento de recursos no nível do sistema.

1. (Opcional) Clique em **Editar riscos** para adicionar riscos em potencial a este projeto. Para obter informações sobre como adicionar riscos ao Business Case, consulte a seção [Riscos](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#risks) no artigo [Visão Geral das Áreas do Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).
1. (Opcional) Selecione um **Scorecard** no menu suspenso **Adicionar um Scorecard a este Projeto**.

   Scorecards devem ser criados antes de serem anexados a projetos.

   Para obter mais informações sobre cartões de pontuação, consulte o artigo [Aplicar um cartão de pontuação a um projeto e gerar uma Pontuação de Alinhamento](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

1. (Opcional) Selecione um **Formulário personalizado** no menu suspenso **Forms personalizado**.

   O Forms personalizado deve ser criado antes de ser anexado aos projetos.

   Para obter mais informações sobre o Forms Personalizado, consulte o artigo [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Clique em **Enviar**. O status do projeto foi alterado para **Solicitado** e enviado para que o Business Case seja aprovado.

   Para obter mais informações sobre a aprovação de um Business Case, consulte o artigo [Aprovar um Business Case](../../../manage-work/projects/define-a-business-case/approve-business-case.md).


>[!TIP]
>
> Após concluir o Business Case, você pode exportar uma cópia dele para um arquivo .pdf. Para obter mais informações sobre como exportar o Business Case para um arquivo .pdf, consulte [Exportar o Business Case de um projeto](/help/quicksilver/manage-work/projects/define-a-business-case/export-business-case.md).


