---
product-area: projects
navigation-topic: financials
title: Definir o PIM (Performance Index Method)
description: O PIM (Performance Index Method) do projeto controla o método que a Adobe Workfront usa para calcular métricas de desempenho do projeto, como CPI (Cost Performance Index), CSI (Cost Schedule Performance Index), SPI (Schedule Performance Index) e EAC (Estimate At Completion Index).
author: Alina
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 1%

---

# Definir o PIM (Performance Index Method)

O PIM (Performance Index Method) do projeto controla o método que a Adobe Workfront usa para calcular métricas de desempenho do projeto, como CPI (Cost Performance Index), CSI (Cost Schedule Performance Index), SPI (Schedule Performance Index) e EAC (Estimate At Completion Index).

O Workfront calcula esses valores usando o seguinte:

* Horas
* Custo

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos e Dados Financeiros</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerencie permissões do projeto com permissões para Gerenciar finanças</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Considerações sobre o PIM no Workfront

* O administrador do Workfront ou um administrador de grupo configura o padrão para determinar se o Método de Índice de Desempenho (PIM) deve ser baseado em hora ou em custo. Os cálculos para as métricas de desempenho mudam de acordo com a forma como esse padrão é definido. Para obter mais informações sobre como alterar o padrão de como calcular o PIM, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Os gerentes de projeto também podem alterar a configuração do PIM, no nível do projeto, para projetos individuais na subguia Finanças do projeto. Você deve ter permissões de gerenciamento no projeto para editar a subguia Finanças do projeto.

## Definir o Método de Índice de Desempenho (PIM) de um projeto

1. Vá para um projeto do qual você é o proprietário.

   >[!IMPORTANT]
   >
   >Você precisa gerenciar permissões no projeto para executar as etapas a seguir. Recomendamos também que somente o Proprietário do projeto faça alterações na área de finanças do projeto.

1. Clique em **Detalhes do projeto** no painel esquerdo, em seguida, vá para o **Finanças** área.
1. Clique duas vezes no valor na **Método do Índice de Desempenho** para editá-lo.
1. Selecione dentre as seguintes opções no **Método do Índice de Desempenho** campo :

   | Baseado em Hora | O Workfront usa as Horas Planejadas para calcular o CPI e o EAC do projeto, e o EAC do projeto é exibido como um número, em horas. |
   |---|---|
   | Baseado em Custo | O Workfront usa o Custo Planejado da Mão de obra para calcular o CPI e o EAC do projeto, e o EAC é exibido como um valor de moeda. Ao selecionar essa opção, verifique se os destinatários da tarefa (funções de trabalho ou usuários) estão associados a taxas de custo. |

   {style=&quot;table-layout:auto&quot;}

1. Clique em **Salvar** **Alterações**.
