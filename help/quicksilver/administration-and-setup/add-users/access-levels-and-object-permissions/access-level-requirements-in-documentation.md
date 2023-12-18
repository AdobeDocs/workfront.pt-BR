---
title: Requisitos de níveis de acesso
content-type: reference
product-area: system-administration
keywords: acesso,nível,sistema,administrador,planejador,trabalhador,revisor,solicitante,externo,usuário
navigation-topic: access-levels
description: Os artigos de instruções da documentação do Workfront contêm uma tabela que explica o acesso e as permissões necessárias para esse procedimento. Este artigo explica a tabela de requisitos de acesso com mais detalhes e contém links para obter mais informações.
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
source-git-commit: d786a5bd86bcc1a4fbacf022cc9fbee9cb321da5
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 0%

---

# Requisitos de níveis de acesso na documentação do Workfront

Os artigos de instruções da documentação do Workfront contêm uma tabela que explica os requisitos de acesso e permissões necessários para esse procedimento. Esta tabela de Requisitos de acesso permite compreender se você pode executar uma determinada ação no Workfront ou por que não pode fazê-lo. Este artigo explica cada elemento da tabela Requisitos de acesso e fornece dicas e links para a solução de problemas a informações mais detalhadas.

Se uma linha estiver ausente da tabela Requisitos de acesso em um determinado artigo, não há requisitos desse tipo para essa ação.

>[!NOTE]
>
>Em caso de dúvidas sobre como qualquer um dos campos desta tabela se aplica a você, entre em contato com o administrador do Workfront.

## A tabela Requisitos de acesso

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> Os planos da Adobe Workfront se referem ao conjunto de recursos que sua organização adquiriu. A maior parte da funcionalidade do Workfront está disponível em todos os planos, com algumas exceções, relacionadas principalmente ao planejamento estratégico e aos controles corporativos. 
   <ul><li>Para descobrir qual plano da Adobe Workfront sua organização usa, incluindo se sua organização está no novo ou no atual modelo de empacotamento, entre em contato com o administrador do Workfront.</li>
   <li>Para obter instruções sobre como um administrador do Workfront pode localizar o plano Workfront de sua organização, consulte <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan" class="MCXref xref">Exibir o cluster da sua organização e o plano da Workfront</a>.</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> As licenças do Adobe Workfront se referem ao conjunto de recursos do Workfront incluídos na licença atribuída a você. Por exemplo, um usuário pode ter uma licença que inclui a marcação da conclusão dos itens de trabalho e o registro do tempo, enquanto outro usuário tem uma licença que permite apenas aprovar ativos ou enviar solicitações. <p> 
   <ul>
   <li>Para descobrir qual licença você está atribuído, entre em contato com o administrador do Workfront.</li>
   <li>A Adobe Workfront está fazendo a transição para um novo modelo de preços e pacotes. Para obter informações sobre licenças, consulte:
   <ul>
   <li>Novo: <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Visão geral de novas licenças</a></li>
   <li>Atual: <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Visão geral de licenças</a></li></ul></li>
   <li>Se você tiver o nível de acesso correto e ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.
   </ul>
      </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso</td> 
   <td> Os níveis de acesso são conjuntos de permissões para ações que podem ser executadas no Workfront, definidos pelo administrador do Workfront. <p>A Workfront tem níveis de acesso integrados que correspondem às licenças da Workfront, mas o administrador do Workfront pode criar mais níveis de acesso para refletir com mais precisão os conjuntos de permissões necessários na organização.</p>
   <ul>
    <li>A Adobe Workfront está fazendo a transição para um novo modelo de preços e pacotes. Para obter informações sobre níveis de acesso para cada modelo, consulte:
   <ul>
   <li>Novo: <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md" class="MCXref xref">Visão geral dos novos níveis de acesso</a></li>
   <li>Atual: <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref">Visão geral dos níveis de acesso</a></li></ul></li>
    <li>Para descobrir os detalhes do seu nível de acesso, entre em contato com o administrador do Workfront</li>
    <li>Se você for um administrador do Workfront, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configuração do acesso ao Adobe Workfront</a> para saber mais sobre como conceder acesso a objetos específicos no nível de acesso.</li>  
   <li>Se você tiver o nível de acesso correto e ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</li>
    </td>
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td><p>As permissões de objeto se referem ao acesso que você tem a objetos individuais do Workfront quando os cria ou quando são compartilhados com você. Por exemplo, você deve ter acesso de Visualização a um projeto específico para visualizar o projeto, mesmo se o nível de acesso permitir que você visualize projetos. Esta seção da tabela Requisitos de acesso descreve as permissões de objeto específicas necessárias para executar a ação no artigo.</p>
   <p>Para obter informações sobre como solicitar acesso adicional a um objeto, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>A Workfront oferece alguns produtos que podem ser comprados além do Workfront.
   <p>Os artigos que descrevem os procedimentos executados nesses produtos adicionais listam o produto necessário aqui.</p>
   <ul>
   <li>Adobe Experience Manager Assets ou Assets Essentials </li>
   <li>Workfront Fusion</li>
   <li>Workfront Goals</li>
   <li>Planejador de cenários do Workfront</li>
   </ul>
   <p>Para saber se sua organização adquiriu um desses produtos adicionais, entre em contato com o administrador do Workfront.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront Fusion</td> 
   <td>O Adobe Workfront Fusion tem um modelo de licenciamento separado do Workfront. 
   <ul><li>Atual: O modelo de licença atual é baseado no número de operações realizadas e não tem limitações sobre quais ações uma organização pode executar. </li>
   <li>Herdados: as licenças herdadas se baseiam na capacidade dos cenários de se conectarem a aplicativos de terceiros ou se os cenários são usados apenas para automação do Workfront. </li>
   </ul>
   Para obter informações sobre o licenciamento do Fusion, consulte <a href="/help/quicksilver/workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">Licenças do Workfront Fusion</a>.
   </td> 
  </tr> 
 </tbody> 
</table>


