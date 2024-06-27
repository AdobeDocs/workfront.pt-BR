---
title: Gerenciar registros na seção Planning de objetos do Adobe Workfront
description: Você pode exibir os registros conectados a objetos do Adobe Workfront na seção Planejamento de um objeto do Workfront, no painel esquerdo.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: 64f187ed78b69db9b9ac0259e96ef0bf47abf4f4
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--add also Group and Company when they are available-->

<!-- opening the Details preview and page is not possible yet - hid those steps, but add them when released-->


# Gerenciar registros na seção Planning de objetos do Adobe Workfront

{{planning-important-intro}}

Você pode exibir os registros conectados a objetos do Adobe Workfront na seção Planejamento de um objeto do Workfront, no painel esquerdo.

A seção Planejamento está disponível para os seguintes objetos do Workfront:

* Projeto
* Portfólio
* Programa
<!--* Group
* Company-->

## Requisitos de acesso

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
   <p> Produto</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>contrato do Adobe Workfront</p></td>
   <td>
<p>Sua organização deve estar inscrita no estágio de acesso antecipado do Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plano do Adobe Workfront</p></td>
   <td>
<p>Qualquer</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td>
   <td>
   <p>Novo: Padrão</p>
   Ou
   <p>Atual: Plano</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurações de nível de acesso</p></td>
   <td> <p>Acesso igual ou superior a Projetos, Programas e Portfolio</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>No Workfront, visualize ou aumente as permissões de um projeto, portfólio ou programa</a> </p> 
   <p>No Workfront Planning, no Contribute ou em permissões superiores para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho do Workfront Planning, incluindo aqueles que eles não criaram</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área Planejamento no Menu Principal e a seção Planejamento no painel esquerdo ao modelo de layout. Para obter informações, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Considerações sobre a seção Planejamento de objetos do Workfront

* Primeiro, você deve conectar tipos de registro a tipos de objeto do Workfront e registros a objetos do Workfront para visualizá-los no Workfront.

  Para obter informações, consulte os seguintes artigos:

   * [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Conectar registros](/help/quicksilver/planning/records/connect-records.md)
* Você pode exibir a seção Planejamento em um objeto Workfront, mesmo quando não há registros associados ao objeto Workfront.
* Você pode conectar registros do Planning a objetos do Workfront a partir do Workfront, na seção Planning quando houver pelo menos um registro conectado ao objeto do Workfront.

## Gerenciar registros na seção Planejamento

{{step1-to-planning}}

1. Clique no cartão de um espaço de trabalho.

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique no cartão de um tipo de registro conectado a um projeto, portfólio ou programa do Workfront.
1. Vá para um campo de registro conectado que tenha uma conexão com um objeto do Workfront, na exibição de tabela ou na página de detalhes de um registro. Para obter informações, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).
1. Clique no nome de um objeto Workfront no campo de registro conectado.
A página dos objetos é aberta no Workfront Planning.
1. Clique em **Ir para origem**, no canto superior direito da tela.

   A página do objeto é aberta no Workfront.
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

1. Clique em um cartão de registro para exibir mais informações sobre o registro. A caixa de visualização do registro é exibida.
1. (Opcional) Inicie a modificação de campos na caixa de visualização do registro. Suas alterações são salvas automaticamente.
1. (Opcional) Clique no link **Abrir em uma nova guia** ícone ![](assets/open-details-in-a-new-tab-icon.png) no canto superior direito da caixa de visualização para abrir a página de detalhes do registro. A página de detalhes do registro é aberta no Workfront Planning.
1. Passe o mouse sobre um cartão de registro e clique no ícone desconectar registro **-** e, em seguida, clique em **Desconectar**.
As seguintes situações ocorrem:
   * O registro não está mais conectado ao objeto Workfront.
   * O objeto Workfront também é removido do campo conectado do registro do Workfront Planning.
   * Os valores dos campos de pesquisa do Workfront conectados ao registro do Planning também são excluídos.
1. Clique em **Conectar** para conectar mais registros.

   >[!NOTE]
   >
   >   O botão Conectar é exibido apenas para os espaços de trabalho em que você tem permissões do Contribute. <!--they might replace this with one button at the top of the page. Rephrase-->

1. Clique nos registros que deseja conectar. As seguintes situações ocorrem:

   * Os registros são conectados imediatamente ao objeto Workfront e são exibidos na seção Planejamento.
   * O objeto Workfront é adicionado ao campo conectado do registro do Workfront Planning.
   * Os valores dos campos de pesquisa do Workfront conectados ao registro do Planning são preenchidos no Workfront Planning.

<!--add more steps here for what happens after clicking Connect-->
