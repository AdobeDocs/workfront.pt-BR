---
product-area: resource-management
navigation-topic: resource-planning
title: Ajustar datas de orçamento no Planejador de Recursos
description: Se você achar que há sobrealocações de seus recursos depois de fazer o orçamento deles no Planejador de Recursos, você pode explorar cenários de hipóteses movendo as Horas Orçadas, FTE ou Custos para outro período. Com base nas descobertas nesses cenários, você pode ajustar as Horas orçadas, FTE ou Custo.
author: Alina
feature: Resource Management
exl-id: bc49d45a-73a5-4b02-9054-9c9dbb54224d
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 1%

---

# Ajustar datas de orçamento no Planejador de Recursos

Se você achar que há sobrealocações de seus recursos depois de fazer o orçamento deles no Planejador de Recursos, você pode explorar cenários de hipóteses movendo as Horas Orçadas, FTE ou Custos para outro período. Com base nas descobertas nesses cenários, você pode ajustar as Horas orçadas, FTE ou Custo.

As atribuições excessivas podem aparecer quando as Horas Orçadas, FTE ou Custos de seus recursos forem maiores que as Horas Disponíveis, FTE ou Custos. Isso gera um valor líquido negativo.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Pro e superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Edite o acesso ao Gerenciamento de Recursos que inclui acesso a Editar prioridades e horas orçamentárias no Planejador de Recursos</p> <p>Editar acesso a dados financeiros, projetos e usuários</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerencie permissões dos projetos para os quais deseja obter informações de orçamento com a capacidade de Gerenciar finanças</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Ajustar Datas de Orçamento

1. Vá para o Planejador de Recursos e selecione **Exibir por projeto**.

   >[!NOTE]
   >
   >Você pode usar a opção Ajustar Datas Orçadas somente quando exibir o Planejador de Recursos por projeto.

1. Passe o mouse sobre o nome de um projeto e clique no botão **Mais** menu.
1. Clique em **Ajustar datas de orçamento**.\
   A linha do tempo de alocação do projeto é exibida.\
   O período em que as horas estão orçamentadas é destacado em laranja se houver um conflito orçamentário e em azul se não houver conflitos.

   ![](assets/rp-adjust-budgeting-dates-with-no-done-button-350x63.png)

1. Arraste e solte o período de tempo destacado para outro momento para entender onde não há conflitos de orçamento para o projeto selecionado. Quando você encontra um período em que o valor de Líquido é positivo, o período realçado muda para azul.
1. Clique no &quot;x&quot; no canto superior direito da linha do tempo de alocação do projeto para fechá-lo.
1. Remova as horas orçadas da linha do tempo existente do projeto e adicione-as à linha do tempo que mostra a maior disponibilidade.
1. Clique em **Salvar**.
1. (Condicional e opcional) Se os intervalos de tempo sem conflitos de orçamento estiverem fora da linha do tempo do projeto, clique no nome do projeto para acessar o projeto.
1. (Condicional e opcional) Clique em **Editar projeto** em seguida, edite o **Data de início planejada** ou **Data de Conclusão Planejada** para modificar a linha do tempo do projeto para o período sem conflitos de orçamento.\
   Para obter mais informações sobre edição de projetos, consulte o artigo [Editar projetos](../../manage-work/projects/manage-projects/edit-projects.md).

1. (Condicional e opcional) Clique em **Salvar alterações**.
1. Retorne ao Planejador de Recursos e insira novamente as Horas Orçadas, FTEs ou Custos no período sem conflitos orçamentários.
1. Clique em **Salvar**.
