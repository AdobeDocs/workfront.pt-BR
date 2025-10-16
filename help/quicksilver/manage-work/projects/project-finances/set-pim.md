---
product-area: projects
navigation-topic: financials
title: Definir o PIM (Método de Índice de Desempenho)
description: O Método de índice de desempenho (PIM) do projeto controla o método que a Adobe Workfront usa para calcular as métricas de desempenho do projeto, como Índice de desempenho de custo (CPI), Índice de desempenho de cronograma de custo (CSI), Índice de desempenho de cronograma (SPI) e Estimar na conclusão (EAC).
author: Lisa
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 1%

---

# Definir o PIM (Método de Índice de Desempenho)

O Método de índice de desempenho (PIM) do projeto controla o método que a Adobe Workfront usa para calcular as métricas de desempenho do projeto, como Índice de desempenho de custo (CPI), Índice de desempenho de cronograma de custo (CSI), Índice de desempenho de cronograma (SPI) e Estimar na conclusão (EAC).

O Workfront calcula esses valores usando o seguinte:

* Horas
* Custo

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <p>Standard</p>
   <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Editar acesso a Projetos e Dados Financeiros</td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td>Gerenciar permissões do projeto com permissões para Gerenciar Finanças</td> 
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
