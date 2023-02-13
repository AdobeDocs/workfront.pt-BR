---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Imprimir um resumo de prova no Adobe Workfront
description: Você pode imprimir um resumo de prova, salvá-lo como um PDF ou exportá-lo como um arquivo XLS ou PDF que esteja otimizado para o Adobe Reader.
author: Courtney
feature: Digital Content and Documents
exl-id: 129c8e6b-5c66-445b-a5d0-7b1460aeabd6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 1%

---

# Imprimir um resumo de prova no Adobe Workfront

Você pode imprimir um resumo de prova, salvá-lo como um PDF ou exportá-lo como um arquivo XLS ou PDF que esteja otimizado para o Adobe Reader.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Plano atual: Pro ou superior</p> <p>ou</p> <p>Plano herdado: Selecionar ou Premium</p> <p>Para obter mais informações sobre como revisar o acesso com os diferentes planos, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de prova no Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano atual: Trabalho ou Plano</p> <p>Plano herdado: Qualquer (É necessário ter a prova ativada para o usuário)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de Permissões de Prova </td> 
   <td>Gerente ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, função ou Perfil de permissão de prova você possui, entre em contato com o administrador da Workfront ou da Workfront Proof.

## Imprima um resumo de prova ou salve-o como um arquivo PDF

Você pode imprimir um resumo de prova diretamente da lista de documentos.

>[!NOTE]
>
>Não é possível imprimir vários resumos de prova a partir da lista de documentos ao mesmo tempo.

1. Na lista de documentos que contém a prova, passe o mouse sobre a linha que contém o documento e clique em **Imprimir resumo**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

   Ou

   Enquanto estiver exibindo a prova no visualizador de prova, clique no botão **Imprimir**&#x200B;ícone ![](assets/print-icon-in-pv.png) na barra de ferramentas esquerda. (Se a barra de ferramentas esquerda não estiver visível, clique no ícone Menu ![](assets/menu-icon-in-pv.png) no canto superior esquerdo do visualizador de prova.)

1. Use qualquer uma das seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Apresentar</td> 
      <td> <p>Especifique o que deseja imprimir:</p> 
       <ul> 
        <li>O <strong>Versão atual</strong> ou <strong>Todas as versões</strong> da prova</li> 
        <li>Somente a variável <strong>Páginas com comentários</strong> ou <strong>Todas as páginas</strong></li> 
        <li>Somente a variável <strong>Miniaturas de página</strong> (uma pequena renderização de cada página) ou <strong>Páginas completas</strong> (uma prova completa)<br></li> 
        <p>Observação: Para ver os números de pinos na marcação na saída impressa, é necessário selecionar Páginas completas, não Miniaturas de página. </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Classificar comentários por</td> 
      <td> <p>(Disponível somente se você selecionou Miniaturas de página acima) Especifique a ordem na qual deseja que os comentários da prova sejam impressos:</p> 
       <ul> 
        <li><strong>Mais antigo</strong>: Do primeiro comentário feito até o último</li> 
        <li><strong>Mais recentes</strong>: Do último comentário feito ao primeiro</li> 
        <li><strong>Página</strong>: Por página, da primeira página para a última ou da última página para a primeira</li> 
        <li><strong>Criador</strong>: Pelos nomes dos usuários que os adicionaram, de A-Z ou Z-A</li> 
       </ul> <p>Essas opções não afetam a saída que você exporta como um arquivo XLS ou PDF.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Filtrar comentários por</td> 
      <td> <p>Você pode usar qualquer combinação dessas opções para incluir apenas determinados comentários na saída impressa ou exportada como um arquivo XLS ou PDF:</p> 
       <ul> 
        <li>Autores selecionados (padrão)</li> 
        <li>Ações selecionadas</li> 
        <li><strong>Não resolvido</strong> status</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fluxo de trabalho</td> 
      <td> <p>(Disponível somente se a prova tiver um Fluxo de trabalho automatizado) Você pode clicar em <strong>Mostrar diagrama</strong> para incluir um diagrama na saída impressa mostrando os estágios na prova e as decisões tomadas em cada estágio. No diagrama que aparece, as cores representam decisões tomadas em um palco:</p> <p><strong>Verde</strong>: Aprovado</p> <p><strong>Azul</strong>: Pendente de uma decisão</p> <p><strong>Vermelho</strong>: Alterações na decisão necessária</p> <p><strong>Cinza</strong>: Ainda não iniciado</p> <p><strong>Amarelo</strong>: Aprovado com alterações</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Imprimir**.
1. No painel direito da janela exibida, se você quiser imprimir o resumo, clique no botão **Destino** , em seguida, clique em **Veja mais**. Clique na impressora que deseja usar na lista exibida e clique em **Imprimir**.

   Ou

   Se quiser salvar o resumo como um arquivo PDF, clique no link **Destino** , clique em **Salvar como PDF**, depois clique em **Salvar**.

## Exportar um resumo de prova como XLS ou PDF

Você pode exportar um resumo de prova para conteúdo estático como um arquivo XLS ou como um arquivo PDF. As exportações de prova incluem apenas o conteúdo da prova.

1. Na lista de documentos que contém a prova, passe o mouse sobre a linha que contém o documento e clique em **Imprimir resumo**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

1. Clique no ícone XLS ou no ícone de PDF próximo ao canto superior direito da página.

   ![](assets/xls-pdf-icons-350x136.png)

Quando o arquivo exportado estiver pronto, você receberá um email do qual poderá baixar o arquivo.

Se você exportou o resumo como um arquivo PDF, os comentários na prova são exibidos no leitor de PDF. Se um comentário tiver várias marcações associadas a ele, ele aparecerá várias vezes na lista de comentários (uma vez para cada marcação).
