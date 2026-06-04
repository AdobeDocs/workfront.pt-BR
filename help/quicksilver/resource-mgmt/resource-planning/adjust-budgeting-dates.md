---
product-area: resource-management
navigation-topic: resource-planning
title: Ajustar datas de orçamento no Planejador de recursos
description: Se você descobrir que há superalocações de seus recursos depois de tê-los orçado no Planejador de Recursos, poderá explorar cenários hipotéticos movendo as Horas Orçadas, FTE ou Custos para outro intervalo de tempo. Com base nos resultados nesses cenários, você pode ajustar as Horas orçadas, o FTE ou o Custo.
author: Lisa
feature: Resource Management
exl-id: bc49d45a-73a5-4b02-9054-9c9dbb54224d
TQID: https://experienceleague.adobe.com/GksjnlROYkPaLMrp8vMkvx8IBZ8CPy2A54KGB2GBnVs
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 509
ht-degree: 9%

---

# Ajustar datas de orçamento no planejador de recursos

Se você descobrir que há superalocações de seus recursos depois de tê-los orçado no Planejador de Recursos, poderá explorar cenários hipotéticos movendo as Horas Orçadas, FTE ou Custos para outro intervalo de tempo. Com base nos resultados nesses cenários, você pode ajustar as Horas orçadas, o FTE ou o Custo.

As superalocações podem aparecer quando as Horas Orçadas, o FTE ou os Custos dos recursos forem maiores que as Horas Disponíveis, o FTE ou os Custos. Isso gera um valor líquido negativo.

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
   <td> <p>Editar acesso ao Gerenciamento de recursos que inclui acesso a Editar prioridades e horas de orçamento no Planejador de recursos</p> <p>Editar acesso aos Dados Financeiros que incluem acesso a Editar Taxas de Custo e Editar Finanças Gerais</p>
   <p>Editar acesso a projetos e usuários</p></td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para os projetos para os quais você deseja orçar informações com a capacidade de Editar Taxas de Custo e Editar Finanças Gerais</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajustar Datas de Orçamento

1. Vá para o Planejador de recursos e selecione **Visualizar por projeto**.

   >[!NOTE]
   >
   >Você pode usar a opção Ajustar Datas Orçadas somente quando visualiza o Planejador de Recursos por projeto.

1. Passe o mouse sobre o nome de um projeto, em seguida, clique no menu **Mais**.
1. Clique em **Ajustar Datas de Orçamento**.\
   A linha do tempo de alocação do projeto é exibida.\
   O período em que as horas são orçadas no momento é destacado em laranja se houver um conflito de orçamento e em azul se não houver conflitos.

   ![Ajustar datas de orçamento](assets/rp-adjust-budgeting-dates-with-no-done-button-350x63.png)

1. Arraste e solte o intervalo de tempo destacado para outro horário para entender onde não há conflitos de orçamento para o projeto selecionado. Quando você encontra um intervalo de tempo em que o valor Líquido é positivo, o intervalo de tempo destacado muda para azul.
1. Clique no &quot;x&quot; no canto superior direito da linha do tempo de alocação do projeto para fechá-lo.
1. Remova as horas orçadas da linha do tempo existente do projeto e adicione-as à linha do tempo que mostra mais disponibilidade.
1. Clique em **Salvar**.
1. (Condicional e opcional) Se os intervalos de tempo sem conflitos de orçamento estiverem fora da linha do tempo do projeto, clique no nome do projeto para acessá-lo.
1. (Condicional e opcional) Clique em **Editar projeto** e edite a **Data de início planejada** ou a **Data de conclusão planejada** para modificar a linha do tempo do projeto para o período sem conflitos de orçamento.\
   Para obter mais informações sobre como editar projetos, consulte o artigo [Editar projetos](../../manage-work/projects/manage-projects/edit-projects.md).

1. (Condicional e opcional) Clique em **Salvar alterações**.
1. Retorne ao Planejador de recursos e insira novamente as Horas Orçadas, FTEs ou Custos no período sem conflitos de orçamento.
1. Clique em **Salvar**.
