---
title: Visão geral da versão 22.2
description: Visão geral da versão 22.2
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: e490a955-b2cb-4b9b-9794-12ff2a2c2338
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '3973'
ht-degree: 0%

---

# Visão geral da versão 22.2

Esta página fornece informações sobre a funcionalidade incluída na versão 22.2 do. Todos os recursos listados estão disponíveis na nova experiência do Adobe Workfront. Alguns recursos também estão disponíveis no Adobe Workfront Classic; no entanto, o [Workfront Classic será descontinuado em março de 2022](https://one.workfront.com/s/new-workfront-experience), seguido brevemente pela data de fim da vida útil do Workfront Classic em julho de 2022.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
to help you unlock productivity and collaboration.
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment. As the 22.2 release nears its planned Production release later this year
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
the week of January 17, 2022
</MadCap:conditionalText>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in October 2021
</MadCap:conditionalText>
, this page will be updated with all functionality included with 22.2. </p>
-->

Essas melhorias foram disponibilizadas no ambiente de Produção na semana de 4 de abril de 2022.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment and will be made available in the Production environment
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
later this year
</MadCap:conditionalText>
the week of April 4, 2022, unless otherwise specified. For specific release dates and times for each cluster, see the <a href="https://status.adobe.com/en/products/5943" target="_blank">Adobe Workfront status page</a> on <a href="http://status.adobe.com/" target="_blank">status.adobe.com</a>. You must log in to see specific release times. </p>
-->

## Aprimoramentos do Adobe Workfront

* [Aprimoramentos do administrador](#administrator-enhancements)
* [Aprimoramentos do projeto](#project-enhancements)
* [Melhorias no gerenciamento de recursos](#resource-management-enhancements)
* [Aprimoramentos na página inicial](#home-enhancements)
* [Aprimoramentos móveis](#mobile-enhancements)
* [Aprimoramentos de integrações](#integrations-enhancements)
* [Outras melhorias](#other-enhancements)

### Melhorias do administrador {#administrator-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Recurso</strong> </p> </td> 
   <td> <p><strong>Datas e ambientes de lançamento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">Configurar um formulário personalizado para trabalhar com vários tipos de objeto</a> </p> <p>Agora é possível configurar um formulário personalizado novo ou existente para funcionar com vários tipos de objeto, tornando o formulário muito mais útil. Os usuários poderão anexar e preencher o formulário em objetos de todos os tipos para os quais você o configura.</p> <p>Anteriormente, você podia configurar um formulário personalizado para funcionar com apenas um tipo de objeto.</p> <p>Essa funcionalidade funciona com todos os formulários personalizados criados anteriormente em seu sistema Workfront. Por exemplo, se você já tiver um formulário personalizado que foi criado para o tipo de objeto Tarefa, agora também poderá configurá-lo para trabalhar com outros tipos de objeto, como Projeto e Problema.</p> </td> 
   <td> <p><b>Disponível nestas datas:</b> </p> 
    <ul> 
     <li> <p>Versão de pré-visualização: 10 de março de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2 </p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#blueprin" class="MCXref xref" xrefformat="{para}">O catálogo de blueprints está disponível para todos os usuários e os administradores podem permitir solicitações</a> </p> <p>Todos os usuários do Adobe Workfront agora podem navegar pelo catálogo de blueprints disponíveis. </p> <p>Além disso, o administrador do sistema pode habilitar o acesso para que os usuários solicitem a instalação de blueprints. Atribuir uma fila de solicitações para armazenar as solicitações permite que os usuários façam solicitações no catálogo de blueprints. </p> </td> 
   <td> <p><b>Disponível nestas datas:</b> </p> 
    <ul> 
     <li> <p>Versão de pré-visualização: 10 de março de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2 </p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#add" class="MCXref xref" xrefformat="{para}">Adicionar uma imagem a um formulário personalizado</a> </p> <p>Em um formulário personalizado que você cria ou edita, agora é possível adicionar uma imagem e incluir uma dica de ferramenta informativa ou instrutiva que os usuários podem ler ao passar o mouse sobre ela.</p> <p>Isso pode ser útil, por exemplo, para mostrar a identidade visual de um novo produto ou para fornecer informações visuais que as pessoas precisam ao preencher o formulário.</p> <p>Anteriormente, os formulários personalizados eram completamente baseados em texto.</p> </td> 
   <td> <p><b>Disponível nestas datas:</b> </p> 
    <ul> 
     <li> <p>Versão de pré-visualização: 10 de março de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2 </p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#deactiva" class="MCXref xref" xrefformat="{para}">Desativar um grupo</a> </p> <p>À medida que suas organizações internas mudam, talvez seja necessário parar de usar determinados grupos no Workfront e criar novos. Para ajudar nisso, adicionamos a capacidade de desativar um grupo sem perder seus dados históricos. Para usuários regulares que não precisam vê-los, os grupos inativos são apagados dos campos de digitação antecipada de grupo.</p> <p>Você ainda pode encontrar e configurar opções, preferências e associações de objetos para grupos inativos que gerencia. E desativar um grupo não altera nada sobre os objetos aos quais o grupo está anexado.</p> <p>Anteriormente, não era possível desativar um grupo.</p> </td> 
   <td> <p><b>Disponível nestas datas:</b> </p> 
    <ul> 
     <li> <p>Versão de pré-visualização: 10 de março de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2 </p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Novas configurações de nível de acesso padrão</a> </p> <p>Para atender melhor às necessidades da maioria dos administradores que criam níveis de acesso, alteramos a configuração padrão de várias opções de "Ajustar suas configurações" exibidas ao clicar no ícone de engrenagem em um botão Editar.</p> <p>As opções, anteriormente ativadas por padrão, agora estão desativadas. Se isso não atender às necessidades de sua organização, você poderá habilitá-los ao configurar um novo nível de acesso, ou posteriormente.</p> </td> 
   <td> <p><b>Disponível nestas datas:</b> </p> 
    <ul> 
     <li> <p>Versão de pré-visualização: 27 de janeiro de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2 </p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
     <li> <p>O Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic será descontinuado em março de 2022</a>, seguido em breve pela data de término da vida útil do Workfront Classic em julho de 2022.)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#blueprin2" class="MCXref xref" xrefformat="{para}">Aprimoramentos no histórico de instalação de blueprints</a> </p> <p>Ao instalar um blueprint, uma mensagem agora exibe os objetos específicos (como funções, equipes ou grupos) que foram instalados com êxito com o blueprint e quaisquer objetos que falharam na instalação. Você também pode exibir a lista de objetos instalados na página Detalhes do blueprint clicando em Exibir detalhes ao lado de uma instalação específica na tabela de histórico de instalação.</p> </td> 
   <td> <p><b>Disponível nestas datas:</b> </p> 
    <ul> 
     <li> <p>Versão de pré-visualização: 10 de fevereiro de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2 </p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#a" class="MCXref xref" xrefformat="{para}">Um aviso agora é exibido ao instalar um blueprint somente para visualização na Produção</a> </p> <p>Determinados blueprints só estão disponíveis para instalação no ambiente de Pré-visualização para fins de teste.</p> <p>Se você acessar somente o conteúdo de Visualização no seu ambiente de Produção, Sandbox 1 ou Sandbox 2, o botão Instalar não estará ativo e você poderá ver uma mensagem de aviso.</p> </td> 
   <td><b>Disponível nestas datas:</b> 
    <ul> 
     <li> <p>Versão de pré-visualização: 10 de fevereiro de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2 </p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Aprimoramentos do projeto {#project-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Recurso</strong> </p> </td> 
   <td> <p><strong>Datas e ambientes de lançamento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#adobe" class="MCXref xref" xrefformat="{para}">Os painéis do Adobe Workfront já estão disponíveis! </a> </p> <p>Quadros são ferramentas flexíveis que permitem a colaboração em equipe, fornecendo acesso a um quadro compartilhado contendo colunas e cartões. </p> <p>Usando quadros, você pode configurar rapidamente um quadro de tarefas com várias colunas, configurar colunas para mostrar um status ou categoria, adicionar outros usuários ao quadro e atribuí-los a cartões e muito mais.</p> </td> 
   <td> <p><b>Disponível nestas datas:</b> </p> 
    <ul> 
     <li> <p>Versão de pré-visualização: 10 de março de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2 </p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#addition" class="MCXref xref" xrefformat="{para}">Melhorias adicionais nas placas Workfront</a></p> <p>As seguintes melhorias adicionais estão disponíveis para as placas Workfront:</p> 
    <ul> 
     <li> <p>Cartões de tag em quadros</p> </li> 
     <li> <p>Mover cartões</p> </li> 
     <li> <p>Copiar cartões</p> </li> 
     <li> <p>Pesquisar em painéis</p> </li> 
     <li> <p>Definir uma data de vencimento para um cartão em Quadros</p> </li> 
    </ul> </td> 
   <td><b>Disponível nestas datas:</b> 
    <ul> 
     <li> <p>Versão de pré-visualização: 24 de março de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2 </p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#undo" class="MCXref xref" xrefformat="{para}">Opção Desfazer para atualizar postagens</a> </p> <p>Agora é mais fácil detectar erros ao postar uma atualização. Finalizar um comentário na guia Atualizar de um objeto agora cria uma janela pop-up por 7 segundos que permite cancelar a publicação e retornar à edição, antes que o sistema carimbe o comentário ou envie emails e notificações no aplicativo. Se você fechar a janela pop-up, sair da página ou esperar 7 segundos pelo tempo limite da janela, a publicação será feita normalmente.</p> </td> 
   <td> <p><b>Disponível nestas datas:</b> </p> 
    <ul> 
     <li> <p>Versão de pré-visualização: 10 de março de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2 </p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nova experiência ao copiar um projeto</a> </p> <p>Para tornar seu uso do Workfront consistente com a nova experiência do Adobe Workfront, reprojetamos a interface para copiar projetos. Isso está disponível ao copiar um projeto da página do projeto ou ao copiar um projeto de uma lista ou relatório. Antes desta atualização, você só podia copiar um projeto da página do projeto.</p> </td> 
   <td> <p><b>Disponível nestas datas:</b> </p> 
    <ul> 
     <li> <p>Versão de pré-visualização: 10 de março de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2 </p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#ability" class="MCXref xref" xrefformat="{para}">Capacidade de gerenciar projetos de listas e relatórios em um novo menu Mais</a> </p> <p>Adicionamos um novo menu Mais em listas e relatórios de projeto para permitir que você execute as seguintes ações dessas áreas:</p> 
    <ul> 
     <li> <p>Para vários projetos de uma vez:</p> </li> 
     <li> <p>Recalcular Linha de Tempo</p> </li> 
     <li> <p>Recalcular Finanças</p> </li> 
     <li> <p>Recalcular Expressões Personalizadas</p> </li> 
     <li> <p>Para um único projeto:</p> </li> 
     <li> <p>Vincular Modelo</p> </li> 
     <li> <p>Exportar para o MS Project</p> </li> 
     <li> <p>Assinar</p> </li> 
    </ul> </td> 
   <td> <p><b>Disponível nestas datas:</b> </p> 
    <ul> 
     <li> <p>Versão de pré-visualização: 10 de março de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2 </p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">Nova experiência ao converter um problema em um projeto usando um modelo no nível do problema</a> </p> <p>Para tornar seu uso do Workfront consistente com a nova experiência do Workfront, reprojetamos a interface para converter um problema em um projeto ao usar um modelo ao convertê-lo da página de problema.</p> <p>Agora é possível acessar com mais facilidade sua lista de favoritos imediatamente após selecionar para converter o problema.</p> <p>A interface reprojetada corresponde à experiência ao criar um projeto a partir de um modelo que também atualizamos recentemente.</p> </td> 
   <td><strong>Disponível nestas datas:</strong> 
    <ul> 
     <li> <p>Versão de pré-visualização: 8 de dezembro de 2021<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.1 do <span style="color: #ff0000; font-weight: bold;">Esse recurso foi removido temporariamente do ambiente de produção do em 4 de março de 2022. Mais tarde, foi lançado em uma implantação em fases a partir de 28 de abril de 2022. A implantação foi concluída em 5 de maio de 2022. Isso agora está disponível em Pré-visualização e Produção para todos os clientes.</span></p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#convert" class="MCXref xref" xrefformat="{para}">Converter problemas em projetos usando um modelo de listas, relatórios e painéis</a> </p> <p>Para aumentar a eficiência do seu trabalho e facilitar a conversão de problemas em um ambiente de ritmo rápido, adicionamos a capacidade de converter um problema em um projeto usando um modelo de uma lista, relatório ou painel.</p> <p>Antes desse aprimoramento, essa funcionalidade existia somente quando você convertia o problema da página de problemas.</p> </td> 
   <td><strong>Disponível nestas datas:</strong> 
    <ul> 
     <li> <p>Versão de pré-visualização: 8 de dezembro de 2021<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.1 do <span style="color: #ff0000; font-weight: bold;">Esse recurso foi removido temporariamente do ambiente de produção do em 4 de março de 2022. Mais tarde, foi lançado em uma implantação em fases a partir de 28 de abril de 2022. A implantação foi concluída em 5 de maio de 2022. Isso agora está disponível em Pré-visualização e Produção para todos os clientes.</span></p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#updated" class="MCXref xref" xrefformat="{para}">Experiência atualizada ao copiar e mover problemas</a> </p> <p>Para tornar seu uso do Workfront consistente com a nova experiência do Adobe Workfront, reprojetamos a interface para copiar e mover problemas. Isso está disponível ao copiar ou mover um único problema ou ao copiar ou mover problemas em massa de uma lista ou relatório.</p> </td> 
   <td><strong>Disponível nestas datas:</strong> 
    <ul> 
     <li> <p>Versão de pré-visualização: 18 de fevereiro de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2</p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#keep" class="MCXref xref" xrefformat="{para}">Manter usuários no painel, lista ou relatório após converter o problema em projeto</a> </p> <p>Para aumentar a eficiência e eliminar o número de cliques, lançamos uma melhoria ao converter problemas em projetos de uma lista, relatório ou painel.</p> <p>Os usuários permanecem na lista, relatório ou painel após converterem um problema em um projeto, em vez de serem redirecionados para a página do projeto. Uma notificação de sucesso com o link para o projeto é exibida após a conclusão da conversão, para permitir que você navegue facilmente até o projeto, se necessário. </p> </td> 
   <td><strong>Disponível nestas datas:</strong> 
    <ul> 
     <li> <p>Versão de pré-visualização: 10 de fevereiro de 2022<br></p> </li> 
     <li> <p>Versão de produção: 24 de fevereiro de 2022</p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#allocati" class="MCXref xref" xrefformat="{para}">As horas de alocação não serão mais removidas quando forem feitas alterações nas atribuições</a> </p> <p>Para garantir a precisão de seus dados, fizemos uma alteração para preservar as horas de alocação e manter as Horas planejadas da tarefa inalteradas ao fazer alterações em atribuições na tarefa.</p> <p>As seguintes alterações foram feitas em tarefas com um Tipo de Duração Simples:</p> 
    <ul> 
     <li> <p>As alocações de atribuição individuais são preservadas ao substituir usuários e funções.</p> </li> 
     <li> <p>As alocações de atribuição individuais são preservadas na função ao remover o usuário.</p> </li> 
     <li> <p>As horas planejadas são preservadas ao remover todos os atribuídos. <span style="color: #ff0000;">(Removido da versão. Agora, o Trabalho necessário será definido como 0 após a remoção de todos os atribuídos.)</span></p> </li> 
    </ul> </td> 
   <td><strong>Disponível nestas datas:</strong> 
    <ul> 
     <li> <p>Versão de pré-visualização: 10 de fevereiro de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2 <span style="color: #ff0000; font-weight: bold;">Esse recurso será lançado para produção logo após a versão 22.2</span></p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
     <li> <p>O Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic será descontinuado em março de 2022</a>, seguido em breve pela data de término da vida útil do Workfront Classic em julho de 2022.)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#share" class="MCXref xref" xrefformat="{para}">Compartilhar pastas somente nos cinco níveis superiores de uma hierarquia de pastas</a> </p> <p>Para garantir o melhor desempenho para usuários que compartilham pastas, estamos limitando o compartilhamento aos cinco principais níveis em uma hierarquia de pastas em um objeto.</p> <p>Cada pasta no sexto nível ou abaixo herda suas configurações de compartilhamento da pasta diretamente acima dela.</p> </td> 
   <td><strong>Disponível nestas datas:</strong> 
    <ul> 
     <li> <p>Versão de pré-visualização: 10 de fevereiro de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2 <span style="color: #ff0000; font-weight: bold;">Este recurso está temporariamente indisponível. Esta página será atualizada quando o recurso estiver disponível na Produção.</span></p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
     <li> <p>O Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic será descontinuado em março de 2022</a>, seguido em breve pela data de término da vida útil do Workfront Classic em julho de 2022.)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Melhorias no gerenciamento de recursos {#resource-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Recurso</strong> </p> </td> 
   <td> <p><strong>Datas e ambientes de lançamento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-resource-management-enhancements.md#improvem" class="MCXref xref" xrefformat="{para}">Melhorias na navegação do Balanceador de carga de trabalho</a> </p> <p>Para melhorar sua experiência ao usar o Balanceador de carga de trabalho, introduzimos os seguintes aprimoramentos:</p> 
    <ul> 
     <li> <p>Os botões Cancelar e Salvar ao ajustar alocações agora são fixos, mesmo quando a tarefa é mais longa do que o período incluído na tela ou quando o painel Resumo é exibido.</p> </li> 
     <li> <p>O painel esquerdo que exibe os nomes de usuários e itens de trabalho agora é fixo, para permitir rolar horizontalmente por períodos mais longos e ainda poder ler os nomes dos itens listados no painel.</p> </li> 
     <li> <p>Você pode recolher e expandir todos os itens listados no painel esquerdo com um clique em vez de no nível do usuário ou do projeto.</p> </li> 
     <li> <p>Agora, o painel esquerdo também pode ser redimensionado.</p> </li> 
     <li> <p>Agora há um modo de tela cheia para o Balanceador de carga de trabalho.</p> </li> 
    </ul> </td> 
   <td> <p><b>Disponível nestas datas:</b> </p> 
    <ul> 
     <li> <p>Versão de pré-visualização: 10 de março de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2 </p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-resource-management-enhancements.md#access" class="MCXref xref" xrefformat="{para}">Acessar atribuições avançadas no Balanceador de carga de trabalho</a> </p> <p>Para tornar a atribuição de itens de trabalho mais fácil e precisa, agora é possível fazer atribuições avançadas ao atribuir itens de trabalho manualmente no Balanceador de carga de trabalho. Antes desse aprimoramento, você poderia acessar as Atribuições avançadas ao editar itens, nos cabeçalhos dos itens ou em listas.</p> </td> 
   <td> <p><b>Disponível nestas datas:</b> </p> 
    <ul> 
     <li> <p>Versão de pré-visualização: 10 de março de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2 </p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-resource-management-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nova fórmula para calcular a disponibilidade do usuário quando a preferência Agendamento padrão está selecionada</a> </p> <p>Para fornecer informações mais precisas nas ferramentas de gerenciamento de recursos, alteramos a fórmula usada pelo Workfront para calcular a disponibilidade dos usuários quando o administrador do Workfront seleciona A programação padrão nas Preferências de gerenciamento de recursos. Com a nova atualização, o Workfront usa a seguinte fórmula para calcular a disponibilidade do usuário:</p> <p>Horas Disponíveis do Usuário = (Horas Programadas Padrão - Exceções) * FTE - Horas de folga</p> <p>Antes dessa atualização, o Workfront usava a seguinte fórmula para calcular a disponibilidade do usuário quando o Agendamento padrão era selecionado:</p> <p>Horas Disponíveis do Usuário = (Horas Programadas Padrão - (Exceções Programadas + Horas de folga)) * Valor FTE do Usuário</p> </td> 
   <td> <p><b>Disponível nestas datas:</b> </p> 
    <ul> 
     <li> <p>Versão de pré-visualização: 10 de março de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2 </p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
     <li> <p>O Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic será descontinuado em março de 2022</a>, seguido em breve pela data de término da vida útil do Workfront Classic em julho de 2022.)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Aprimoramentos na página inicial {#home-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Recurso</strong> </p> </td> 
   <td> <p><strong>Datas e ambientes de lançamento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-home-enhancements.md#improvem" class="MCXref xref" xrefformat="{para}">Melhorias nos filtros na Lista de trabalho da página inicial</a> </p> <p>Para dar mais controle e foco sobre sua lista de trabalho, implementamos várias melhorias nos filtros na área da Página inicial. Com as novas melhorias, você pode selecionar filtros por tipo de objeto e restringir ainda mais seus resultados pelo estado dos itens de trabalho (por exemplo, Pronto para iniciar, Trabalhando em ou Solicitado). Os novos Filtros da página inicial agora fornecem uma contagem correta de tarefas, problemas, itens de trabalho pessoais e aprovações ao aplicar uma combinação de filtros de tipo de objeto e estado do item de trabalho.</p> <p>Antes dessa experiência, os filtros na área da Página inicial não forneciam uma contagem precisa do número de itens de trabalho na lista quando você selecionava um ou mais filtros e eles criavam confusão sobre o estado dos itens de trabalho.</p> </td> 
   <td> <p><b>Disponível nestas datas:</b> </p> 
    <ul> 
     <li> <p>Versão de pré-visualização: 10 de março de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2 </p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Melhorias na mobilidade {#mobile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Recurso</strong> </p> </td> 
   <td> <p><strong>Datas e ambientes de lançamento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-mobile-enhancements.md#drawings" class="MCXref xref" xrefformat="{para}">Desenhos e comentários nos documentos de prova no aplicativo móvel</a></p> <p>O aplicativo móvel do Adobe Workfront agora permite adicionar desenhos e comentários em documentos de prova. Uma nova barra de ferramentas na prova contém ferramentas de desenho para formas. É possível escolher configurações como cor e espessura da linha para cada forma. Desenhar uma forma na prova conecta seu comentário a essa área do documento de prova.</p> <p>Você também pode responder aos comentários que outras pessoas fizeram sobre a prova.</p> </td> 
   <td><strong>Disponível nestas datas:</strong> 
    <ul> 
     <li> <p>Versão de pré-visualização: N/D<br></p> </li> 
     <li> <p>Versão de produção: meados a final de abril de 2022 </p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>aplicativo móvel iOS</p> </li> 
     <li> <p>aplicativo móvel Android</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-mobile-enhancements.md#enhancem" class="MCXref xref" xrefformat="{para}">Aprimoramentos na funcionalidade de prova no aplicativo móvel</a> </p> <p>No aplicativo móvel do Adobe Workfront, agora é possível:</p> 
    <ul> 
     <li> <p>Compartilhar provas com recipients internos e externos</p> </li> 
     <li> <p>Exibir comentários de prova</p> </li> 
     <li> <p>Baixar provas</p> </li> 
    </ul> </td> 
   <td><strong>Disponível nestas datas:</strong> 
    <ul> 
     <li> <p>Versão de pré-visualização: N/D<br></p> </li> 
     <li> <p>Versão de produção: início de fevereiro de 2022 (essas melhorias foram originalmente comunicadas com a versão 22.1).</p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>aplicativo móvel iOS</p> </li> 
     <li> <p>aplicativo móvel Android</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Melhorias nas integrações {#integrations-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Recurso</strong> </p> </td> 
   <td> <p><strong>Datas e ambientes de lançamento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#adobe" class="MCXref xref" xrefformat="{para}">O Adobe Workfront com integração Anaplan está disponível agora</a> </p> <p>Para oferecer mais flexibilidade e insight sobre os aspectos financeiros dos projetos da Workfront, a Workfront agora pode se integrar à sua conta Anaplan. Ao vincular objetos Workfront a objetos Anaplan, você pode atualizar informações entre as duas contas automaticamente, garantindo que as informações em ambas estejam atualizadas e idênticas. </p> <p>Você também pode acionar processos automatizados no Anaplan com base em ações no Workfront (ou vice-versa).</p> <p>Por exemplo, você pode criar uma campanha no Anaplan e, em seguida, criar um projeto ou programa do Workfront vinculado à campanha. Quaisquer custos rastreados no Workfront podem ser enviados de volta ao Anaplan para analisar o desempenho da campanha.</p> </td> 
   <td><strong>Disponível nestas datas:</strong> 
    <ul> 
     <li> <p>Versão de pré-visualização: 10 de março de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2</p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Workfront para atualizações avançadas de conector do Experience Manager</a> </p> <p>O conector aprimorado do Workfront para Experience Manager agora inclui as seguintes atualizações:</p> 
    <ul> 
     <li> <p>Agora é possível criar pastas vinculadas entre o Adobe Workfront e o Adobe Experience Manager Assets as a Cloud Service, mesmo se houver várias configurações de pastas vinculadas do projeto.</p> </li> 
     <li> <p>Adição de suporte para paginação de subscrição de evento.</p> </li> 
     <li> <p>Adição de suporte para AEM 6.4.x</p> </li> 
     <li> <p>Adição de suporte para ambientes proxy</p> </li> 
     <li> <p>Várias correções de bugs com base no feedback do parceiro e do cliente</p> </li> 
    </ul> </td> 
   <td><strong>Disponível nestas datas:</strong> 
    <ul> 
     <li> <p>Versão de pré-visualização: N/D<br></p> </li> 
     <li> <p>Versão de produção: 28 de março de 2022</p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#see" class="MCXref xref" xrefformat="{para}">Veja detalhes do Segredo do Cliente para integrações OAuth2 ou JWT personalizadas</a> </p> <p>Para fornecer transparência no uso das integrações OAuth2 e JWT personalizadas, possibilitamos que você veja detalhes dos Segredos do cliente que suas integrações usam. Agora você pode ver as datas em que o Segredo do cliente foi criado e usado pela última vez. Você também pode adicionar e exibir suas próprias observações sobre o Segredo do cliente.</p> <p>Anteriormente, esses detalhes estavam indisponíveis.</p> </td> 
   <td><strong>Disponível nestas datas:</strong> 
    <ul> 
     <li> <p>Versão de pré-visualização: 3 de março de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2</p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#adobe2" class="MCXref xref" xrefformat="{para}">As integrações do Adobe Creative Cloud agora usam OAuth2</a> </p> <p>Para maior segurança e para tornar uma experiência mais consistente em todas as integrações, atualizamos as integrações do Adobe Creative Cloud para usar a autenticação OAuth2, uma maneira padrão do setor para autenticar usuários. Agora, quando os usuários fizerem logon, eles poderão ver as ações e áreas específicas às quais as integrações têm acesso e permitir acesso. Depois disso, eles não precisarão fazer logon com a mesma frequência.</p> </td> 
   <td><strong>Disponível nestas datas:</strong> 
    <ul> 
     <li> <p>Versão de pré-visualização: 24 de fevereiro de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2</p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#see2" class="MCXref xref" xrefformat="{para}">Consulte o tipo de autenticação na lista de aplicativos OAuth2 personalizados</a> </p> <p>Agora, ao visualizar a lista de aplicativos OAuth2 personalizados em sua organização, você pode ver se cada aplicativo usa autenticação de usuário ou autenticação de servidor.</p> <p>Anteriormente, só era possível ver essas informações acessando as opções de edição em cada aplicativo.</p> </td> 
   <td><strong>Disponível nestas datas:</strong> 
    <ul> 
     <li> <p>Versão de pré-visualização: 17 de fevereiro de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2</p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#set" class="MCXref xref" xrefformat="{para}">Defina a expiração para atualizar tokens em suas integrações OAuth2 personalizadas</a> </p> <p>Para controlar melhor o acesso e a segurança de suas integrações OAuth2 personalizadas, agora é possível personalizar a duração de tokens de atualização. Depois que um token de atualização do usuário expirar, será necessário fazer logon na integração novamente.</p> </td> 
   <td> <p><b>Disponível nestas datas:</b> </p> 
    <ul> 
     <li> <p>Versão de pré-visualização: 10 de fevereiro de 2022 <br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2 </p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#use" class="MCXref xref" xrefformat="{para}">Use chaves públicas e privadas em suas integrações OAuth2 personalizadas para aplicativos de servidor para servidor</a> </p> <p>Agora é possível configurar aplicativos OAuth2 de servidor para servidor em suas integrações personalizadas. Ao configurar chaves públicas e privadas, você pode permitir que o Workfront se comunique com outro aplicativo sem usar credenciais de logon.</p> <p>Anteriormente, todas as autenticações nos aplicativos OAuth2 personalizados usavam as credenciais de logon do usuário.</p> </td> 
   <td> <p><b>Disponível nestas datas:</b> </p> 
    <ul> 
     <li> <p>Versão de pré-visualização: 10 de fevereiro de 2022 <br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2 </p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Outras melhorias {#other-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Recurso</strong> </p> </td> 
   <td> <p><strong>Datas e ambientes de lançamento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-look-and-feel-updates.md#enhancem" class="MCXref xref" xrefformat="{para}">Atualizações de aparência durante o período da versão 22.2</a> </p> <p>Pequenas atualizações na aparência de várias áreas do aplicativo Adobe Workfront estão sendo feitas dentro do período da versão 22.2. Essas melhorias serão disponibilizadas no ambiente de Produção no mínimo 2 semanas após o lançamento para Pré-visualização. </p> </td> 
   <td><strong>Disponível nestas datas:</strong> 
    <ul> 
     <li> <p>Versão de pré-visualização: ao longo do período da versão 22.2<br></p> </li> 
     <li> <p>Versão de produção: um mínimo de 2 semanas após o lançamento para pré-visualização</p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-other-enhancements.md#enhancem" class="MCXref xref" xrefformat="{para}">Melhorias na barra de navegação superior</a> </p> <p>Fizemos várias melhorias na barra de navegação superior do Adobe Workfront.</p> 
    <ul> 
     <li> <p>Favoritos e Recentes agora têm ícones separados na barra de navegação superior. Cada página ainda exibe o mesmo conteúdo (páginas marcadas como favoritas e páginas visitadas recentemente), e você pode continuar a adicionar e remover páginas favoritas da mesma maneira.</p> </li> 
     <li> <p>A aparência dos pinos e do menu principal foi atualizada para os padrões de design de Adobe, incluindo cores e fontes. A maneira de adicionar e remover pinos e as áreas às quais você tem acesso no menu principal não foram alteradas.</p> </li> 
     <li> <p>Os ícones à direita da barra de navegação superior foram reordenados para serem mais intuitivos. A ordem dos ícones é: link de ajuda, notificações, favoritos, recentes, pesquisa, menu principal.</p> </li> 
    </ul> </td> 
   <td><strong>Disponível nestas datas:</strong> 
    <ul> 
     <li> <p>Versão de pré-visualização: 10 de março de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2</p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-other-enhancements.md#redesign" class="MCXref xref" xrefformat="{para}">Listas de planilhas de horas reprojetadas</a> </p> <p>Para tornar seu uso do Workfront consistente com a nova experiência do Adobe Workfront, reprojetamos as listas de folhas de horas na área Folhas de horas. Você pode esperar a mesma funcionalidade na lista de folha de horas, apenas com uma experiência do usuário mais limpa e simplificada.</p> <p>Alguns dos destaques desse novo design são:</p> 
    <ul> 
     <li> <p>A lista Folha de horas agora corresponde à experiência em todas as outras listas no Workfront.</p> </li> 
     <li> <p>A experiência de filtro agora corresponde aos filtros em todas as outras listas. Você terá mais flexibilidade para criar seus próprios filtros com os campos e atributos que mais fazem sentido para você, bem como compartilhá-los com outros usuários.</p> </li> 
    </ul> </td> 
   <td><strong>Disponível nestas datas:</strong> 
    <ul> 
     <li> <p>Versão de pré-visualização: 10 de março de 2022<br></p> </li> 
     <li> <p>Versão de produção: com a versão 22.2</p> </li> 
    </ul> <p><strong>Disponível nestes ambientes:</strong> </p> 
    <ul> 
     <li> <p>A nova experiência do Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Aprimoramentos do Workfront Fusion

Novos recursos no Workfront Fusion estão disponíveis na Produção em uma cadência fora da programação de lançamento 22.2. Para obter mais informações sobre os recursos mais recentes, consulte [atividade de versão do Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

## Aprimoramentos no Planejador de cenários do Workfront

Não há atualizações do Planejador de cenários neste momento na versão. Esta área será atualizada quando houver atualizações disponíveis.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features are coming to Workfront Scenario Planner release with the 21.4 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-activity.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront Scenario Planner release activity</a>.</p>
-->

## Aprimoramentos do Workfront Proof

Não há atualizações do Workfront Proof neste momento na versão. Esta área será atualizada quando houver atualizações disponíveis.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features in Workfront Proof are now available. For more information, see <a href="../../../product-announcements/product-releases/workfront-proof-release-activity/wp-release-22-1.md" class="MCXref xref" xrefformat="{para}">Workfront Proof release activity:&nbsp;Week of November 29, 2021</a>.</p>
-->

## Aprimoramentos das metas do Workfront

Não há atualizações do Workfront Goals neste momento na versão. Esta área será atualizada quando houver atualizações disponíveis.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Most new features coming to Workfront Goals release with the 21.2 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/goals-release-activity/goals-21.2-release/goals-release-21-2.md" class="MCXref xref" xrefformat="{para}" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Adobe Workfront Goals with the 21.2 release</a>.</p>
-->

## API versão 14

Para a API versão 14, modificamos alguns recursos e endpoints. Algumas das alterações são compatíveis com a nova funcionalidade, enquanto outras facilitam o uso das informações disponíveis por meio da API.

Para obter informações sobre novidades e atualizações, consulte [Novidades na API versão 14](../../../wf-api/api/new-api-version-14.md).

Para obter informações sobre versões de API, consulte [Controle de versão de API e agendamento de suporte](../../../wf-api/api/api-version-support-schedule.md).

## Atualizações de manutenção do Workfront 

Para obter informações sobre as atualizações de manutenção feitas durante a versão 22.2, consulte [Atualizações de manutenção do Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

## Webinário da versão 22.2

O webinário da versão 22.2 do Workfront será apresentado em 24 de março de 2022 às 8h MST. Você pode se inscrever para o evento na [página Eventos no Workfront One](https://webinars.on24.com/adobe_workfront/WF22point2?partnerref=WFOne).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This area will be updated as more information becomes available.
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
was presented on January 12, 2022. You can view the webinar recording on the
<a href="https://one.workfront.com/s/event">Events page on Workfront One</a>.
</MadCap:conditionalText>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Functionality being removed from Production</h2>
<h3>Feature rollback: Carry over the existing proof workflow when generating a new version</h3>
<p>Due to customer feedback, <b>Workfront is removing this change from Preview environments on March 30, 2021 and from Production environments on March 31, 2021</b>.</p>
<p>On March 11, 2021, Workfront released a change to existing proof workflows in both Workfront Classic and the new Workfront experience. The change allowed for an existing workflow to carry over to any new proof versions created by a user, regardless of the method used to generate them.</p>
<p>In the new Workfront experience after this change is removed, proofs created with the Simple proof selection will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>In Workfront Classic after this change is removed, the option to Generate Proof will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>Similar functionality to easily copy existing workflows might be added to Production at a future time.</p>
</div>
-->

## Atualizações de treinamento

Explore as atualizações mais recentes feitas em programas de aprendizado, caminhos de aprendizado, vídeos e guias para cada versão de produto do Adobe Workfront. Para obter mais informações, consulte a [página de atualizações da versão de treinamento](https://one.workfront.com/s/training-release-updates).

## Funcionalidade não mais compatível

### Internet Explorer 11

Com a remoção do suporte ao Internet Explorer, a Workfront agora oferece suporte oficial ao Microsoft Edge.

Para obter mais informações sobre navegadores compatíveis, consulte [requisitos do navegador Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md).
