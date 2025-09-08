---
title: Preencher automaticamente uma solicitação usando prompts ou documentos
content-type: reference
description: Você pode usar a IA para preencher automaticamente os campos de solicitação inserindo um prompt ou fornecendo um documento.
author: Becky
feature: Get Started with Workfront
exl-id: 4a22f9ea-c9ee-4947-8683-9989c54903b1
source-git-commit: b8c29ecb30dda449bc604f585a06b5a6663994f9
workflow-type: tm+mt
source-wordcount: '1144'
ht-degree: 2%

---

# Preencher automaticamente uma solicitação usando prompts ou documentos

>[!NOTE]
>
>* Essa funcionalidade estará disponível como um beta aberto no seguinte agendamento:
>
>   * Lançamento mensal: 11 de setembro de 2025
>   * Versão trimestral: 16 de outubro de 2025
>
>* Para usar essa funcionalidade, sua organização deve atender aos requisitos para usar o Assistente de IA da Workfront. Para obter detalhes, consulte [Pré-requisitos do Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

A IA pode ajudar a preencher automaticamente os campos de solicitação com base em um prompt inserido. Ele também pode preencher campos com base em texto, como emails que são documentos carregados. Você pode aprovar ou rejeitar essas sugestões antes de enviar a solicitação.

O preenchimento automático não substitui nenhum campo já preenchido.

Os usuários não recebem sugestões de dados aos quais, de outra forma, não teriam acesso.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Novo: Colaborador ou superior</p>
   Ou
   <p>Atual: solicitação ou superior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a ocorrências</p>  </td> 
  </tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td><p>Acesso para adicionar solicitações a uma fila de solicitações</p> <p>Exibir permissões ou mais altas na solicitação existente</p> <p>Para obter informações sobre como configurar uma fila de solicitações, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Criar uma fila de solicitações</a>. </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Para preencher automaticamente solicitações usando um prompt ou documento, **todos** dos itens a seguir devem ser aplicados:

* Sua organização deve ter migrado para o Adobe IMS (Identity Management System)
* A Experiência unificada do Adobe deve ser habilitada
* Sua organização deve ter um plano Select, Prime ou Ultimate Workfront
* A Adobe deve ter um contrato de geração de IA da Adobe assinado no arquivo

  Para obter mais informações sobre como assinar o contrato, consulte [Assinar o contrato de IA de geração da Adobe](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) no artigo Visão geral do Assistente de IA.
* O Assistente de IA deve estar ativado nas configurações do sistema de sua organização. Ele é gerenciado pelo administrador do Workfront.

  Para obter mais informações sobre como habilitar o Assistente de IA nas configurações do sistema, consulte [Habilitar ou desabilitar o Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

## Obter sugestões de um prompt de texto

O preenchimento automático pode sugerir valores de campo com base em texto, como emails. Você cola um bloco de texto e o Workfront processa o texto para sugerir valores de campo com base no texto.

Por exemplo, se o email incluir &quot;Isso vence em 1º de junho&quot; e o formulário de solicitação tiver um campo para data de vencimento, a Workfront sugerirá 1º de junho para esse valor de campo.

Esse tipo de sugestão também verifica solicitações anteriores para contextos semelhantes. Por exemplo, se o prompt mencionar que a solicitação é para um determinado cliente, o Workfront poderá localizar e inserir o endereço de faturamento desse cliente automaticamente, com base em solicitações anteriores.

Você pode colar no texto a ser aplicado a todo o formulário ou a uma única seção do formulário.

Para usar sugestões com base em um prompt de texto colado:

1. Comece a criar uma solicitação.

   Para obter instruções, consulte [Criar e enviar solicitações](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Para aplicar o prompt de texto a todo o formulário, clique no ícone de IA ![Ícone de IA](assets/request-prompt-icon.png) sob o nome do formulário.

   Ou

   Para aplicar o prompt de texto para uma única seção, clique no ícone de IA ![Ícone de IA](assets/request-prompt-icon.png) ao lado do nome da seção.

1. Cole o texto na caixa de prompt.
1. Clique em **Preencher o formulário**.

   O Workfront gera sugestões para o formulário.
1. Para cada sugestão de campo, selecione **Aceitar** ou **Rejeitar** para esse campo.

   ![Aceitar ou rejeitar sugestão](assets/accept-reject-suggestion.png)

   Ou

   Selecione **Aceitar tudo** ou **Rejeitar tudo** na parte superior da página para aceitar ou rejeitar todas as sugestões.

   >[!NOTE]
   >
   >Quaisquer sugestões não revisadas serão automaticamente aceitas quando você enviar a solicitação.

### Exemplos de prompt de texto

Esses exemplos mostram solicitações para várias maneiras de a IA fazer referência a outros projetos.

* Fazendo referência a uma campanha de cliente anterior

  ```
  Create a similar campaign request as we did for (Client Company)'s Q2 launch, but this time for their Automotive division. Keep the same deliverable set and audience profile.
  ```

* Com base em um projeto existente

  ```
  Use the same setup we had in the (Client Company) project kickoff last spring. I want to run a digital ad campaign targeting the same executive audience, but with updated dates for this quarter.
  ```

* Reutilizar um estilo de um produto anterior

  ```
  Prepare a request similar to the (Client Company) summer promotion campaign we ran last year. Focus on social media assets, keep Spanish as the primary language, and adjust the budget to $75,000.
  ```

* Expandir um tipo de campanha mais antigo

  ```
  Take the (Client Company) webinar series campaign from Q1 as a reference. I want the same registration workflow and assets, but this time the topic is 'AI in Financial Planning' and the audience is young professionals.
  ```

* Repetição de uma solicitação para um produto diferente

  ```
  Set up a campaign request just like the (Client Company) rebranding project we handled, but replace with (New Client Company) as the client. Keep all deliverables aligned to corporate branding.
  ```

* Estilo narrativo com referências implícitas

  ```
  We're planning a campaign similar to the holiday social ads we ran last year. Budget should be about 50k, goal is lead generation, and deliverables should include Instagram and TikTok assets.
  ```

## Obter sugestões com base em um documento do qual você fez upload

O preenchimento automático pode sugerir valores de campo com base em um documento que você fez upload.

Esse tipo de sugestão também verifica solicitações anteriores para contextos semelhantes. Por exemplo, se o prompt mencionar que a solicitação é para um determinado cliente, o Workfront poderá localizar e inserir o endereço de faturamento desse cliente automaticamente, com base em solicitações anteriores.

### Proteções de upload de documento

#### Tipos de arquivo compatíveis

Os seguintes tipos de arquivos são compatíveis:

<table>
<tr style="border: 0;">
<td>
<ul>
<li>BMP</li>
<li>CSV</li>
<li>DOC</li>
<li>DOCX</li>
<li>GIF</li>
<li>JPEG</li>
</ul>
</td>
<td>
<ul>
<li>ODP</li>
<li>ODS</li>
<li>ODT</li>
<li>PDF</li>
<li>Imagem PNG</li>
<li>PPT</li>
</ul>
</td>
<td>
<ul>
<li>PPTX</li>
<li>RTF</li>
<li>TIFF</li>
<li>TXT</li>
<li>XLS</li>
<li>XLSX</li>
</ul>
</td>
</tr>
</table>

#### Tamanho de arquivo suportado

Cada arquivo pode ter até 100 MB

#### Número de arquivos

É possível carregar até 50 arquivos (páginas, slides ou folhas).

>[!IMPORTANT]
>
>Os documentos são convertidos em uma série de imagens, cada uma considerada um arquivo separado.
>
>Por exemplo, você pode carregar um PowerPoint com 50 slides ou 5 documentos do Word com 10 páginas cada.

#### Tipos de campo compatíveis

Os tipos de campo do Workfront afetam se um determinado campo pode ser preenchido automaticamente.

<table>
<tr>
<td><b>O preenchimento automático </b><br> suportado pode ser preenchido</td>
<td><b>Sem suporte</b> <br>O preenchimento automático não preenche</td>
</tr>
<tr>
<td>
<ul>
<li>Texto de linha única</li>
<li>Área de texto ou parágrafo</li>
<li>Campo de data</li>
<li>Caixa de seleção</li>
<li>Botões de opção</li>
<li>menus suspensos Seleção única e múltipla</li>
</ul>
</td>
<td><li>Typeahead</li>
<li>Pesquisa externa</li>
<li>Pesquisa interna</li>
<li>Referência</li>
<li>Campos incorporados do WF Planning</li>
</ul>
</td>
</tr>
</table>

#### Outras práticas recomendadas

Considere o seguinte ao fazer upload de um documento para preenchimento automático da solicitação:

* O preenchimento automático está otimizado para o alfabeto latino.
* Recomendamos usar um tamanho de texto de 8 pontos ou maior.
* O preenchimento automático pode ter dificuldade com imagens no documento, como imagens giradas ou distorcidas, gráficos e contagem ou uso de motivos espaciais em objetos em imagens.
* Como sempre, recomendamos verificar a precisão dos resultados antes de enviar a solicitação.

### Carregar um documento para preencher uma solicitação automaticamente

Você pode carregar um documento para ser aplicado a todo o formulário ou a uma única seção do formulário.

1. Comece a criar uma solicitação.

   Para obter instruções, consulte [Criar e enviar solicitações](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Para aplicar o documento ao formulário inteiro, clique no ícone de IA ![Ícone de IA](assets/request-prompt-icon.png) sob o nome do formulário.

   Ou

   Para aplicar o documento a uma única seção, clique no ícone de IA ![Ícone de IA](assets/request-prompt-icon.png) ao lado do nome da seção.

1. Clique em **Carregar arquivos** e selecione o arquivo no gerenciador de arquivos.

   Ou

   Arraste o documento do gerenciador de arquivos para a caixa **Carregar arquivos para preencher automaticamente o formulário de solicitação**.
1. Clique em **Preencher o formulário** de **Preencher a seção**.

   O Workfront gera sugestões para o formulário.
1. Para cada sugestão de campo, selecione **Aceitar** ou **Rejeitar** para esse campo.

   ![Aceitar ou rejeitar sugestão](assets/accept-reject-suggestion.png)

   Ou

   Selecione **Aceitar tudo** ou **Rejeitar tudo** na parte superior da página para aceitar ou rejeitar todas as sugestões.

   >[!NOTE]
   >
   >Quaisquer sugestões não revisadas serão automaticamente aceitas quando você enviar a solicitação.

## Solução de problemas

Se você não estiver recebendo as sugestões esperadas, talvez seja devido a um dos seguintes motivos:

* Você deve ter pelo menos um mês de dados de solicitação no sistema para que ele possa sugerir valores de campo de solicitações anteriores.
* Talvez você não tenha seguido as medidas de proteção de carregamento de documento ao carregar um documento do qual extrair sugestões. Para obter mais informações, consulte [Medidas de proteção para o carregamento de documentos](#document-upload-guardrails) neste artigo.
