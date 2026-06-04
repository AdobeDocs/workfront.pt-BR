---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Criar uma prova para conteúdo interativo em um arquivo ZIP
description: Você pode gerar uma prova para conteúdo interativo que não seja de sites armazenado em um arquivo ZIP. Exemplos desse tipo de conteúdo da Web incluem anúncios com streaming de vídeo ou áudio, animações HTML e banners interativos.
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
TQID: https://experienceleague.adobe.com/wJNC4pCRhTpOfoiB1X6-6vKrYvWA2EaR-x2HfhwcDaY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 350
ht-degree: 24%

---

# Criar uma prova para conteúdo interativo em um arquivo ZIP

Você pode gerar uma prova para conteúdo interativo que não seja de sites armazenado em um arquivo ZIP. Exemplos desse tipo de conteúdo da Web incluem anúncios com streaming de vídeo ou áudio, animações HTML e banners interativos.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Padrão</p>
   <p>Trabalho ou Plano</p> 
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

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar uma prova para conteúdo interativo em um arquivo ZIP

Depois de adicionar o conteúdo interativo em um arquivo ZIP a uma prova, o Adobe Workfront cria uma prova dos documentos compactados. Dependendo do tamanho do arquivo, o tempo de carregamento do upload pode variar. Arquivos maiores demoram mais para serem criados. Você pode sair da página e o Workfront continua a criar seu arquivo. O tamanho máximo do upload de arquivo é 4 GB. 

1. Prepare seu conteúdo criando um arquivo ZIP incorporado.

   O arquivo ZIP deve atender aos seguintes requisitos:

   * Todos os ativos, como CSS, JavaScript, vídeos, sons e imagens devem ser incluídos no arquivo de pacote.
   * Verifique se o arquivo principal (como index.html, index.htm) está na pasta raiz e se é o único arquivo .html/.htm armazenado lá.

     Se o arquivo principal não for colocado na pasta raiz, o Workfront pesquisará a pasta para encontrar o arquivo principal.

   * O tamanho máximo do pacote é de 500 MB.
   * No caso de arquivos ZIP criados no iOS, a ferramenta identifica automaticamente a pasta correta onde o conteúdo é colocado.

1. Vá para o projeto, tarefa ou problema em que deseja fazer upload do arquivo ZIP.
1. Clique em **Documentos** no painel esquerdo.
1. Clique em **Adicionar novo** e em **Prova** no menu exibido.
1. Na seção **Adicionar arquivos**, arraste e solte ou procure o arquivo ZIP necessário.
1. Clique em **Criar prova** para criar uma prova simples sem processo de revisão.\
   ou\
   Continue configurando uma prova avançada:

   * [Criar uma prova avançada com um fluxo de trabalho básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Criar uma prova avançada com um fluxo de trabalho automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
