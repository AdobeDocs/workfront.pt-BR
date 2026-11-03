---
title: Exibir o número de licenças alocadas e usadas em um grupo
description: Como administrador do Adobe Workfront, você pode exibir contagens dos tipos individuais de licenças usados atualmente no seu grupo e seus subgrupos. Isso é útil quando você precisa avaliar se redistribui licenças.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
TQID: 'https://experienceleague.adobe.com/z7vh7rdkB40A2gzfSYddUAHF-nOGqVCgpVyu729gYgE'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: 254442ca-6997-5cfa-963e-f420870aea53
    internal-label: People Teams and Groups
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: cb0f538ff392ebff585fbdeeba3729d9b2247292
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 6%
---
# Exibir o número de licenças alocadas e usadas em um grupo

Como administrador do Adobe Workfront, você pode exibir contagens dos tipos individuais de licenças usados atualmente no seu grupo e seus subgrupos. Isso é útil quando você precisa avaliar se redistribui licenças.

Se houver algum grupo acima do grupo gerenciado por você, os administradores também poderão fazer isso pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

>[!IMPORTANT]
>
>Uma licença de usuário é contada em um grupo específico somente se o grupo for o Grupo inicial do usuário.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Padrão</p>
       <p>Plano</p></td>
  </tr>
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Você deve ser um administrador de grupo do grupo ou um administrador do sistema.</td>
  </tr>
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir o número de licenças usadas em um grupo

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos** ![Grupos](assets/groups-icon.png).

1. Clique no nome do grupo.
1. Na página exibida, na área de cabeçalho próxima ao canto superior direito, exiba a área **Licenças em uso** para ver o número de licenças que estão sendo usadas no momento.

   Dependendo do pacote do Workfront, as licenças podem ser:

   * **Padrão** e **Leve**
   * **Plano** e **Trabalho**

   ![Licenças alocadas](assets/how-many-licenses-standard-light.png)

   Se você estiver visualizando um grupo de nível superior e o administrador do Workfront tiver definido um número máximo de cada tipo de licença para o grupo, esses números também serão exibidos como uma proporção. Por exemplo, 2/10 significa que duas licenças foram atribuídas de dez licenças disponíveis.

   Para obter informações sobre como um administrador do Workfront define um número máximo de licenças alocadas para um grupo, consulte a seção [Definir a contagem máxima de licenças para um Grupo Doméstico](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set) no artigo [Gerenciar licenças disponíveis no sistema](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

   >[!NOTE]
   >
   >Se o grupo que você está observando for um subgrupo, você poderá ver somente os números de licenças que estão sendo usadas, não o número máximo de licenças alocadas para o grupo. Isso ocorre porque os administradores do Workfront não definem uma contagem máxima de licenças para um subgrupo.
   >

1. Para contagens separadas de cada tipo de licença usada atualmente no grupo (incluindo Revisão e Solicitação), clique na área que exibe as licenças em uso.

   A caixa que é exibida fornece as mesmas informações para todos os tipos de licença do Workfront aplicáveis. Dependendo do pacote do Workfront, pode ser:

   * Padrão, Claro, Contribuinte e Externo
   * Planejar, Trabalhar, Revisar e Solicitar

   Na parte inferior da caixa, é possível ver o número total de licenças que estão sendo usadas por membros desse grupo ou de um de seus subgrupos.

   Para licenças de Revisão e Solicitação, a coluna Máximo sempre exibe Ilimitado.
