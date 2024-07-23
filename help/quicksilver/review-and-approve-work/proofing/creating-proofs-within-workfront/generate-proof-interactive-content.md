---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Criar uma prova para conteúdo interativo em um arquivo ZIP
description: Você pode gerar uma prova para conteúdo interativo que não seja de sites armazenado em um arquivo ZIP. Exemplos desse tipo de conteúdo da Web incluem anúncios com streaming de vídeo ou áudio, animações HTML, banners interativos.
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
source-git-commit: ac908d52d1538b1ffe7d9bfca94cb9921445633d
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 1%

---

# Criar uma prova para conteúdo interativo em um arquivo ZIP

Você pode gerar uma prova para conteúdo interativo que não seja de sites armazenado em um arquivo ZIP. Exemplos desse tipo de conteúdo da Web incluem anúncios com streaming de vídeo ou áudio, animações HTML, banners interativos.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Plano atual: Pro ou Superior</p> <p>ou</p> <p>Plano herdado: Premium</p> <p>Para obter mais informações sobre acesso de revisão de texto com os diferentes planos, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de revisão de texto no Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano atual: Trabalho ou Plano</p> <p>Plano herdado: Qualquer um (Você deve ter a prova ativada para o usuário)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de Permissões de Prova </td> 
   <td>Gerente ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual perfil de plano, função ou permissão de prova você tem, contate o administrador do Workfront ou do Workfront Proof.

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
