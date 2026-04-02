---
title: Visão geral da versão do primeiro trimestre de 2026
description: Esta página fornece informações sobre as funcionalidades incluídas na versão do primeiro trimestre de 2026. Essas melhorias estão previstas para serem disponibilizadas no ambiente de produção ao longo do trimestre.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: ed348f44-eae1-4478-8425-6114f2b310ad
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '2885'
ht-degree: 100%

---

# Visão geral da versão do primeiro trimestre de 2026

Esta página fornece informações sobre as funcionalidades incluídas na versão do primeiro trimestre de 2026, prevista para janeiro de 2026.

As melhorias nesta página estão disponíveis no ambiente de pré-visualização. Esta página será atualizada com melhorias adicionais à medida que a versão do primeiro trimestre de 2026 se aproxima de sua data prevista para produção.


<!--
 Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>.
-->

>[!IMPORTANT]
>
>
>As versões mensais e trimestrais estão previstas para serem disponibilizadas na quinta-feira da segunda semana completa do mês, salvo indicação em contrário.
>
>| Versão mensal | Versão trimestral |
>|----|----|
>| <ul><li>25.11 (13 de novembro de 2025)</li><li>25.12 (11 de dezembro de 2025)</li><li>26.1 (14 de janeiro de 2026)</li></ul> | <ul><li>26.1 (15 de janeiro de 2026)</li></ul> |
>
>Observe que, para a versão final de cada trimestre (26.1 neste trimestre), os usuários no cronograma de lançamento rápido receberão a versão um dia antes (14 de janeiro de 2026).
>
>Para obter mais informações sobre o processo de lançamento rápido, consulte [Habilitar ou desabilitar o processo de lançamento rápido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Aprimoramentos do Adobe Workfront

* [Aprimoramentos do administrador](#administrator-enhancements)
* [Aprimoramentos de documentos e aprovações](#documents-and-approvals-enhancements)
* [Aprimoramentos na página inicial](#home-enhancements)
* [Aprimoramentos de integração](#integration-enhancements)
* [Aprimoramentos de projeto](#project-enhancements)
* [Aprimoramentos nos relatórios](#reporting-enhancements)
* [Aprimoramentos nas solicitações](#requests-enhancements)
* [Outros aprimoramentos](#other-enhancements)

### Aprimoramentos do administrador

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Recurso</strong>
        </td>
        <td><strong>Pré-visualização</strong></td>
        <td><strong>Lançamento rápido</strong></td>
        <td><strong>Trimestralmente</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Gerenciar prioridades no modelo de layout</a>
            <p><span class="preview">Temporariamente indisponível no ambiente de pré-visualização</span></p>
            <p>Agora você pode habilitar ou desabilitar prioridades para usuários específicos no modelo de layout. Se você já tinha as prioridades desabilitadas para sua organização, elas permanecerão desabilitadas no modelo de layout com essa alteração.</p>
        </td>
        <td>18 de dezembro de 2025</td>
        <td>14 de janeiro de 2025</td>
        <td>15 de janeiro de 2025</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Verifique se há conflitos entre vários formulários para campos personalizados calculados</a>
            <p>Para fornecer visibilidade sobre quais objetos podem ser afetados ao editar uma expressão em campos personalizados, adicionamos uma opção para verificar se há conflitos. Esta caixa de diálogo mostra todos os objetos que podem ser afetados pela alteração da fórmula, agrupados por tipo de objeto. Você pode navegar até os detalhes de cada objeto e revisar os campos para decidir se o campo deve ser removido de algum dos formulários ou se a expressão deve permanecer inalterada.</p>
        </td>
        <td>18 de dezembro de 2025</td>
        <td>14 de janeiro de 2025</td>
        <td>15 de janeiro de 2025</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Data de entrada e ID do Cadastrador armazenados em objetos personalizados</a><p>[!BADGE Off schedule]{type=Neutral}</p>
            <p>A data de entrada e a ID de quem realizou a entrada agora são armazenados em formulários personalizados, campos e seções. Você pode usar essas opções de dados em relatórios como filtros, exibições ou agrupamentos. Para exibi-los na lista de formulários personalizados, campos ou seções em Configuração, adicione “Data de entrada” e “Inserido por: nome” como colunas em uma exibição nova ou já existente.</p>
        </td>
        <td>13 de novembro de 2025</td>
        <td>13 de novembro de 2025</td>
        <td>13 de novembro de 2025</td>
    </tr>  
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Atualizações dos nomes dos botões ao editar um modelo de layout</a>
            <p>Para proporcionar mais consistência com outras áreas da Configuração, como o designer de formulários personalizados, os botões exibidos ao editar um modelo de layout foram alterados para Aplicar, Salvar e Fechar e Cancelar. A nova opção, Aplicar, permite salvar as alterações no modelo de layout e continuar editando. Anteriormente, as opções disponíveis eram Salvar e Cancelar. </p>
        </td>
        <td>30 de outubro de 2025</td>
        <td>13 de novembro de 2025</td>
        <td>15 de janeiro de 2026</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}"> Gerenciamento de campo aprimorado com sinalizador Ativo em campos personalizados</a>
            <p>Quando há um grande número de campos personalizados no sistema, o gerenciamento desses campos em formulários e relatórios personalizados pode ser difícil. Agora você pode marcar campos personalizados como inativos com o novo sinalizador <b>Ativo</b>. Este sinalizador está disponível ao trabalhar com um campo em um formulário personalizado ou ao adicionar ou editar um campo da lista Campos. </p>
        </td>
        <td>30 de outubro de 2025</td>
        <td>13 de novembro de 2025</td>
        <td>15 de janeiro de 2026</td>
    </tr>   
  </tbody>
</table>

### Aprimoramentos de documentos e aprovações

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Recurso</strong>
        </td>
        <td><strong>Pré-visualização</strong></td>
        <td><strong>Lançamento rápido</strong></td>
        <td><strong>Trimestralmente</strong></td>
        </tr>
       <!--
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Set up brands for the AI reviewer in Workfront<p>[!BADGE Off schedule]{type=Neutral}</p> </a>
            <p>You can now set up brands for the AI reviewer in the Workfront Setup area. This allows you to customize the AI review process based on your organization's branding guidelines.</p>
            <p>The AI reviewer is currently in beta.</p>
        </td>
        <td>January 8, 2026</td>
        <td>January 8, 2026</td>
        <td>January 8, 2026</td>
    </tr>
    -->
    </tr>
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Escolha um projeto do Workfront ao enviar uma revisão no Adobe Express<p>[!BADGE Off schedule]{type=Neutral}</p> </a>
            <p>Você pode escolher um projeto do Workfront para o qual enviar uma prova. Isso ajuda a manter todos os ativos e provas relacionados organizados dentro do mesmo projeto.</p>
        </td>
        <td>15 de dezembro de 2025</td>
        <td>15 de dezembro de 2025</td>
        <td>15 de dezembro de 2025</td>
    </tr> 
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Suporte interorganizacional para o Adobe Express com o Workfront Proofing<p>[!BADGE Off schedule]{type=Neutral}</p> </a>
            <p>Estamos introduzindo o suporte entre organizações para o Adobe Express com o Workfront Proof. Esse aprimoramento permite que clientes que operam em várias organizações IMS utilizem e gerenciem fluxos de trabalho de revisão de forma integrada.</p>
        </td>
        <td>13 de novembro de 2025</td>
        <td>13 de novembro de 2025</td>
        <td>13 de novembro de 2025</td>
    </tr>   
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">O Adobe Experience Manager agora está disponível com a integração do Frame.io <p>[!BADGE Off schedule]{type=Neutral}</p> </a>
            <p>Agora você pode usar o Experience Manager Assets para gerenciar e armazenar seus ativos digitais que passaram pelo ciclo de revisão e aprovação. Essa integração permite que você aproveite os recursos do Adobe Experience Manager, Frame.io e Workfront para otimizar seus processos de gestão de conteúdo e colaboração. </p>
        </td>
        <td>30 de outubro de 2025</td>
        <td>30 de outubro de 2025</td>
        <td>30 de outubro de 2025</td>
    </tr>   
  </tbody>
</table>



### Aprimoramentos na página inicial

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Recurso</strong>
        </td>
        <td><strong>Pré-visualização</strong></td>
        <td><strong>Lançamento rápido</strong></td>
        <td><strong>Trimestralmente</strong></td>
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-home.md" class="MCXref xref" xrefformat="{para}">Atualização do widget Menções na página inicial</a>
            <p>Fizemos as seguintes melhorias no widget Menções na página inicial: <ul><li>A mesma experiência na área Atualizações da maioria dos objetos do Workfront agora também está disponível no widget Menções na página inicial. </li><li>O widget Menções agora contém os comentários que o usuário fez ou nos quais foi marcado nas últimas duas semanas</li><ul></p>
        </td>
        <td>17 de dezembro de 2025</td>
        <td>14 de janeiro de 2026</td>
        <td>15 de janeiro de 2026</td>
    </tr>   
  </tbody>
</table>

### Aprimoramentos de integração

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Recurso</strong>
        </td>
        <td><strong>Pré-visualização</strong></td>
        <td><strong>Lançamento rápido</strong></td>
        <td><strong>Trimestralmente</strong></td>
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">Escolha um projeto Workfront ao enviar uma revisão no Creative Cloud Express.</a><p>[!BADGE Off schedule]{type=Neutral}</p>
            <p>Você pode escolher um projeto do Workfront para o qual enviar uma prova. Isso ajuda a manter todos os ativos e provas relacionados organizados dentro do mesmo projeto. </p>
        </td>
        <td>15 de dezembro de 2025</td>
        <td>15 de dezembro de 2025</td>
        <td>15 de dezembro de 2025</td>
    </tr>   
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">Seletor de ativos atualizado para a integração nativa do Adobe Workfront com o Experience Manager Assets. </a>
            <p>Atualizamos o seletor de ativos na integração do Adobe Workfront para o Experience Manager Assets. Com essa atualização, agora é possível selecionar e enviar coleções do AEM diretamente para o Workfront. </p>
        </td>
        <td>20 de novembro de 2025</td>
        <td>11 de dezembro de 2025</td>
        <td>15 de janeiro de 2026</td>
    </tr>   
    <!--
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">New version of Salesforce integration now available </a>
            <p>To stay up-to-date with recent changes to the Workfront API, we've created a new Salesforce integration. The new integration features the same functionality as the previous version, and was updated to avoid losing functionality deprecated in the API.</p><p>NOTE: The Workfront for Salesforce integration, including the new version, will not be available after **February 28, 2026**. </p>
        </td>
        <td>October 30, 2025</td>
        <td>October 30, 2025</td>
        <td>October 30, 2025</td>
    </tr>
    -->
  </tbody>
</table>

### Aprimoramentos de projeto

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Recurso</strong>
        </td>
        <td><strong>Pré-visualização</strong></td>
        <td><strong>Lançamento rápido</strong></td>
        <td><strong>Trimestralmente</strong></td>
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-projects.md" class="MCXref xref" xrefformat="{para}">Usuários Light podem registrar horas em projetos</a>
            <p>Os usuários com licença Light agora podem registrar o tempo diretamente nos projetos. Anteriormente, apenas usuários com uma licença Padrão podiam registrar o tempo em projetos.</p>
        </td>
        <td>11 de dezembro de 2025</td>
        <td>15 de janeiro de 2026</td>
        <td>15 de janeiro de 2026</td>
    </tr>   
  </tbody>
</table>

### Aprimoramentos nos relatórios

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Recurso</strong>
        </td>
        <td><strong>Pré-visualização</strong></td>
        <td><strong>Lançamento rápido</strong></td>
        <td><strong>Trimestralmente</strong></td>
    </tr>
 <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Atualizações de moedas nos painéis da Tela</a>
            <p>Fizemos as seguintes atualizações para os campos de moeda:<ul><li>Quando várias moedas são definidas no Workfront, agora você pode escolher uma moeda padrão para o painel durante a criação. </li><li>Ao criar um relatório, você pode bloquear um campo de moeda. Isso garante que a preferência de moeda no painel não afete a exibição desses valores.</li><li>Ao visualizar um painel, os usuários podem usar o botão de alternância entre quaisquer moedas definidas no Workfront. Essas alterações se aplicam a todo o painel, com exceção dos campos de moeda bloqueados</li></ul></p>
        </td>
        <td>18 de dezembro de 2025</td>
        <td>14 de janeiro de 2026</td>
        <td>15 de janeiro de 2026</td>
    </tr>
 <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}"> Resultados da pesquisa rápida na tabela em painéis de tela</a>
            <p>Adicionamos uma pesquisa rápida aos relatórios da tabela. Esta pesquisa funciona em todas as páginas, para que você possa encontrar dados mesmo que eles não estejam visíveis no momento.</p>
        </td>
        <td>18 de dezembro de 2025</td>
        <td>14 de janeiro de 2026</td>
        <td>15 de janeiro de 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Nova opção Mostrar total para gráficos de pizza</a>
            <p>Introduzimos uma nova opção Mostrar total que converte gráficos de pizza em gráficos de rosquinha. Esse recurso permite que os usuários exibam um valor central que representa o total de todos os segmentos no gráfico.</p>
        </td>
        <td>18 de dezembro de 2025</td>
        <td>14 de janeiro de 2026</td>
        <td>15 de janeiro de 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Novas opções de configuração para gráficos de pizza nos painéis da tela</a>
            <p>Introduzimos duas novas opções de configuração para gráficos de pizza: <ul><li>Ocultar rótulos de segmentos: agora você pode optar por ocultar os rótulos de segmentos em um gráfico de pizza se eles forem muito longos e prejudicarem a legibilidade do gráfico.</li><li>Ocultar e reposicionar a legenda do gráfico: agora você pode optar por ocultar a legenda de um gráfico de pizza. Você também pode definir a posição da legenda à direita (padrão), à esquerda, na parte superior ou inferior do gráfico. </li></ul></p>
        </td>
        <td>18 de dezembro de 2025</td>
        <td>14 de janeiro de 2026</td>
        <td>15 de janeiro de 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Melhorias na contagem de agrupamentos dos painéis de tela</a>
            <p>Atualizamos a barra de agrupamento nos painéis de tela para exibir a contagem de registros da página atual e a contagem geral de registros do agrupamento em todas as páginas. </p>
        </td>
        <td>18 de dezembro de 2025</td>
        <td>14 de janeiro de 2026</td>
        <td>15 de janeiro de 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Novo recurso de linha de referência nos relatórios dos painéis de tela</a>
            <p>Agora é possível definir uma linha de referência nos gráficos de barra, coluna e linha para definir uma meta ou um limite para seus relatórios baseados em séries. </p>
        </td>
        <td>18 de dezembro de 2025</td>
        <td>14 de janeiro de 2026</td>
        <td>15 de janeiro de 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Personalizar rótulos de eixos em relatórios de gráficos nos painéis de tela</a>
            <p>Agora é possível personalizar os rótulos de eixo nos relatórios de gráfico. Esse novo recurso permite inserir um rótulo de eixo de substituição para ser exibido em vez do objeto padrão e do caminho de campo. Além disso, você pode optar por ocultar totalmente os rótulos dos eixos.</p>
        </td>
        <td>18 de dezembro de 2025</td>
        <td>14 de janeiro de 2026</td>
        <td>15 de janeiro de 2026</td>
    </tr>   
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Duplicar um relatório em um painel de tela</a><p>[!BADGE Off schedule]{type=Neutral}</p>
            <p>Agora é possível duplicar um relatório de KPI, tabela ou gráfico em um painel de tela após sua criação. Após a duplicação, é possível editar o relatório conforme necessário antes de salvar.</p>
        </td>
        <td>23 de outubro de 2025</td>
        <td>23 de outubro de 2025</td>
        <td>23 de outubro de 2025</td>
    </tr>   
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Remover opções de campo dos filtros do relatório</a>
            <p>Removemos as seguintes opções de campo que estavam disponíveis anteriormente ao aplicar um filtro a um relatório:
            <ul>
            <li>IDs de outros grupos</li>
            <li>IDs de outras funções</li>
            <li>IDs de outras equipes</li>
            </ul>
            </p>
        </td>
        <td>6 de novembro de 2025</td>
        <td>13 de novembro de 2025</td>
        <td>15 de janeiro de 2026</td>
    </tr>    
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Novas proteções para melhorar os tempos de carregamento nos painéis de tela</a>
            <p>Para evitar atrasos de tempo de carregamento e melhorar o desempenho geral nos painéis de tela, aplicamos limites em quantos componentes de painel podem ser adicionados a um painel:
            <ul>
            <li>Relatórios por painel: limite de 25</li>
            <li>Agrupamentos em exibições em tabela: limite de 5</li>
            <li>Distância do objeto base do relatório: limite de 10</li>
            <li>Colunas em uma exibição em tabela: limite de 25</li>
            <li>Prompts de filtro no nível do painel: limite de 10</li>
            </ul></p>
        </td>
       <td>6 de novembro de 2025</td>
        <td>13 de novembro de 2025</td>
        <td>15 de janeiro de 2026</td>
    </tr>   
  </tbody>
</table>

### Aprimoramentos nas solicitações

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Recurso</strong>
        </td>
        <td><strong>Pré-visualização</strong></td>
        <td><strong>Lançamento rápido</strong></td>
        <td><strong>Trimestralmente</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Os links dos objetos criados agora estão disponíveis na área Solicitações e no widget Minhas solicitações.</a>
            <p>Para facilitar o acesso ao objeto criado por uma solicitação específica, adicionamos links à coluna Objeto criado. Agora, você pode clicar no link nesta coluna para ser direcionado diretamente para a página do objeto criado.</p>
        </td>
        <td>18 de dezembro de 2025</td>
        <td>14 de janeiro de 2026</td>
        <td>15 de janeiro de 2026</td>
    </tr> 
    <!--
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Create groupings in the Requests list and My Requests widget</a>
            <p>To make it easier for you to find the requests you need, we've added groupings to the Requests list and the My Requests widget. Now, you can group requests by any column on the list. These groupings become part of the view that you are using when you create the grouping.</p>
        </td>
        <td>December 18, 2025</td>
        <td>January 14, 2026</td>
        <td>January 15, 2026</td>
    </tr>
    -->
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Adicionar campos personalizados à lista de Solicitações e ao widget Minhas solicitações.</a>
            <p>Para facilitar a visualização das informações necessárias, adicionamos a possibilidade de incluir campos personalizados como colunas na lista Solicitações e no widget Minhas solicitações na página inicial. Agora, você pode adicionar campos de formulários personalizados como uma coluna, e as solicitações que tiverem informações nesses campos exibirão essas informações na lista ou no widget.</p><p>Esta funcionalidade está disponível apenas na nova experiência de Solicitações.</p>
        </td>
        <td>18 de dezembro de 2025</td>
        <td>14 de janeiro de 2026</td>
        <td>15 de janeiro de 2026</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">O curinga do usuário atual agora está disponível no filtro Solicitações</a>
            <p>Para facilitar a filtragem das solicitações que se aplicam a você, criamos um curinga para o usuário atual. Agora, ao filtrar, você pode selecionar “Eu (usuário conectado)”. O filtro será então aplicado ao usuário que estiver visualizando a lista de solicitações.   </p>
        </td>
        <td>18 de dezembro de 2025</td>
        <td>14 de janeiro de 2026</td>
        <td>15 de janeiro de 2026</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Preenchimento de formulários com tecnologia de IA agora disponível para solicitações</a>
            <p>Para facilitar a criação de solicitações, criamos o preenchimento de formulários com tecnologia de IA. Agora, você pode colar um prompt ou fazer upload de um documento para um formulário de solicitação, e a IA irá obter as informações relevantes e preencherá o formulário.  </p>
        </td>
        <td>11 de dezembro de 2025</td>
        <td>11 de dezembro de 2025</td>
        <td>11 de dezembro de 2025</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Compartilhar visualizações na área Solicitações e no widget Minhas solicitações.</a>
            <p>Para facilitar a visualização das informações necessárias, adicionamos a possibilidade de compartilhar visualizações à nova experiência de solicitação. Agora, você pode compartilhar visualizações com outros usuários, equipes ou grupos. </p>
        </td>
        <td>4 de dezembro de 2025</td>
        <td>14 de janeiro de 2026</td>
        <td>15 de janeiro de 2026</td>
    </tr> 
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Salvar rascunhos de solicitações na nova experiência de solicitação</a>
            <p>Para facilitar a criação e o envio de solicitações, adicionamos a possibilidade de salvar rascunhos à nova experiência de solicitação. Agora, quando você começa a preencher uma solicitação e a fecha, ela é salva no status Rascunho e pode ser encontrada no formulário de solicitação usado para criar o rascunho. Você pode então reabrir, atualizar e enviar o rascunho quando for conveniente. </p>
        </td>
        <td>20 de novembro de 2025</td>
        <td>14 de janeiro de 2026</td>
        <td>15 de janeiro de 2026</td>
    </tr>  
        <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Excluir solicitações enviadas na nova experiência de solicitação</a>
            <p>Para facilitar a organização e a clareza de suas solicitações, adicionamos a possibilidade de excluir solicitações à nova experiência de solicitação. Agora, você pode excluir as solicitações que enviou. Os administradores do Workfront e do espaço de trabalho do Workfront Planning também podem excluir solicitações.</p>
        </td>
        <td>20 de novembro de 2025</td>
        <td>14 de janeiro de 2026</td>
        <td>15 de janeiro de 2026</td>
    </tr>   
        <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Criar novas solicitações copiando solicitações enviadas anteriormente na nova experiência de solicitação</a>
            <p>Para facilitar o envio de solicitações, adicionamos a possibilidade de copiar solicitações para a nova experiência de solicitação. Agora, você pode copiar uma solicitação, editar qualquer campo e enviá-la como uma nova solicitação. </p>
        </td>
        <td>20 de novembro de 2025</td>
        <td>11 de dezembro de 2025</td>
        <td>15 de janeiro de 2026</td>
    </tr>    
  </tbody>
</table>

### Outros aprimoramentos

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>Recurso</strong>
        </td>
        <td><strong>Pré-visualização</strong></td>
        <td><strong>Lançamento rápido</strong></td>
        <td><strong>Trimestralmente</strong></td>
    </tr>   
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}">Atualizações de aparência durante o período de lançamento do primeiro trimestre de 2026</a>
                        <p>Pequenas atualizações na aparência de várias áreas do aplicativo Adobe Workfront estão sendo feitas dentro do período do primeiro trimestre de 2026. </p>
                    </td>
                    <td><p>Ao longo do período de lançamento do primeiro trimestre de 2026<br /></p>
                    <td colspan="2"><p>Lançamento rápido: no mínimo uma semana após o lançamento em pré-visualização (a menos que especificado de outra forma)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                 <td>
                <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}"> Limites de seleção em campos de seleção múltipla</a>
              <p>Os campos que permitem múltiplas seleções, como caixas de seleção e menus suspensos com seleção múltipla, agora estão limitados a 5.000 seleções quando um usuário está preenchendo o formulário.</p>
             </td>
        <td>30 de outubro de 2025</td>
        <td>13 de novembro de 2025</td>
        <td>15 de janeiro de 2026</td>
             </tr>   
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}">Adobe Unified Experience agora disponível para mais organizações do Workfront</a><p></p>
            <p>Para permitir que as organizações tenham acesso aos benefícios da Experiência Unificada da Adobe, estamos continuando a disponibilizá-la para clientes do Workfront.</p>
        </td>
        <td><p>sexta-feira, 11 de dezembro de 2025</p></td>
        <td><p>quinta-feira, 11 de fevereiro de 2026</p></td>
        <td><p>quinta-feira, 11 de fevereiro de 2026</p></td>
    <tr>
            </tbody>
        </table>


### Funcionalidade que será removida em breve do Workfront

#### Descontinuidade do campo Substituir moeda em funções de trabalho com a versão 25.11

Como parte da simplificação do modelo financeiro, iremos descontinuar o campo Substituir moeda nas funções de trabalho em pré-visualização em 30 de outubro e na Produção para todos os clientes com a versão 25.11. Essa alteração afeta a forma como as moedas e as taxas são configuradas nas funções de trabalho na área Configuração.

* Os campos **Substituir moeda** em uma função de trabalho não estarão mais disponíveis.
* Cada função no trabalho terá uma única moeda com seu custo associado e taxa de faturamento.
* Todas as moedas de substituição e seus valores de taxa serão migrados automaticamente para se tornarem a única moeda e as únicas taxas para essa função de trabalho.

## Modernização da interface

Estamos atualizando a interface em todo o Adobe Workfront para melhorar a experiência do usuário e unificá-la com outros aplicativos da Adobe. Essas alterações são lançadas fora do cronograma padrão de lançamento. Para obter uma lista dessas alterações, consulte [Modernização da interface](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

## Notas de versão para outras áreas

### Aprimoramentos do Workfront Fusion

Os novos recursos do Workfront Fusion são disponibilizados em Produção em um ritmo fora do cronograma de lançamentos padrão. Para obter mais informações sobre os recursos mais recentes, consulte [Atividade de lançamento do Adobe Workfront Fusion](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Aprimoramentos do Workfront Planning

Novos recursos no Workfront Planning estão disponíveis em Produção. Para obter mais informações sobre os recursos mais recentes, consulte [Atividade de lançamento do primeiro trimestre de 2026 para o Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-26-q1.md).

Ainda não há atualizações para o seguinte nesta versão:

* Planejador de cenários
* Proof
* Metas

## Atualizações do visualizador de prova para desktop

### Versão 2.1.54

**Lançamento de produção para todos os clientes: 11 de dezembro de 2025**

O Visualizador de prova para desktop foi atualizado da versão 2.1.52 para a 2.1.54. Essa atualização incluiu melhorias internas nas ferramentas e não impactou os recursos para o usuário final.

A versão 2.1.53 também incluiu alterações internas nas ferramentas.

Esta atualização é para Mac e Windows.

### Versão 2.1.52

**Versão de produção para todos os clientes: 31 de julho de 2025**

O Visualizador de prova para desktop foi atualizado para a versão 2.1.52, que aborda correções de erros.

A atualização 2.1.51 incluiu atualizações internas de ferramentas e não afetou os recursos para o usuário final.

Esta atualização é para Mac e Windows.

## Avisos

### API versão 21

A versão 21 da API do Workfront foi lançada em 23 de outubro de 2025. Para a versão 21 da API, modificamos alguns recursos e pontos de acesso. Algumas das alterações oferecem suporte a novas funcionalidades, enquanto outras facilitam o uso das informações disponíveis por meio da API.

>[!IMPORTANT]
>
>Esta alteração na versão da API apresenta uma mudança significativa que pode afetar suas chamadas de API. Isso se deve ao fato de que a versão 21 da API usa a versão 2 das assinaturas de eventos.
>
> Para campos de seleção múltipla, a versão 2 das Assinaturas de evento sempre envia como matriz. A versão 1 enviava uma matriz se mais de um valor fosse selecionado. Se apenas um valor fosse selecionado, ela enviaria uma string.

Para obter informações sobre as novidades e atualizações, consulte [Novidades na versão 21 da API](/help/quicksilver/wf-api/api/new-api-version-21.md).

Para obter informações sobre as versões da API, consulte [controle de versão da API e cronograma de suporte](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Nova versão do Workfront para Microsoft Teams

Como a [Microsoft faz a transição para o novo cliente Teams](https://learn.microsoft.com/pt-br/microsoftteams/teams-classic-client-end-of-availability), o cliente Classic Teams não estará mais disponível após 1º de julho de 2025. Para continuar usando o Microsoft Teams e aplicativos integrados como o Workfront, os clientes devem fazer a transição para o novo cliente Teams antes dessa data.

A integração atualizada do Workfront já está disponível e é totalmente compatível com a nova experiência do Teams. Na maioria dos casos, o Workfront aparecerá automaticamente assim que os usuários tiverem feito a transição. Caso contrário, a integração pode ser instalada manualmente a partir da App Store do Microsoft Teams. Para instalar ou verificar a integração do Workfront no novo cliente do Teams, consulte [Instalar [!DNL Adobe Workfront] para Microsoft Teams](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

### Workfront para Microsoft Outlook

[A Microsoft está desativando o suporte para tokens online do Exchange legados](https://learn.microsoft.com/pt-br/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), que atualmente são usados pelo complemento do Workfront Outlook para autenticação. Essa mudança da Microsoft já começou a afetar os clientes e continuará a ser implementada em fases até outubro de 2025.

* **Depois que a Microsoft desativar completamente esses tokens, a integração do Workfront para Microsoft Outlook não funcionará mais.**

Como parte dessa mudança, a Microsoft decidiu alterar a forma como os tokens são habilitados. Após **30 de junho de 2025**, os administradores não poderão mais habilitar os tokens por conta própria — somente o Suporte da Microsoft poderá conceder exceções. **Em 1º de outubro de 2025, os tokens legados serão desativados para todos os locatários. Exceções não serão concedidas.**

### Outras transições de integração do Workfront

Para fornecer integrações mais estáveis e escaláveis, estamos mudando para uma abordagem de integração moderna e flexível usando a Automação e Integração do Workfront (Fusion). Como parte desse processo de transição, as seguintes integrações não estarão disponíveis após **28 de fevereiro de 2026**:

* Workfront para G Suite
* Workfront para Jira
* Workfront para Salesforce.

Recomendamos usar a Automação e Integração do Workfront para as necessidades de integração de sua organização com o Google Workspace.
Para obter uma visão geral da Automação e Integração do Workfront, consulte [Visão geral do Adobe Workfront Fusion](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).


### Atualizações de manutenção do Workfront 

Para obter informações sobre as atualizações de manutenção feitas durante a versão do primeiro trimestre de 2025, consulte [Atualizações de manutenção do Workfront](https://experienceleague.adobe.com/pt-br/docs/workfront-known-issues/releases/current-updates).

### Atualizações de treinamento

Explore as últimas atualizações feitas nos programas de aprendizagem, caminhos de aprendizagem, vídeos e guias para cada versão do Adobe Workfront. Para obter mais informações, consulte a seção &quot;Novidades&quot; da [página de tutoriais do Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=pt-BR).
