---
title: Visão geral da Integridade do Projeto
content-type: reference
description: O recurso Integridade do projeto utiliza o poder do Assistente de IA para fornecer instantaneamente uma avaliação do desempenho de seus projetos.
author: Jenny
feature: Get Started with Workfront
exl-id: e4d200c6-7f35-4919-96d3-2880a655ed62
source-git-commit: 2024f19709f7859ed6f19b830321d9e4c09e71f8
workflow-type: tm+mt
source-wordcount: '1822'
ht-degree: 0%

---

# Visão geral da Integridade do Projeto

>[!IMPORTANT]
>
>No momento, o recurso Integridade do projeto está disponível apenas para usuários que participam da fase beta.

O recurso Saúde do projeto do Adobe Workfront utiliza o poder do Assistente de IA para fornecer instantaneamente uma avaliação do desempenho de seus projetos, quais áreas precisam de sua atenção e como evitar problemas que podem custar tempo e dinheiro.

O Assistente de IA pode gerar uma avaliação de Integridade do projeto para os seguintes objetos:

* Um único projeto
* Um único programa
* Vários projetos

Para obter mais informações sobre o Assistente de IA, consulte [Visão geral do Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

+++ Expanda para visualizar os requisitos de acesso. 
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>plano do Adobe Workfront</p></td> 
   <td> 
<p>Select, Prime ou Ultimate </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td> 
<p>Standard</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurações de nível de acesso</p></td> 
   <td><p>Administrador para gerenciar configurações de Integridade do Projeto </p>
   <p>Editar para aplicar configurações de Integridade do Projeto </p>
     <p>Exibir para exibir as configurações de Integridade do Projeto </p>
  </td> 
  </tr>  
    </tr>  
</tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Inscrever-se no beta de Integridade do projeto

Para utilizar o Project Health, sua organização deve ter o Assistente de IA ativado.

Para habilitar o Assistente de IA para sua organização, todos os itens a seguir devem se aplicar:

* Sua organização deve ter migrado para o Adobe IMS (Identity Management System).
* A Experiência unificada do Adobe deve ser habilitada.
* A Adobe deve ter um contrato de API Gen da Adobe assinado no arquivo.
* O administrador do Workfront deve ativar o Assistente de IA para os usuários em sua organização. O Assistente de IA é ativado por meio de níveis de acesso.

Para obter mais informações, consulte [Visão geral do Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

## Lista de prompts do assistente do AI

Abaixo está uma lista de prompts que você pode usar para solicitar a Avaliação da IA a fim de gerar uma Avaliação da Integridade do Projeto para um projeto, programa ou todos os projetos em sua conta.

<table>
    <tr>
        <td><b>Localização</b></td>
        <td><b>Prompt</b></td>
    </tr>
    <tr>
        <td>Uma página de detalhes do projeto específica</td>
        <td><em>Qual é o estado deste projeto?</em></td>
    </tr>
    <tr>
        <td>Qualquer página no Workfront </td>
        <td><em>Qual é a integridade do projeto [NOME DO PROJETO]?</em></td>
    </tr>
    <tr>
        <td>Qualquer página no Workfront </td>
        <td><em>Qual é o estado dos meus projetos?</em></td>
    </tr>
       <tr>
        <td>Uma página de detalhes do programa específico</td>
        <td><em>Qual é o estado deste programa?</em></td>
    </tr>
       <tr>
        <td>Qualquer página no Workfront </td>
        <td><em>Qual é a integridade do programa [NOME DO PROGRAMA]?</em></td>
    </tr>
   </table>


## Lista de condições de projeto e programa

Abaixo estão as condições disponíveis que o Assistente de IA atribuirá ao seu projeto ou programa ao gerar uma avaliação de Integridade do projeto.

<table>
    <tr>
        <td><b>Condição do projeto</b></td>
        <td><b>Status de Progresso do Projeto</b></td>
    </tr>
    <tr>
        <td>No Prazo</td>
        <td>Quando o status de progresso do projeto é No prazo, a condição do projeto é No destino.</td>
    </tr>
    <tr>
        <td>Em Risco</td>
        <td>Quando o status de progresso do projeto está atrasada ou está em risco, a condição do projeto é Em risco.</td>
    </tr>
    <tr>
        <td>Com problemas</td>
        <td>Quando o Status de Progresso do projeto é Atrasado, a condição do projeto é Em Risco.</td>
    </tr>
    </tr>
   </table>

## Gerenciar configurações de Integridade do Projeto

Uma configuração de integridade do projeto contém critérios específicos que determinam como a integridade do projeto é calculada. Depois que uma configuração é criada, você pode aplicá-la a um projeto.

>[!NOTE]
>
>Você precisa ser um Administrador do Sistema para gerenciar as configurações de Integridade do Projeto.

{{step-1-to-setup}}

1. Clique em **Preferências do projeto** no painel esquerdo e selecione **Integridade do projeto** no menu suspenso exibido.

1. No canto superior direito da página, selecione **Nova configuração**.

1. (Opcional) Na página de detalhes das configurações, substitua *Configuração sem título* por uma nova configuração **Nome**.

1. Na seção **Que fatores você deseja incluir na integridade do projeto**, desmarque qualquer fator que não queira incluir ao determinar os critérios de integridade do projeto:
   * **Trilha de escopo**: quanto o escopo do projeto foi expandido desde seu início.

   * **Campos obrigatórios**: se algum campo obrigatório estiver ausente (por exemplo, descrição do projeto). Estes campos obrigatórios determinam a integridade do projeto e são especificados em **Quais campos você deseja verificar?** seção de configuração abaixo.


   * **Alterações de agendamento**: quantas alterações de agendamento ocorreram desde que o projeto foi iniciado.

   * **Estimativa da tarefa**: a precisão com que o trabalho da tarefa foi estimado (por exemplo, nenhuma tarefa vencida atualmente no projeto).

   * **Burndown de tarefas**: a comparação entre o andamento do trabalho do projeto e a linha do tempo do projeto.

   * **Tarefas vencidas**: quantas tarefas estão atrasadas na data de vencimento.

   * **Custo**: se o projeto estiver acima do orçamento.

1. No **Quando o projeto é iniciado oficialmente?**, selecione o evento que sinaliza o início do seu projeto no menu suspenso.

1. No **Como você estima o escopo do trabalho em um projeto?Seção**, selecione qual fator de projeto aumentará à medida que o escopo do projeto aumentar.

1. Na **Em quais campos você deseja verificar a integridade?**, selecione um ou mais campos que serão verificados para determinar a integridade do projeto.

   ![Campos de conclusão do projeto](assets/project-completeness-fields.png)


1. Clique em **Salvar** no canto superior direito.

## Aplicar configurações de Integridade do Projeto

Depois que um administrador cria uma configuração de Integridade do projeto, os usuários com acesso de Edição podem aplicá-la a um projeto.


{{step1-to-projects}}

1. Na página **Projetos**, selecione um projeto.

1. Clique no ícone **Mais** ![Mais ícone](assets/more-icon.png) à direita do nome do projeto e selecione **Editar**. O painel lateral **Editar projeto** é aberto.

1. No painel esquerdo, selecione **Configurações do projeto**.

1. No campo **Configuração de Integridade do Projeto**, selecione a configuração que deseja aplicar a este projeto.

   ![Campo de configuração de Integridade do Projeto](assets/project-health-configurations.png)

1. Clique em **Salvar** no canto inferior esquerdo do painel.

## Gerar uma avaliação de Integridade do Projeto para um projeto ou programa

Se você tiver acesso de Visualização para um projeto ou programa, poderá gerar a avaliação de Integridade do projeto usando o assistente de IA.

Se estiver gerando uma avaliação para um projeto, isso pode ser feito a partir da página do projeto ou referenciando o nome do projeto quando você perguntar ao assistente como o projeto está se saindo.

Se estiver gerando uma avaliação para um programa, você pode fazê-lo na página de detalhes do programa.

>[!NOTE]
>
>Uma avaliação de Integridade do Projeto não pode ser gerada para um projeto até que ele tenha sido iniciado. Você pode definir qual evento aciona um projeto para começar nas configurações do projeto.

Para obter mais informações, consulte a seguinte seção neste artigo: [Gerenciar configurações de integridade do projeto](#manage-project-health-configurations).

1. Navegue até o projeto ou programa para o qual você deseja gerar uma avaliação de Integridade do Projeto.

1. Na página de detalhes do projeto/programa, clique no **ícone do Assistente de IA** ![ícone do Assistente de IA](assets/ai-assistant-icon.png), no canto superior direito da tela. O Assistente de IA é aberto.

1. Digite o seguinte no campo **Pergunte-me sobre o Workfront**: *Qual é a integridade deste projeto?*

   Ou

   Digite o seguinte no campo **Pergunte-me sobre o Workfront**: *Qual é a integridade deste programa?*

   >[!NOTE]
   >
   >Se você estiver acessando o Assistente de IA de uma página diferente no Workfront, poderá digitar *Qual é a integridade do projeto [NOME DO PROJETO]?* ou *Qual é a integridade do programa [NOME DO PROGRAMA]?* <br>
   >Para obter uma lista completa dos prompts atuais que você pode inserir, consulte a seguinte seção neste artigo: [lista de prompts do Assistente de IA](#ai-assistant-prompts-list).

1. Clique no ícone **Enviar** ![Ícone Enviar](assets/send-icon.png). A avaliação de Integridade do projeto é gerada e exibida no painel. Uma medalha é exibida na parte superior de cada avaliação de Integridade do Projeto, o que reflete a condição atual do projeto.

   ![Avaliação de integridade do projeto](assets/health-assessment.png)

   Se estiver gerando uma avaliação para um portfólio, várias medalhas serão listadas mostrando a condição de cada projeto no programa. Para obter mais informações sobre os rótulos de medalha, consulte a seguinte seção neste artigo: [Lista de condições de projeto e programa](#project-and-program-conditions-list).

1. (Opcional) Clique em um dos pontos de avaliação para expandir seus detalhes.

1. (Opcional) No modo de detalhes expandido, clique no link da tarefa para abrir os detalhes da tarefa.

   ![Detalhes expandidos](assets/expanded-details.png)

1. Depois de examinar os detalhes de integridade do projeto, clique no ícone **Fechar** ![Ícone Fechar](assets/close-icon.png) no canto superior direito do Assistente de IA.

## Gerar uma avaliação de Integridade do Projeto para vários projetos

Você pode gerar uma avaliação combinada da Integridade do projeto para todos os projetos aos quais você tem acesso de Visualização (ou superior) no momento.

Um projeto só será incluído na avaliação combinada da Integridade do Projeto se o projeto tiver sido iniciado. Você pode definir qual evento aciona um projeto para começar nas configurações do projeto. Para obter mais informações, consulte a seguinte seção neste artigo: [Gerenciar configurações de integridade do projeto](#manage-project-health-configurations).

1. Clique no ícone do **Assistente de IA** ![ícone do Assistente de IA](assets/ai-assistant-icon.png), no canto superior direito da tela. O Assistente de IA é aberto.

1. Digite o seguinte no campo **Pergunte-me sobre o Workfront**: *Qual é a integridade dos meus projetos?*

   Para obter uma lista completa dos prompts atuais que você pode inserir, consulte a seguinte seção neste artigo: [lista de prompts do Assistente de IA](#ai-assistant-prompts-list).

1. Clique no ícone **Enviar** ![Ícone Enviar](assets/send-icon.png). A avaliação de Integridade do projeto é gerada e exibida no painel.

   ![Avaliação de vários projetos](assets/multiple-projects-assessment.png)

   Ao gerar uma avaliação para vários projetos, o Assistente de IA agrupa os resultados com base no desempenho atual dos projetos.

1. (Opcional) Clique em um dos emblemas de condição de integridade do projeto para expandir a lista de projetos e, em seguida, selecione um link para um projeto específico para ir para a página de detalhes desse projeto.

1. Depois de examinar os detalhes de integridade dos projetos, clique no ícone **Fechar** ![Ícone Fechar](assets/close-icon.png) no canto superior direito do Assistente do AI para fechá-lo.


## Criar um relatório de tabela de Integridade do projeto em um Painel da Tela

>[!IMPORTANT]
>
>No momento, o recurso Painéis do Canvas está disponível apenas para usuários que participam da fase beta. Para obter mais informações, consulte [informações beta de Painéis do Canvas](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md).

Você pode adicionar um relatório de tabela a um Painel da Tela para visualizar facilmente os dados de Integridade do Projeto em um formato de tabela.

### Pré-requisitos

Você deve criar um painel antes de criar um relatório de tabela.

Para obter mais informações, consulte [Criar um Painel da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

### Criar um relatório de tabela de Integridade do Projeto

Há muitas opções de configuração disponíveis para criar um relatório de tabela Integridade do projeto. Nesta seção, guiaremos você pelo processo de criação de uma que exibe as seguintes colunas:

* **Nome**: contém o nome do projeto.
* **Análise de Integridade do Projeto**: contém um resumo da avaliação de Integridade do Projeto.
* **Integridade do Projeto Criada às**: contém a data/hora em que a avaliação de Integridade do Projeto foi gerada pela última vez.
* **Rótulo de Integridade do Projeto**: contém o rótulo do projeto (por exemplo, No alvo, em risco ou com problemas).

{{step1-to-dashboards}}

1. No painel esquerdo, clique em **Painéis do Canvas**.
1. No canto superior direito, clique em **Novo Painel**.
1. Na caixa **Criar painel**, digite o **Nome** e a **Descrição** do painel.
1. Clique em **Criar**.
1. Na caixa **Adicionar relatório**, selecione **Criar relatório**.
1. No lado esquerdo, selecione **Tabela**.
1. No canto superior direito, clique em **Criar relatório**.
1. (Opcional) Siga as etapas abaixo para configurar a seção **Detalhes** ![Ícone de detalhes](assets/details-icon.png):
   1. Insira um relatório **Nome**.
   1. Insira uma **Descrição** do relatório.
1. Siga as etapas abaixo para configurar a seção **Criar tabela** ![Criar ícone de tabela](assets/drilldown-column.png):
   1. No painel esquerdo, clique no ícone **Colunas da tabela**.
   1. Clique em **Adicionar coluna** e selecione **Projeto** > **Nome**.
   1. Clique em **Adicionar coluna** e selecione **Projeto** > **Integridade do Projeto** > **Análise de Integridade**.
   1. Clique em **Adicionar coluna** e selecione **Projeto** > **Integridade do Projeto** > **Criado às**.
   1. Clique em **Adicionar coluna** e selecione **Projeto** > **Integridade do Projeto** > **Rótulo de Integridade**.

1. Siga as etapas abaixo para configurar a seção **Ícone de** Filtro![](assets/filter-icon.png):
   1. No painel esquerdo, clique no ícone **Filtro**.
   1. Selecione **Editar filtro**.
   1. Clique em **Adicionar condição** e especifique o campo pelo qual deseja filtrar e o modificador que define o tipo de condição que o campo deve atender. A coluna é exibida na seção de visualização à direita.
   1. (Opcional) Clique em **Adicionar grupo de filtros** para adicionar outro conjunto de critérios de filtragem. O operador padrão entre os conjuntos é AND. Clique no operador para alterá-lo para OU.

1. Siga as etapas abaixo para configurar a seção **Configurações do Grupo de Detalhamento** ![Configurações do grupo](assets/drilldown-group-icon.png):
   1. No painel esquerdo, clique no ícone **Configurações de grupo**.
   1. Clique no botão **Adicionar agrupamento** e selecione o campo que deseja criar como agrupamento. A coluna de agrupamento aparece na seção de visualização à direita.

1. Clique em **Salvar** para criar o relatório.
