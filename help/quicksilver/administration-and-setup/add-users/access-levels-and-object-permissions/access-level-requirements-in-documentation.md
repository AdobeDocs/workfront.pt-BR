---
title: Requisitos de acesso na documentação do Workfront
content-type: reference
product-area: system-administration
keywords: acesso,nível,sistema,administrador,planejador,trabalhador,revisor,solicitante,externo,usuário
navigation-topic: access-levels
description: Os artigos de instruções da documentação do Workfront contêm uma tabela que explica o acesso e as permissões necessárias para esse procedimento. Este artigo explica a tabela de requisitos de acesso com mais detalhes e contém links para obter mais informações.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 39ea0d53-ec31-4644-b772-cfe260b8e013
source-git-commit: 469242118429fa37835766737b88d35d2baefb69
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 0%

---

# Requisitos de acesso na documentação do Workfront

Os artigos de instruções da documentação do Workfront contêm uma tabela que explica os requisitos de acesso e permissões necessários para esse procedimento. Esta tabela de Requisitos de acesso permite compreender se você pode executar uma determinada ação no Workfront ou por que não pode fazê-lo. Este artigo explica cada elemento da tabela Requisitos de acesso e fornece dicas e links para a solução de problemas a informações mais detalhadas.

Se uma linha estiver ausente da tabela Requisitos de acesso em um determinado artigo, não há requisitos desse tipo para essa ação.

Algumas linhas contêm informações rotuladas como &quot;Novo&quot; e &quot;Atual&quot;. Isso ocorre porque a Workfront está fazendo a transição para um novo modelo de preços e pacotes, com algumas organizações operando sob o novo modelo e outras ainda usando o modelo atual. Para descobrir qual modelo sua organização usa, entre em contato com o administrador do Workfront. Você pode encontrar detalhes e links para informações na seção [Tabela de requisitos de acesso](#the-access-requirements-table) deste artigo.

>[!NOTE]
>
>Em caso de dúvidas sobre como qualquer um dos campos desta tabela se aplica a você, entre em contato com o administrador do Workfront.

## A tabela Requisitos de acesso

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> Os pacotes do Adobe Workfront se referem ao conjunto de recursos que sua organização adquiriu. A maioria das funcionalidades do Workfront está disponível em todos os pacotes, com algumas exceções, principalmente relacionadas ao planejamento estratégico e aos controles corporativos. <p>Os pacotes existentes antes de 2022 não são listados.</p>
   <p>Os pacotes do Workfront são divididos em três áreas. Cada área oferece pacotes diferentes, como Select, Prime e Ultimate.<p>
   <ul>
   <li><b>Fluxo de Trabalho do Workfront</b>: inclui funcionalidades relacionadas a operações, como gerenciamento de tarefas, aprovações e planilhas de horas.</li>
   <li><b>Workfront Planning</b>: inclui a funcionalidade relacionada ao planejamento estratégico.</li>
   <li><b>Automação e Integração do Workfront</b>: inclui funcionalidades relacionadas à automatização de processos e à integração com outros aplicativos.</li>
   </ul>
  <p>Sua organização pode ter comprado um pacote do Workfront em uma ou mais dessas áreas.</p>
  <p>Anteriormente, a Workfront oferecia os pacotes Workfront Select, Workfront Prime e Workfront Ultimate, sem distinguir entre Fluxo de trabalho, Planejamento e Automação e Integração. Sua organização pode estar em um desses pacotes herdados. 
   <ul><li>Para saber qual pacote do Adobe Workfront sua organização usa, incluindo se a organização está no modelo de pacote atual ou herdado, entre em contato com o administrador do Workfront.</li>
   <li>Para obter instruções sobre como um administrador do Workfront pode localizar o pacote Workfront da sua organização, consulte <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-package" class="MCXref xref">Exibir o cluster da sua organização e o pacote Workfront</a>.</li><li>Para obter mais informações sobre os pacotes do Workfront, consulte <a href="https://business.adobe.com/br/products/workfront/pricing.html">Preços e pacotes do Adobe Workfront</a>.</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> As licenças do Adobe Workfront se referem ao conjunto de recursos do Workfront incluídos na licença atribuída a você. Por exemplo, um usuário pode ter uma licença que inclui a marcação da conclusão dos itens de trabalho e o registro do tempo, enquanto outro usuário tem uma licença que permite apenas aprovar ativos ou enviar solicitações. <p> 
   <ul>
   <li>Para descobrir qual licença você está atribuído, entre em contato com o administrador do Workfront.</li>
   <li>Para obter informações sobre licenças, consulte:
   <ul>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Visão geral de novas licenças</a></li>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Visão geral de licenças</a></li></ul></li>
   <li>Se você tiver o nível de acesso correto e ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-package" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.
   </ul>
      </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td><p>Como o Workfront funciona em conjunto com outros produtos da Adobe, alguns procedimentos no Workfront interagem diretamente com esses produtos. Para seguir esses procedimentos, sua organização deve ter adquirido esse produto. Por exemplo, para usar uma funcionalidade que permita ao Workfront interagir com o Adobe Experience Manager Assets, sua organização deve ter comprado o Adobe Experience Manager Assets.</p>
   <p>Os artigos que descrevem procedimentos executados com produtos adicionais listam o produto necessário na linha de produtos desta tabela.</p>
   <p>Para saber se sua organização adquiriu um desses produtos adicionais, entre em contato com o administrador do Workfront.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso</td> 
   <td> Os níveis de acesso são conjuntos de permissões para ações que podem ser executadas no Workfront, definidos pelo administrador do Workfront. <p>A Workfront tem níveis de acesso incorporados que correspondem às licenças da Workfront, mas o administrador do Workfront pode criar mais níveis de acesso para refletir com mais precisão os conjuntos de permissões necessários em sua organização.</p>
   <ul>
    <li>Para obter informações sobre níveis de acesso, consulte:
   <ul>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md" class="MCXref xref">Visão geral dos novos níveis de acesso</a></li>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref">Visão geral dos níveis de acesso</a></li></ul></li>
    <li>Para descobrir os detalhes do seu nível de acesso, entre em contato com o administrador do Workfront</li>
    <li>Se você for um administrador do Workfront, consulte <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configurar acesso ao Adobe Workfront</a> para saber mais sobre como conceder acesso a objetos específicos no nível de acesso.</li>  
   <li>Se você tiver o nível de acesso correto e ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</li>
    </td>
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td><p>As permissões de objeto se referem ao acesso que você tem a objetos individuais do Workfront quando os cria ou quando são compartilhados com você. Por exemplo, você deve ter acesso de Visualização a um projeto específico para visualizar o projeto, mesmo se o nível de acesso permitir que você visualize projetos. Esta seção da tabela Requisitos de acesso descreve as permissões de objeto específicas necessárias para executar a ação no artigo.</p>
   <p>Para obter informações sobre como solicitar acesso adicional a um objeto, consulte <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos</a>.</p><p>Para obter informações sobre como compartilhar um objeto, consulte <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md" class="MCXref xref">Compartilhar um objeto</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Modelo de layout</td> 
   <td><p>Os modelos de layout controlam o que pode ser visto no menu principal e são configurados pelo administrador do Workfront. Essa linha anota quaisquer áreas específicas do Workfront que devem ser incluídas no Menu principal para executar a ação.</p><p>Em geral, se um artigo instruir você a clicar em uma área no menu principal e essa área não estiver visível nesse menu, entre em contato com o administrador do Workfront para determinar se essa área pode ser disponibilizada para você.</p><p>
   Para obter informações sobre como um administrador do Workfront pode configurar o Menu Principal, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref">Personalizar o Menu Principal usando um modelo de layout</a>.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront Fusion</td> 
   <td>O Adobe Workfront Fusion tem um modelo de licenciamento separado do Workfront. 
   <ul><li>O modelo de licença atual é baseado no número de operações realizadas e não tem limitações sobre quais ações uma organização pode executar. </li>
   <li>As licenças herdadas são baseadas na capacidade dos cenários de se conectarem a aplicativos de terceiros ou se os cenários são usados apenas para automação do Workfront. </li>
   </ul>
   Para obter informações sobre o licenciamento do Fusion, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration" class="MCXref xref">licenças do Workfront Fusion</a>.
   </td> 
  </tr> 
 </tbody> 
</table>
