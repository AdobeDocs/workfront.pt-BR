---
product-area: reporting
navigation-topic: reporting-elements
title: Usar formatação condicional em exibições
description: À medida que você compartilha seus relatórios com outros usuários no Adobe Workfront, considere personalizar a visualização dos relatórios para facilitar a leitura ou destacar algumas informações.
author: Lisa
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '1148'
ht-degree: 2%

---

# Usar formatação condicional em exibições

À medida que você compartilha seus relatórios com outros usuários no Adobe Workfront, considere personalizar a visualização dos relatórios para facilitar a leitura ou destacar algumas informações.

Você pode personalizar a guia Detalhes de seus relatórios, adicionando formatação especial ou condicional à exibição dos relatórios.

Você deve ter permissões de gerenciamento no relatório para editá-lo e adicionar formatação especial à exibição.

Para obter mais informações sobre como criar relatórios, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Ao formatar condicionalmente colunas na exibição do relatório, é possível configurar regras que afetam a forma como o relatório é exibido. Quando essas condições ou regras são cumpridas, a formatação especial é aplicada.

Por exemplo, se a porcentagem completa de uma tarefa for menor que 20%, você poderá realçar o campo mostrando o número da porcentagem em negrito, texto vermelho e uma cor de fundo amarela.

Com uma exibição formatada condicionalmente, é possível:

* Altere o cabeçalho de uma coluna.
* Altere o valor de uma coluna para texto personalizado ou uma imagem.
* Formate a exibição de um campo alterando o tipo da fonte, a cor, o alinhamento ou a cor do plano de fundo.

As alterações feitas na visualização do relatório só têm efeito na guia Details do relatório. Essas alterações não afetam as guias Resumo, Matriz ou Gráfico do relatório.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Plano Adobe Workfront*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Editar o acesso a Relatórios, Painéis, Calendários para editar uma visualização em um relatório</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Gerenciar permissões de um relatório para criar ou editar uma visualização em um relatório</p> <p>Gerenciar permissões para uma exibição</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Você deve criar um relatório antes de poder adicionar formatação condicional a ele.

Para obter informações sobre como criar um relatório, consulte [Criar um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Criar uma exibição formatada condicionalmente

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, em seguida, clique em **Relatórios**.

1. Clique no nome de um relatório onde deseja criar uma view formatada condicionalmente.

   Ou

   Clique em **Ações de Relatório**, depois clique em **Editar**.

1. (Condicional) Se você editou um relatório, selecione uma coluna existente ou crie uma nova coluna.
1. Clique em **Opções avançadas**.

1. Especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Personalizar rótulo da coluna</strong></td> 
      <td> <p>Especifique um nome para a coluna.</p> <p>Se você estiver editando uma coluna existente, especificar um nome aqui altera o nome da coluna existente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formato do campo</strong></td> 
      <td>Escolha o formato no qual o valor na coluna é exibido. Dependendo do campo de coluna, é possível definir como as datas, números ou moedas são exibidos.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostrar esta coluna quando estiver em um Painel</strong></td> 
      <td>Selecione esse campo se desejar que a coluna seja exibida quando o relatório for colocado em um painel. A coluna sempre é exibida quando você observa o relatório fora de um painel.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Adicionar uma regra para esta coluna**.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. No **Quando:** , defina uma declaração de condição para a coluna. Por exemplo: quando a porcentagem de tarefas concluída é igual a (distinção entre maiúsculas e minúsculas) 50.
1. No **Mostrar o campo desta forma:** especifique a aparência desse campo quando a condição definida acima for atendida.

   Especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Cor do texto</strong></td> 
      <td> <p>Selecione a cor na qual o texto é exibido. Há 8 cores disponíveis.</p> <p>Observação: Se o campo contiver um hiperlink, as seleções de cor do texto não serão aplicadas a esse campo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formato do texto</strong></td> 
      <td>Selecione se o texto deve ser exibido em negrito ou itálico.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Alinhamento do texto</strong></td> 
      <td>Selecione se o texto deve ser alinhado à direita, ao centro ou à esquerda dentro da coluna.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Plano de fundo</strong></td> 
      <td>Selecione a cor do plano de fundo do texto. Há 8 cores disponíveis.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostrar ícone</strong></td> 
      <td>Selecione de um dos 16 ícones, se desejar exibir um ícone em vez do valor real para essa coluna.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostrar texto</strong></td> 
      <td> <p>Selecione essa opção para exibir um rótulo personalizado para essa coluna, em vez de seu valor real. Especifique o texto a ser exibido em vez do valor no campo fornecido.</p> <p>Importante: Selecionar <strong>Mostrar texto</strong> desativa a capacidade de editar o texto em linha nesta coluna.<br>Além disso, não é possível alterar o valor de uma coluna Predecessor porque ela contém uma lógica incorporada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Aplicar a toda a linha</strong></td> 
      <td>Selecione essa opção para aplicar configurações à linha inteira, em vez de aplicar configurações somente à coluna selecionada.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Adicionar regra**.\
   Você pode adicionar regras à mesma coluna ou adicionar regras a outras colunas.

   As regras são aplicadas na ordem em que foram criadas. Elas são combinadas, mas não se substituem, embora uma regra de coluna tenha precedência sobre uma regra de linha na mesma célula.

   Exemplo 1: Primeiro, você pode criar uma regra que declara quando o Status do projeto é Criação, a cor do texto é violeta e negrito. Em seguida, você cria uma segunda regra que declara quando o Nome da tarefa não está em branco, a cor do texto é vermelha e em itálico e a cor do plano de fundo é verde. Neste exemplo, ocorre o seguinte:

   * As tarefas cujo status do projeto é Criação são exibidas em texto roxo e negrito. Se o nome da tarefa não estiver em branco, as tarefas também terão um plano de fundo verde.
   * As tarefas cujo Status do projeto seja qualquer coisa diferente de Criação (e o Nome da tarefa não estiver em branco) são exibidas em um texto vermelho e itálico com um plano de fundo verde.

   Exemplo 2: Crie uma regra na Data de Conclusão Planejada do Projeto que afete a linha inteira, tornando o plano de fundo cinza se o projeto for cancelado (Status = &quot;Morto&quot;). Em seguida, crie uma regra de coluna que torne o plano de fundo vermelho quando a Data de conclusão planejada do projeto for menor que hoje (o que significa que o projeto está atrasado). Neste exemplo, se um projeto cancelado tiver uma data de conclusão tardia, essa célula aparecerá vermelha mesmo que as outras células na linha sejam cinza. Para corrigir essa formatação:

   * Edite a formatação da Data de conclusão planejada e exclua a regra de coluna para o plano de fundo vermelho em projetos atrasados.
   * Adicione uma regra de coluna com a mesma formatação da regra de linha (fundo cinza quando o Status do projeto = &quot;Morto&quot;).
   * Adicione a regra da coluna novamente para o plano de fundo vermelho em projetos atrasados.
   * Ao salvar as regras e a visualização, o plano de fundo vermelho não é aplicado a um projeto cancelado.


1. Clique em **Concluído**.
1. Clique em **Salvar + Fechar**.\
   No relatório, os usuários veem alterações no formato se as condições especificadas foram atendidas.
