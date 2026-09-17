---
title: Visão Geral do Adobe Workfront Planning CX Coworker
description: Você pode usar o CX Coworker no Workfront Planning para executar ações semelhantes a registros e outros objetos no Planning que normalmente seriam executados na interface. Os comandos do usuário e a execução desses comandos pela IA trabalham juntos para garantir que as alterações feitas pela IA sejam refletidas com precisão no ambiente.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: b529b3aded4ab92015683a0ddccd152bc2cc798c
workflow-type: tm+mt
source-wordcount: '1119'
ht-degree: 3%
---

# Visão geral do Adobe Workfront Planning CX Coworker

<!--replaced information from the AI Assistant for Planning article with CX Coworker-->

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Após o lançamento para Pré-visualização, os mesmos recursos também estarão disponíveis mensalmente no ambiente de Produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

O CX Coworker é uma interface conversacional em que você descreve uma meta em linguagem simples e, em seguida, planeja, executa e valida o trabalho no Workfront Planning e em outros sistemas Adobe conectados antes de trazê-lo de volta para sua aprovação.

O CX Coworker preserva tudo o que o AI Assistant faz hoje e, ao mesmo tempo, adiciona recursos completos mais avançados em uma nova experiência de tela cheia e no painel direito do Workfront.

Ela opera nos controles de acesso de nível de produto existentes em sua organização, de modo que os usuários só podem realizar ações para as quais já têm permissão no Workfront, com acesso somente leitura por padrão e acesso de gravação controlado por administradores do Workfront.

>[!IMPORTANT]
>
>Atualmente, o CX Coworker não está disponível para organizações de assistência médica, finanças ou alguns outros setores com dados confidenciais. O Assistente de IA está disponível para essas organizações.
>
>Para obter mais informações, consulte [Visão geral do Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacotes Adobe Workfront</p></td> 
   <td> 
<p>Qualquer Workfront ou Fluxo de trabalho com um pacote do Planning</p>
Ou
<p>Qualquer pacote do Planning quando adquirido como um produto independente</p>
   </td> </tr>
 <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Padrão</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>licença do Adobe Planning</p></td> 
   <td><p>Padrão</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td>  
   <p>O administrador deve fazer o seguinte para permitir o acesso ao CX Coworker no Planning:</p>
   <ul>
   <li><p>Adicione um Workflow e um tipo de licença do Planning ao seu nível de acesso quando você tiver um Workflow e um pacote do Planning</p></li>
   <li><p>Desmarque Desativar o painel CX Coworker na configuração do Workfront no seu nível de acesso. Ela é selecionada por padrão.</p></li></ul>
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Configurações do sistema</p></td> 
   <td>   <p>O administrador do Workfront deve selecionar as ferramentas MCP somente leitura e somente gravação na área Preferências do sistema da Configuração. As ferramentas de MCP somente leitura são selecionadas por padrão.</p> 
    </td> 
  </tr> 
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações para a CX Coworker

* A CX Coworker deve estar ativada para sua organização antes de estar disponível para os usuários em sua empresa.

  Para obter informações, consulte [visão geral do CX Coworker](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

* Depois que a Workfront ativar o agente para sua instância do Workfront, ele estará disponível para o administrador principal do Workfront e poderá ser ativado para sua organização. Para obter informações, consulte [Configurar preferências do sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

* O administrador do Workfront também deve ativar o CX Coworker para você, no seu nível de acesso. Para obter informações, consulte [Criar e modificar níveis de acesso](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* O CX Coworker funciona com informações e objetos que estão no Workfront ou no Workfront Planning e que você tem permissão para acessar. No painel direito do Planning, o painel Colaborador opera no contexto do espaço de trabalho, tipo de registro ou página de registro que você abriu.

* As ações executadas pela CX Coworker na área Planejamento se encontram no contexto das suas permissões do Workfront Planning e do seu nível de acesso ao Workfront. Para obter informações, consulte os seguintes artigos:

  * [Visão geral das permissões de compartilhamento no Planejamento do Adobe Workfront](/help/quicksilver/planning/access/sharing-permissions-overview.md)
  * [Visão geral dos tipos de licença ao usar o Planejamento do Adobe Workfront](/help/quicksilver/planning/access/license-type-overview.md)

* As alterações feitas pela CX Coworker em nome do usuário são rastreadas no painel de histórico do registro.

* As ações realizadas pela CX Coworker são permanentes e podem ser irreversíveis. Por exemplo, a exclusão de um campo não pode ser revertida. Revise todas as ações propostas pela CX Coworker antes de aceitá-las.

* Ao criar, atualizar ou excluir um objeto por meio da CX Coworker, o CX Coworker exibe as ações desejadas e solicita a confirmação. Você pode confirmar ou cancelar as ações.

## Funcionalidade atualmente disponível para o CX Coworker

Atualmente, o CX Coworker está disponível na área Planejamento do Workfront e usa um conjunto de habilidades para acessar e manipular informações para objetos do Planejamento. Para obter mais informações, consulte [habilidades do CX Coworker](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-skills.md).

Você pode usar o CX Coworker para executar as seguintes ações:

* Pesquisar registros. Você pode pesquisar pelas informações contidas em qualquer campo de registro.
* Criar registros. Uma ID com um link para o novo registro é exibida após a criação do registro. Você pode especificar os campos que deseja atualizar durante o processo de criação, como datas ou descrição.
* Crie registros com base em um documento do qual você fez upload. O Workfront é compatível com os seguintes formatos de documento para o CX Coworker:

  PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT e a maioria dos formatos de imagem
* Atualize os campos dos registros exibidos na tela
* Excluir, duplicar ou restaurar registros
* Vincular registros a outros registros
* Exibir histórico de alterações de um registro


## Localize a CX Coworker no Workfront Planning

Você pode localizar o CX Coworker nas seguintes áreas do Workfront Planning:

* A barra de navegação principal, no canto superior direito da tela.
* Dentro da área de detalhes de um registro ao abri-lo em uma nova guia.

## Acesse o CX Coworker na área Planejamento


1. Faça logon no Workfront, clique no ícone **Menu Principal** ![Menu principal Linhas](assets/lines-main-menu.png) no canto superior esquerdo e clique em **Planning**.

   A área Planejamento é aberta.

   Localize o **Ícone de IA** ![Ícone de IA](assets/ai-icon.png) no canto superior direito da página ou continue com as etapas abaixo.

1. Clique em um **cartão de espaço de trabalho**.

1. Clique em um **cartão de tipo de registro**.

1. Clique em um **registro** para abrir a página **Detalhes** do registro, em seguida, clique em abrir em .

1. Clique no **ícone do CX Coworker** no canto superior direito da tela.

1. No espaço fornecido, comece a digitar comandos para o CX Coworker e, em seguida, clique em Inserir quando terminar.

   ![Painel do CX Coworker com caixa de comando vazia](assets/cx-coworker-right-rail.png)

   Por exemplo, você pode digitar um dos seguintes:

   * Crie um novo registro de campanha chamado Vendas de verão 2026
   * Atualize o campo de orçamento no registro da Campanha de Verão para US$ 75.000
   * Exclua o registro de campanha chamado Promoção antiga
   * Restaurar a campanha que eu excluí acidentalmente

   >[!TIP]
   >
   >Certifique-se de que o administrador do Workfront ativou as Ferramentas MCP somente gravação nas Preferências do sistema antes de solicitar que o CX Coworker execute ações de edição em objetos.

   Um indicador visual é exibido enquanto o CX Coworker processa comandos, definindo expectativas para o tempo de resposta.

   Depois de receber uma resposta bem-sucedida, siga os links fornecidos ou observe as alterações à esquerda.


1. (Opcional) Clique no ícone **Expandir tela inteira** ![Expandir ícone tela inteira](assets/expand-full-screen-icon.png) para abrir a caixa de chat do Coworker em uma guia de navegador completo.


