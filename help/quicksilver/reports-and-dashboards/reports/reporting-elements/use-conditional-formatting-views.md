---
product-area: reporting
navigation-topic: reporting-elements
title: Usar formatação condicional em exibições
description: Ao compartilhar seus relatórios com outros usuários no Adobe Workfront, considere personalizar a exibição dos relatórios para facilitar a leitura de determinadas informações ou apenas destacá-las.
author: Nolan
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: 532ec7f7a33e1e1111a31422c5c3c442b2e176b5
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 2%

---

# Usar formatação condicional em exibições

<!--Audited: 01/2024-->

Ao compartilhar seus relatórios com outros usuários no Adobe Workfront, considere personalizar a exibição dos relatórios para facilitar a leitura de determinadas informações ou apenas destacá-las.

Você pode personalizar a guia Detalhes de seus relatórios adicionando formatação especial ou condicional à exibição de seus relatórios.

Para obter mais informações sobre como criar relatórios, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Ao formatar condicionalmente colunas na exibição do relatório, você pode configurar regras que afetam a maneira como o relatório é exibido. Quando essas condições ou regras são atendidas, a formatação especial é aplicada.

Por exemplo, se a porcentagem concluída de uma tarefa for inferior a 20%, é possível realçar o campo mostrando o número da porcentagem em negrito, texto vermelho e uma cor de fundo amarela.

Com uma view formatada condicionalmente, você pode:

* Alterar o cabeçalho de uma coluna.
* Altere o valor de uma coluna para texto ou imagem personalizados.
* Formate a exibição de um campo alterando o tipo de fonte, cor, alinhamento ou a cor do plano de fundo.

As alterações feitas na visualização do relatório só têm efeito na guia Details do relatório. Essas alterações não afetam as guias Resumo, Matriz ou Gráfico do relatório.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plano do Adobe Workfront*</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td> <p>Novo:</p> 
   <ul><li>Padrão para exibições de relatório</li>
  <li> Colaborador ou superior para exibições de lista</li></ul>

<p>Atual:</p>
   <ul>
    <li> Planejar exibições de relatório </li>
    <li> Solicitação ou superior para exibições de lista </li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> <p>Editar acesso a Relatórios, Painéis, Calendários para editar uma visualização em um relatório</p> <p><b>Nota</b></p> <p>Se você não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Gerenciar permissões para um relatório para criar ou editar uma visualização em um relatório</p> <p>Gerenciar permissões para uma exibição</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Pré-requisitos

Você deve criar um relatório antes de adicionar formatação condicional à respectiva visualização.

Para obter informações sobre como criar um relatório, consulte [Criar um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Criar uma exibição formatada condicionalmente

{{step1-to-reports}}

1. Clique no nome de um relatório em que você deseja criar uma exibição formatada condicionalmente

   Ou

   Clique em **Novo Relatório**, em seguida, selecione um tipo de objeto para criar um novo relatório.

1. (Condicional) Se você editar um relatório existente, clique em **Ações de Relatório** e, em seguida, clique em **Editar**.

1. No **Colunas (Exibir)** clique para selecionar uma coluna existente ou clique em **Adicionar coluna** para criar uma coluna.
1. No **Mostrar nesta coluna** no canto superior esquerdo do report builder, selecione o campo que deseja exibir na nova coluna.
1. Clique em **Opções avançadas**.

1. Especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Personalizar rótulo da coluna</strong></td> 
      <td> <p>Especifique um nome para a coluna.</p> <p>Se você estiver editando uma coluna existente, a especificação de um nome aqui altera o nome da coluna existente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formato do campo</strong></td> 
      <td>Escolha o formato em que o valor na coluna é exibido. Dependendo do campo de coluna, permite definir como datas, números ou moeda serão exibidos. Nem todas as colunas exibem essa opção.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostrar esta coluna quando estiver em um Painel</strong></td> 
      <td>Selecione esse campo se desejar que a coluna seja exibida quando o relatório for colocado em um painel. A coluna sempre é exibida quando você observa o relatório fora de um painel.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Adicionar uma Regra para esta Coluna**.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. No **Quando a:** defina uma declaração de condição para a coluna.

   Por exemplo: &quot;quando o Percentual concluído da tarefa for igual a (diferencia maiúsculas de minúsculas) 50&quot;.
1. No **Mostrar o campo desta forma:** especifique a aparência desse campo quando a condição definida acima for atendida.

   Especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Cor do texto</strong></td> 
      <td> <p>Selecione a cor na qual o texto será exibido. Há 8 cores disponíveis.</p> <p><b>Nota</b></p> <p> Se o campo contiver um hiperlink, as seleções de cor do texto não serão aplicadas a esse campo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formato do texto</strong></td> 
      <td>Selecione se o texto deve ser exibido em negrito ou itálico.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Alinhamento do texto</strong></td> 
      <td>Selecione se deseja alinhar o texto à direita, no centro ou à esquerda dentro da coluna.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Histórico</strong></td> 
      <td>Selecione a cor do plano de fundo do texto. Há 8 cores disponíveis.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostrar ícone</strong></td> 
      <td>Selecione um dos 16 ícones, se desejar exibir um ícone em vez do valor real para essa coluna.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostrar texto</strong></td> 
      <td> <p>Selecione essa opção para exibir um rótulo personalizado para essa coluna, em vez do valor real. Especifique o texto a ser exibido em vez do valor no campo fornecido.</p> <p><b>IMPORTANTE</b></p> <p>Selecionar <strong>Mostrar texto</strong> desativa a capacidade de editar o texto em linha nesta coluna.<br>Além disso, não é possível alterar o valor de uma coluna Predecessora porque ela contém lógica interna.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Aplicar a toda a linha</strong></td> 
      <td>Selecione esta opção para aplicar configurações a toda a linha, em vez de aplicar configurações apenas à coluna selecionada.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Adicionar regra**.\
   É possível adicionar regras à mesma coluna ou adicionar regras a outras colunas.

   As regras são aplicadas na ordem em que foram criadas. Eles são combinados, mas não se substituem, embora uma regra de coluna tenha precedência sobre uma regra de linha na mesma célula.

   **EXEMPLO 1**

   Primeiro, é possível criar uma regra informando que, quando um projeto estiver no Status de criação, a cor do texto será roxa e negrito. Em seguida, você cria uma segunda regra que declara que, quando o Nome de uma tarefa não está em branco, a cor do texto é vermelha e em itálico e a cor do plano de fundo é verde. Neste exemplo, ocorre o seguinte:

   * As tarefas cujo status do projeto é Criação são exibidas em texto roxo e negrito. Se o nome da tarefa não estiver em branco, as tarefas também terão um plano de fundo verde.
   * Tarefas cujo Status do Projeto é qualquer coisa diferente de Criação (e o Nome da Tarefa não está em branco) são exibidas em um texto vermelho e em itálico com um fundo verde.

   **EXEMPLO 2**

   Crie uma regra na coluna Data de conclusão planejada do projeto que afete a linha inteira, tornando o plano de fundo cinza se o projeto for cancelado (por exemplo, quando o Status do projeto for Desativado). Em seguida, crie uma regra de coluna que torne o plano de fundo vermelho quando a Data de conclusão planejada do projeto for anterior à data de hoje (o que significa que o projeto está atrasado). Neste exemplo, se um projeto cancelado tiver uma data de conclusão atrasada, essa célula aparecerá vermelha mesmo que as outras células na linha estejam em cinza. Para corrigir essa formatação:

   * Edite a formatação para a Data de conclusão planejada e exclua a regra de coluna para o plano de fundo vermelho em projetos atrasados.
   * Adicione uma regra de coluna com a mesma formatação da regra de linha (plano de fundo cinza quando o Status do projeto for = Inativo).
   * Adicione a regra de coluna novamente para o plano de fundo vermelho em projetos atrasados.
   * Ao salvar as regras e a visualização, o plano de fundo vermelho não é aplicado a um projeto cancelado.

1. Clique em **Concluído**.
1. Clique em **Salvar + Fechar**.\
   No relatório, os usuários veem as alterações no formato se as condições especificadas tiverem sido atendidas.
