---
title: Gerenciar Registros na Seção de Planejamento de Objetos do Adobe Workfront
description: Você pode exibir os registros do Workfront Planning conectados a objetos do Adobe Workfront na seção Planning de um objeto do Workfront, no painel esquerdo.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 1%

---


<!--add also Group and Company when they are available-->

# Gerenciar registros na seção Planning de objetos do Adobe Workfront

{{planning-important-intro}}

Você pode exibir os registros do Workfront Planning conectados a objetos do Adobe Workfront na seção Planning de um objeto do Workfront, no painel esquerdo.

A seção Planejamento está disponível para os seguintes objetos do Workfront:

* Projeto
* Portfólio
* Programa
<!--* Group
* Company-->

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso do Workfront Planning.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produtos</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Planejamento do Adobe Workfront<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>plano do Adobe Workfront*</p></td>
   <td>
<p>Qualquer um dos seguintes planos da Workfront:</p>
<ul><li>Selecionar</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>O Workfront Planning não está disponível para planos herdados do Workfront</p>
   </td>

<tr>
   <td role="rowheader"><p>Plano de planejamento do Adobe Workfront*</p></td>
   <td>
<p>Qualquer</p>
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p>
   </td>

<tr>
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td>
   <td>
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar todos os recursos do Workfront Planning.</p>
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada do Adobe para Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td>
   <td>
   <p>Padrão</p>
   <p>O Workfront Planning não está disponível para licenças herdadas do Workfront</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configuração do nível de acesso</p></td>
   <td> <p>Acesso igual ou superior a Projetos, Programas e Portfolio</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissões de objeto</p></td>
   <td>
   <p>No Workfront, visualize ou aumente as permissões para um projeto, portfólio ou programa</a> </p> 
   <p>No Workfront Planning, Contribute ou permissões superiores para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho do Workfront Planning, incluindo aqueles que eles não criaram</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclua a área Planejamento no Menu principal e a área Planejamento para projetos, portfólios e programas. </p> Para obter mais informações, consulte <a href="/help/quicksilver/planning/access/access-overview.md">visão geral sobre o acesso ao Adobe</a>. </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações sobre a seção Planejamento de objetos do Workfront

Considere o seguinte ao exibir registros do Workfront Planning na seção Planning de um objeto Workfront:

* Os tipos de registro do Workfront Planning devem primeiro ser conectados aos tipos de objeto do Workfront.

  Para obter informações, consulte os seguintes artigos:

   * [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Conectar registros](/help/quicksilver/planning/records/connect-records.md)
* Você pode exibir a seção Planejamento de um objeto do Workfront, mesmo quando não há registros associados ao objeto do Workfront.
* Além de conectar objetos do Workfront a partir da área Planning do Workfront, você pode conectar registros do Planning a objetos do Workfront a partir do Workfront na seção Planning.

## Gerenciar registros na seção Planejamento

{{step1-to-planning}}

1. Clique no cartão de um espaço de trabalho.

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique no cartão de um tipo de registro conectado a um projeto, portfólio ou programa do Workfront.
1. Vá para um campo de registro conectado que tenha uma conexão com um objeto do Workfront, na exibição de tabela ou na página de detalhes de um registro. Para obter informações, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).
1. Clique no nome de um objeto Workfront no campo de registro conectado.
A página do objeto é aberta no Workfront.

   >[!NOTE]
   >
   >  Se você souber de um objeto do Workfront já conectado a um registro do Planning, poderá navegar até a seção do Planning a partir do objeto do Workfront.

1. Clique em **Planejamento** no painel esquerdo.

   >[!NOTE]
   >
   >   O administrador do Workfront ou do grupo deve adicionar a seção Planejamento ao modelo de layout antes que seja exibida para um projeto, portfólio ou programa do Workfront.

   A seção Planejamento é exibida com as seguintes informações:

   * Os registros conectados são exibidos em cartões individuais que contêm as seguintes informações:
      * Nome do registro
      * A miniatura do registro
      * O nome do campo de registro conectado conforme exibido no Workfront Planning.
   * Os registros são exibidos em seu respectivo espaço de trabalho.

   ![](assets/planning-section-on-project.png)

1. (Opcional) Clique em **Mostrar todas as conexões** para mostrar todos os tipos de registros conectados, incluindo aqueles sem registros conectados. Por padrão, os tipos de registro sem registros conectados não são exibidos.
1. Clique em um cartão de registro para exibir mais informações sobre o registro. A caixa de visualização do registro é exibida.
1. (Opcional) Inicie a modificação de campos na caixa de visualização do registro. Suas alterações são salvas automaticamente.
1. (Opcional) Clique no ícone ![](assets/open-details-in-a-new-tab-icon.png) de **Abrir em uma nova guia** no canto superior direito da caixa de visualização para abrir a página de detalhes do registro. A página de detalhes do registro é aberta no Workfront Planning.
1. (Opcional) Passe o mouse sobre um cartão de registro, em seguida, clique no ícone de desconectar registro **-** e clique em **Desconectar**.
As seguintes situações ocorrem:
   * O registro não está mais conectado ao objeto Workfront.
   * O objeto Workfront também é removido do campo conectado do registro do Workfront Planning.
   * Os valores dos campos de pesquisa do Workfront conectados ao registro do Planning também são excluídos.
1. Clique em **Conectar** para conectar mais registros aos tipos de registro conectados. Para obter mais informações, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

   As seguintes situações ocorrem:

   * Os registros são conectados imediatamente ao objeto Workfront e são exibidos na seção Planejamento.
   * O objeto Workfront é adicionado ao campo conectado do registro do Workfront Planning.
   * Os valores dos campos de pesquisa do Workfront conectados ao registro do Planning são preenchidos no Workfront Planning.


