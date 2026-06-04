---
product-area: projects
navigation-topic: financials
title: Definir o Método de índice de desempenho (PIM)
description: O Método de índice de desempenho (PIM) do projeto controla o método que a Adobe Workfront usa para calcular as métricas de desempenho do projeto, como Índice de desempenho de custo (CPI), Índice de desempenho de cronograma de custo (CSI), Índice de desempenho de cronograma (SPI) e Estimar na conclusão (EAC).
author: Lisa
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
TQID: https://experienceleague.adobe.com/g4FYe8k1psS9xuL6Z40teAyJ-SV4UD6ThnWvnvl8au4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 418
ht-degree: 12%

---

# Definir o Método de índice de desempenho (PIM)

O Método de índice de desempenho (PIM) do projeto controla o método que a Adobe Workfront usa para calcular as métricas de desempenho do projeto, como Índice de desempenho de custo (CPI), Índice de desempenho de cronograma de custo (CSI), Índice de desempenho de cronograma (SPI) e Estimar na conclusão (EAC).

O Workfront calcula esses valores usando o seguinte:

* Horas
* Custo

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td>Qualquer </td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td>
   <p>Padrão</p>
   <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Editar acesso a Projetos e Dados Financeiros</td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td>Gerenciar permissões para o projeto com permissões para Editar Finanças Gerais</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações sobre o PIM no Workfront

* O administrador do Workfront ou um administrador de grupo define o padrão para determinar se o Método de Índice de Desempenho (PIM) deve ser baseado em hora ou em custo. Os cálculos para as métricas de desempenho mudam de acordo com como esse padrão é definido. Para obter mais informações sobre como alterar o padrão de cálculo do PIM, consulte [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Os gerentes de projeto também podem alterar a configuração do PIM, no nível do projeto, para projetos individuais na subguia Finanças do projeto. Você deve ter permissões de Gerenciamento no projeto para editar a subguia Finanças do projeto.

## Definir o Método de Índice de Desempenho (PIM) de um projeto

1. Vá para um projeto do qual você é o proprietário.

   >[!IMPORTANT]
   >
   >Você precisa de Permissões de gerenciamento para o projeto para executar as etapas a seguir. Também recomendamos que somente o Proprietário do projeto faça alterações na área Finanças do projeto.

1. Clique em **Detalhes do projeto** no painel esquerdo e vá para a área **Finanças**.
1. Clique duas vezes no valor no campo **Método de indexação de desempenho** para editá-lo.
1. Selecione entre as seguintes opções no campo **Método de indexação de desempenho**:

   | Baseado em Hora | O Workfront usa as horas planejadas no cálculo da CPI e da EAC do projeto, e a EAC do projeto é exibida como um número, em horas. |
   |---|---|
   | Baseado em Custo | O Workfront usa o Custo de mão de obra planejado no cálculo do CPI e do EAC do projeto, e o EAC é exibido como um valor de moeda. Ao selecionar essa opção, certifique-se de que os atribuídos da tarefa (funções de cargo ou usuários) estejam associados a taxas de custo. |

   {style="table-layout:auto"}

1. Clique em **Salvar** **Alterações**.
