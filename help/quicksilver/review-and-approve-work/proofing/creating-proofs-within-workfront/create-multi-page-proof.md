---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Criar uma prova de várias páginas
description: É possível combinar vários arquivos em uma única prova de várias páginas. Os revisores podem usar as ferramentas de navegação no visualizador de provas para navegar pelas páginas em uma prova de várias páginas.
author: Courtney
feature: Digital Content and Documents
exl-id: a8ad80d8-0758-4fea-824e-8c206424e295
source-git-commit: ac908d52d1538b1ffe7d9bfca94cb9921445633d
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 0%

---

# Criar uma prova de várias páginas

É possível combinar vários arquivos em uma única prova de várias páginas. Os revisores podem usar as ferramentas de navegação no visualizador de provas para navegar pelas páginas em uma prova de várias páginas.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Plano atual: Pro ou Superior</p> <p>ou</p> <p>Plano herdado: Select ou Premium</p> <p>Para obter mais informações sobre acesso de revisão de texto com os diferentes planos, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de revisão de texto no Workfront</a>.</p> </td> 
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

&#42;Para saber qual perfil de plano, licença ou permissão de prova você tem, contate o administrador do Workfront ou do Workfront Proof.

+++

## Criar uma prova de várias páginas

Quando essa opção está ativada, os arquivos estáticos e os sites ficam disponíveis em uma única prova. Quando essa opção está desativada, todos os documentos e sites são gerados como provas individuais e você pode carregar até 100 arquivos em um determinado momento.

Para criar uma prova de várias páginas:

1. Vá para o projeto, tarefa ou problema em que deseja a prova e clique na seção **Documentos**.
1. Clique em **Adicionar novo** > **Prova**.
1. Arraste e solte os arquivos ou procure e selecione-os no explorador de arquivos. É possível carregar até 50 arquivos de cada vez. Para obter informações sobre limites de arquivos, consulte a seção [Considerações](#considerations) neste artigo.

   >[!NOTE]
   >
   >Arquivos interativos, incluindo vídeos e sites interativos, não podem ser combinados em uma única prova.

1. Em **Prova única**, habilite a opção **Combinar todos os arquivos compatíveis em uma única prova**.
1. No campo **Nome da prova**, especifique um novo nome para a prova combinada.
1. (Opcional) Na lista de arquivos que você carregou, reordene os arquivos arrastando-os. A ordem dos arquivos é a ordem de página da prova combinada.
1. (Opcional) Para remover um único arquivo da página Nova prova, passe o mouse sobre o arquivo e clique no ícone **Lixeira**, que aparece à direita.

   Ou

   Para excluir todos os arquivos carregados de uma só vez, clique em **Excluir tudo** no canto superior direito da lista.

1. Depois que todos os arquivos forem carregados, você deve decidir se deseja configurar uma prova básica ou uma prova automatizada:

   * Com uma prova básica, é possível adicionar quantos revisores quiser a uma prova, mas eles não são organizados em estágios. Todos os revisores adicionados podem acessar a prova imediatamente após criá-la. Para configurar uma prova básica, consulte [Criar uma prova avançada com um fluxo de trabalho básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md).
   * Com uma prova automatizada, a prova vai de estágio para estágio e o Adobe Workfront notifica cada usuário quando chegar a sua vez de revisá-la. para configurar uma prova automatizada, consulte [Criar uma prova avançada com um fluxo de trabalho automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Considerações {#considerations}

Considere o seguinte ao combinar arquivos em uma única prova:

* É possível carregar até 500 arquivos separados.
* É possível combinar arquivos estáticos de diferentes tipos (por exemplo, PDF, JPG, DOC, PPT, EXC), até um total de 2.000 páginas.
* Você pode combinar capturas estáticas da Web.
* É possível combinar arquivos GIF; no entanto, os GIF animados são processados como arquivos estáticos.
* Não é possível combinar arquivos AV e capturas da Web interativas.
* A imagem da miniatura da prova é retirada da primeira página da prova (consulte [Gerenciar detalhes da prova no Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)).
* Você pode verificar os nomes dos arquivos que foram combinados para criar a prova na página Detalhes da prova. Para obter mais informações, consulte [Gerenciar detalhes da prova no Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
* Se a opção para baixar os arquivos originais estiver ativada na prova, você poderá baixar todos os arquivos que foram combinados para criar a prova como um arquivo .zip. Para obter mais informações, consulte  [Baixar Arquivos Armazenados no Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).
