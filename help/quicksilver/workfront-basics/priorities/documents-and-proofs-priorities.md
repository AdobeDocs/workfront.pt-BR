---
navigation-topic: get-started-with-workfront
title: Fazer upload de documentos e criar provas em Prioridades
description: Documentos
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
exl-id: 63aa5e45-e51d-4049-a5d9-18dfaaa79647
source-git-commit: 985f1aa11ad1d5efc8d043907d60ad5f5c1bba13
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 2%

---

# Fazer upload de documentos e criar provas em Prioridades

Você pode fazer upload de documentos e criar provas em Prioridades.

Prioridades exibe os itens de trabalho atribuídos a você. Não é possível ver os itens de trabalho atribuídos à sua equipe.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> 
   <p>Qualquer</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Colaborador ou superior para carregar documentos; Padrão para criar provas</p>
   <p>Solicitação ou superior para carregar documentos; Trabalho ou superior para criar provas</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de Permissões de Prova </td> 
   <td>Gerente ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a documentos</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Carregar um documento em um item de trabalho

Você pode fazer upload de um documento para um item de trabalho na lista de trabalho ou na página Detalhes do item de trabalho.

### Painel de resumo da lista de trabalho


{{step1-to-priorities}}

1. Na lista de trabalho, passe o mouse sobre o nome do trabalho e clique no ícone **Resumo** ![abrir ícone de resumo](assets/summary-icon.png).
1. Verifique se você está na guia **Tarefa** ou **Problemas** no painel de resumo.
1. Clique no ícone **Carregar arquivo** ![ícone Carregar arquivo](assets/upload-file-icon.png).
1. Arraste e solte o arquivo ou pressione Cmd/Ctrl + V para colar da área de transferência
ou
Clique em **Adicionar arquivos** para procurar arquivos ou importar arquivos de um provedor Document Cloud.
   ![Adicionar arquivos](assets/add-files.png)
1. (Opcional) Adicione um comentário.
1. (Opcional) Adicione mais arquivos.

   >[!NOTE]
   >
   >Arquivos adicionais são carregados como documentos separados.
1. Clique em **Carregar**.

### Detalhes do item de trabalho

{{step1-to-priorities}}

1. Na lista de trabalho, clique no nome do item de trabalho.
1. Clique na guia **Documentos** na parte superior da tela.
1. Clique em **Carregar documento** no canto superior direito e selecione **Documento**.
1. Arraste e solte o arquivo ou pressione Cmd/Ctrl + V para colar da área de transferência
ou
Clique em **Adicionar arquivos** para procurar arquivos ou importar arquivos de um provedor Document Cloud.
   ![Adicionar arquivos](assets/add-files.png)
1. (Opcional) Adicione um comentário.
1. (Opcional) Adicione mais arquivos.

   >[!NOTE]
   >
   >Arquivos adicionais são carregados como documentos separados.
1. Clique em **Carregar**.


## Criar uma prova simples ou avançada

Você pode criar uma prova de um documento da lista de trabalho ou da página Detalhes do item de trabalho.

### Painel de resumo da lista de trabalho


{{step1-to-priorities}}

1. Na lista de trabalho, passe o mouse sobre o nome do trabalho e clique no ícone **Resumo** ![abrir ícone de resumo](assets/summary-icon.png).
1. Verifique se você está na guia **Tarefa** ou **Problemas** no painel de resumo.
1. Clique no ícone **Documentos** ![Ícone Documentos](assets/show-document-icon.png) no painel direito.
1. Clique no ícone **Carregar arquivo** ![Ícone Carregar arquivo](assets/upload-file-icon.png) e escolha o arquivo.

   >[!NOTE]
   >
   >Você deve carregar o documento antes de criar a prova.


1. Depois que o arquivo for carregado, selecione-o na seção **Documentos**.
1. Clique em **Criar prova** no canto superior direito da caixa Detalhes do arquivo.
1. Escolha uma das seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><b>Prova simples</b></td> 
      <td>Essa opção cria uma prova sem fluxo de trabalho anexado e aplica as configurações de prova padrão. Você pode atualizar as configurações de prova padrão ou adicionar um fluxo de trabalho depois de criar a prova. Para obter mais informações sobre configurações de prova, consulte <a href="/help/quicksilver/review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Editar configurações de prova</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><b>Prova avançada</b></td> 
      <td> <p>Essa opção permite configurar um fluxo de trabalho Básico ou Avançado e modificar configurações de prova para a prova criada. Para obter mais informações, consulte </p> 
       <ul> 
        <li><p><a href="/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Criar uma prova avançada com um fluxo de trabalho Básico</a> </p> </li> 
        <li> <p><a href="/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Criar uma prova avançada com um fluxo de trabalho automatizado</a></p></li> 
       </ul>
        </td> 
     </tr> 
    </tbody> 
   </table>

### Detalhes do item de trabalho

{{step1-to-priorities}}

1. Na lista de trabalho, clique no nome do item de trabalho.
1. Clique na guia **Documentos** na parte superior da tela.
1. Clique em **Carregar documento** no canto superior direito e selecione **Prova**.
1. Crie uma prova conforme descrito em
   [Criar uma prova avançada com um fluxo de trabalho Básico](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   [Criar uma prova avançada com um fluxo de trabalho automatizado](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

<!--

## Open a proof



## Edit a document

Edit name

Add description

manage

Add new version, open proof, edit, download, move, share, remove
-->

## Filtrar e classificar

Você pode organizar seu documento usando filtros e opções de classificação.

### Filtro

Você pode filtrar documentos por

* Adicionado por
* Tipo do arquivo

### Ordenar

Você pode classificar documentos por

* Data de adição
* Tipo do arquivo
