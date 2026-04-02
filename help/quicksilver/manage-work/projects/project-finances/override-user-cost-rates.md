---
content-type: overview
product-area: projects
navigation-topic: financials
title: Sobrepor Taxas de Custo do Usuário no Nível do Projeto
description: Este artigo descreve como é possível substituir as taxas de custo de usuário do sistema para um projeto.
author: Lisa
feature: Work Management
source-git-commit: cb21414992587c62c37580f156100f2b5b755e9b
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 5%

---

# Substituir taxas de custo do usuário no nível do projeto

{{highlighted-preview-article-level}}

Você pode especificar qual é a taxa de custo para um usuário em um projeto específico. Essa taxa de custo no nível do projeto substitui a taxa de custo no nível do sistema para esse usuário. O Workfront usa a taxa de custo no nível do projeto da função de trabalho para calcular o custo, em vez de usar a taxa de custo no nível do sistema.

Este artigo descreve como é possível substituir as taxas de custo de usuário do sistema para um projeto.

Para obter mais informações sobre como calcular custos no projeto, consulte [Visão geral da hierarquia de receita e custo](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) e [Rastrear custos](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td>Padrão</td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a Projetos e Dados Financeiros</p>
       <p><p>Você também deve ter um dos seguintes:</p> 
        <ul> 
          <li> <p>O nível de acesso Administrador do sistema. </li> 
          <li> <p>A configuração <b>Usuários</b> no seu nível de acesso foi configurada para <b>Editar</b> acesso, com as opções <b>Criar</b> e pelo menos uma das duas opções <b>Administrador de Usuários</b> habilitadas em <b>Ajustar suas configurações</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Dessas duas opções, se <b>Administrador de Usuários (Usuários de Grupo)</b> estiver habilitado, você deverá ser um administrador de grupo de um grupo do qual o usuário seja membro.</p> </li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td>Gerenciar permissões para o projeto que inclui Editar Dados Financeiros </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

O usuário deve ter o campo **Substituição de taxa de custo permitida** habilitado em seu perfil de usuário. Quando um usuário não tem o campo de sobreposição de custo ativado, as sobreposições de custo não são permitidas para esse usuário em nenhum projeto e o sistema usa a taxa no perfil do usuário para calcular o custo.

Para obter mais informações, consulte [Editar perfil de usuário](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Substituir taxas de custo do usuário no nível do projeto

1. Vá para o projeto para o qual você deseja substituir as taxas de custo.
1. Clique em **Taxas** no painel esquerdo. Talvez seja necessário clicar primeiro em **Mostrar mais**.
1. Clique na guia **Custo** se ela ainda não estiver selecionada.
1. Clique em **Adicionar taxa de custo** > **Nova taxa de custo do usuário**.

   A caixa Nova Taxa de Custo de Usuário é aberta.

1. No campo **Usuário**, selecione o usuário para o qual deseja alterar a taxa de custo.
1. Selecione a **Moeda** para a substituição da taxa de custo.
1. No campo **Taxa de Custo**, insira a primeira substituição de taxa de custo.
1. (Opcional) Clique em **Adicionar taxa efetiva de data** para adicionar mais substituições de taxa de custo.

   >[!NOTE]
   >
   >Se você informar uma sobreposição de taxa única, ela será aplicada por toda a vida útil do projeto.
   >Se você quiser ter taxas diferentes ao longo do tempo, poderá adicionar várias sobreposições de data de efetivação.

1. (Condicional) Se você estiver adicionando várias sobreposições de taxa de custo, especifique as seguintes informações para cada linha:

   * **Taxa de Custo**: o valor da taxa de custo durante o período especificado.
   * **Data de Início**: a data em que a substituição da taxa de custo começa.
   * **Data Final**: a data em que a substituição da taxa de custo termina.

   ![Caixa Nova Taxa de Custo de Usuário mostrando datas de efetivação](assets/new-user-cost-rate-box.png)

   O Workfront aplica a taxa de substituição de função de trabalho às horas que ocorrem durante esses períodos ao calcular o custo do projeto.

   Não deve haver lacunas entre os intervalos de tempo de duas taxas de substituição. A **Data de Início** de uma taxa de substituição deve ser o dia imediatamente após a **Data de Término** da data de substituição anterior.

   Você não precisa especificar uma Data Inicial para a primeira taxa de sobreposição, nem uma Data Final para a última taxa de sobreposição.

   Recomendamos que você use a Taxa padrão para a primeira taxa de substituição.

   O Workfront presume que a primeira taxa de sobreposição seja aplicada para todas as horas com uma data anterior à Data Final da primeira sobreposição e que a última taxa de sobreposição seja aplicada para todas as horas com uma data mais recente que a Data Inicial da última sobreposição.

   Se uma hora for registrada antes da Data de início planejada do projeto, a primeira taxa de custo será usada.

   Se uma hora for registrada depois da Data de conclusão planejada do projeto, a última taxa de custo será usada.

1. Clique em **Salvar**.


