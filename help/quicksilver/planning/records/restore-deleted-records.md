---
title: Restaurar registros excluídos
description: Você pode recuperar registros excluídos da área Excluídos recentemente no Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8b6df633-eb05-4d3e-bfe6-76cedabdb76d
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 1%

---

# Restaurar registros excluídos

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Você pode recuperar registros excluídos da área Excluídos recentemente no Adobe Workfront Planning.

Para obter informações sobre como excluir registros, consulte [Excluir registros](/help/quicksilver/planning/records/delete-records.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso.

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
   <td role="rowheader"><p>Pacote de planejamento do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer </p> 
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td> 
   <td> 
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar o Workfront Planning.</p> 
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada da Adobe para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td> 
   <td><p> Padrão</p>
   <p>O Workfront Planning não está disponível para licenças herdadas do Workfront</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Permissões do Contribute ou superior para um espaço de trabalho <span class="preview">e tipo de registro</span> </a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modelo de layout</p></td> 
   <td> <p>No ambiente de Produção, todos os usuários, inclusive os Administradores do Sistema, devem ser atribuídos a um modelo de layout que inclua o Planning.</p>
<p><span class="preview">No ambiente de Pré-visualização, os usuários do Standard e os administradores do sistema têm o Planning habilitado por padrão.</span></p></td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Considerações sobre a recuperação de registros excluídos

* Os registros são armazenados no compartimento Excluído recentemente por 30 dias. Após 30 dias, os registros são permanentemente excluídos do Workfront Planning.
* Se os registros excluídos estiverem vinculados a outros registros, os registros vinculados não serão excluídos, mas as informações do registro excluído também serão excluídas. Restaurar os registros excluídos restaurará as informações dos registros conectados.
* Você pode restaurar registros em massa.
* Quando os registros são excluídos, as seguintes informações são armazenadas no compartimento Excluído recentemente:
   * **Nome**: estas são as informações no campo Primário do registro. Para obter mais informações sobre campos Primários de registro, consulte [Visão geral do campo Primário](/help/quicksilver/planning/fields/primary-field-overview.md).
   * **Data de exclusão**: a hora e a data em que o registro foi excluído.
   * **Tempo na exclusão recente**: o tempo desde a exclusão do registro. Os registros que foram excluídos mais de 30 dias antes da data atual não são exibidos no compartimento Excluídos recentemente.
   * **Excluído por**: o nome do usuário que excluiu o registro.

## Restaurar registros excluídos

1. Vá para a página de tipo de registro na qual você excluiu registros.
1. Clique no ícone **Desfazer** ![Ícone Desfazer](assets/undo-icon.png) no canto superior direito de qualquer exibição de página de tipo de registro e clique em **Excluído recentemente**.

   A caixa **Excluído recentemente** é exibida.

   ![Caixa excluída recentemente](assets/recently-deleted-box.png)

1. Selecione os registros que deseja excluir e clique em **Restaurar** > **Restaurar**. Você pode selecionar mais de um registro.

   Se a restauração tiver sido bem-sucedida, você receberá uma notificação de sucesso na parte inferior da tela.
1. Vá para a exibição de tabela e revise os registros restaurados.
