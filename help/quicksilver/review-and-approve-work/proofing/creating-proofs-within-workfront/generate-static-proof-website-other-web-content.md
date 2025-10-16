---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Criar uma prova estática para um site ou outro conteúdo da Web
description: Você pode gerar uma nova prova estática ou uma nova versão de uma prova estática existente para conteúdo da Web. O conteúdo da Web pode incluir itens como anúncios com vídeo em streaming, animações do HTML ou banners interativos, mas ele será cortado em várias capturas de tela para permitir provas estáticas.
author: Courtney
feature: Digital Content and Documents
exl-id: 1c0511f6-c60b-4a81-bfff-55b6f866add6
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 1%

---

# Criar uma prova estática para um site ou outro conteúdo da Web

Você pode gerar uma nova prova estática ou uma nova versão de uma prova estática existente para conteúdo da Web. O conteúdo da Web pode incluir itens como anúncios com vídeo em streaming, animações do HTML ou banners interativos, mas ele será cortado em várias capturas de tela para permitir provas estáticas.

Considere o seguinte ao criar provas estáticas para um site ou outro conteúdo da Web:

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> 
   <p>Standard</p>
   <p>Trabalho ou Plano</p> </td> 
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

## Criar uma prova estática para um site ou outro conteúdo da Web

Para criar uma prova estática, o site precisa estar acessível publicamente (não por trás de um firewall) ou a inclui na lista de permissões de sua organização deve incluir o domínio do Workfront. O Workfront não pode capturar um site protegido por senha como uma prova estática.

>[!TIP]
>
>Recomendamos provas interativas em vez de provas estáticas para páginas internas que exigem autorização e páginas protegidas por senha. Para obter mais informações, consulte [Visão geral das provas de conteúdo interativo](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Vá para o projeto, tarefa ou problema em que deseja criar uma nova prova de site ou uma nova versão de uma existente.
1. Clique em **Documentos** no painel esquerdo.
1. (Condicional) Se estiver criando uma nova prova, clique em **Adicionar novo** e em **Prova** no menu exibido.
1. (Condicional) Se você estiver criando uma nova versão de uma prova existente:

   1. Passe o mouse sobre a prova de URL para a qual deseja criar uma nova versão e selecione-a clicando no plano de fundo azul-claro ao redor dela.

      ![Select_proof_by_selection_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. Clique em **Adicionar novo** > **Versão** > **Prova**.

1. Digite a URL do site que deseja revisar na área **Adicionar arquivos** e pressione **Enter**.

   >[!NOTE]
   >
   > A URL deve ter menos de 2.000 caracteres.

1. Clique no URL adicionado.

   As opções para configurar a prova do site são exibidas.

   ![Prova interativa](assets/interactive-proof-radio-btn-area-350x199.png)

1. (Opcional) Se você deseja alterar o nome da prova da URL do site para algo diferente, digite um **Nome da prova.**
1. Verifique se a **Capturar captura de tela** está selecionada e use uma das seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Resolução da captura de tela</strong> </td> 
      <td> <p>Ajuste a resolução do seu conteúdo quando os revisores visualizarem a prova, permitindo que eles vejam como ele aparece em dispositivos de tamanhos variados, como telefones, tablets e monitores.</p> <p>Se você selecionar várias resoluções, uma prova separada será criada para cada resolução selecionada.</p> <p>Observação: quando um revisor comenta na prova, o comentário inclui a resolução que mostra quando o comentário foi feito para que outros revisores saibam qual resolução está associada ao comentário. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Procurar subpáginas</strong> </td> 
      <td> <p>Capture as subpáginas do site, bem como suas páginas principais. Você pode clicar em Selecionar tudo para incluir todas as páginas, ou pode clicar somente em determinadas páginas que deseja incluir. Os botões com sinal de mais e menos permitem expandir e fechar as áreas de subpágina no site.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >Não é possível alterar a configuração Capturar captura de tela para qualquer versão subsequente da prova que você criar.

1. Clique em **Concluído**.

   Se você selecionou várias resoluções de captura de tela na etapa 8, a lista inclui um conjunto de capturas de tela para cada resolução. Você pode gerar essas capturas de tela como provas separadas ou combiná-las em uma única prova (consulte  em .). Recomendamos que você as combine, especialmente se estiver criando uma prova estática de site.

   >[!NOTE]
   >
   >Se você estiver adicionando uma nova versão a uma prova de URL existente, todas as opções configuradas na prova original ou na versão anterior serão mantidas nesta versão.

1. Clique em **Criar prova** para criar uma prova simples sem processo de revisão.\
   ou\
   Continue configurando uma prova avançada:

   * [Criar uma prova avançada com um fluxo de trabalho básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Criar uma prova avançada com um fluxo de trabalho automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
