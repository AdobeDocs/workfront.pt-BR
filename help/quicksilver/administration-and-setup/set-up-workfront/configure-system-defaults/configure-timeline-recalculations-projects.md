---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: Configurar recálculos de linha de tempo para projetos
description: Recalcular linhas do tempo permite que os gerentes vejam como as forças fora do projeto estão afetando a linha do tempo do projeto. A linha do tempo de um projeto se refere às datas planejadas e projetadas para o projeto.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# Configurar recálculos de cronograma de projetos

Recalcular linhas do tempo permite que os gerentes vejam como as forças fora do projeto estão afetando a linha do tempo do projeto. A linha do tempo de um projeto se refere às datas planejadas e projetadas para o projeto.

Como administrador [!DNL Adobe Workfront], você pode recalcular manualmente as linhas de tempo de todos os projetos no sistema. Os proprietários de projetos também podem recalcular manualmente as linhas do tempo de projetos individuais. Para obter mais informações, consulte [Recalcular linhas do tempo do projeto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

Este artigo descreve como você, como administrador do [!DNL Workfront], pode determinar como e quando o [!DNL Workfront] calcula automaticamente as linhas do tempo do projeto, configurando as preferências do projeto na área [!UICONTROL Configuração].

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacote</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licença</td> 
   <td><p>[!UICONTROL Padrão]</p>
       <p>[!UICONTROL Plano]</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar recálculos automáticos

Como administrador [!DNL Adobe Workfront], você pode configurar quando [!DNL Workfront] recalcula automaticamente as linhas de tempo do projeto. [!DNL Workfront] pode recalcular as linhas de tempo do projeto todas as noites, quando o escopo do projeto mudar, ou ambos.

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Preferências do projeto]** > **[!UICONTROL Projetos].**

1. Na seção **[!UICONTROL Linhas do Tempo]**, habilite ou desabilite uma ou ambas as configurações abaixo. Por padrão, ambas as configurações são ativadas.

   * **Todas as noites:** [!DNL Workfront&#x200B;&#x200B;&#x200B;] recalcula as linhas do tempo uma vez a cada 24 horas, à noite, somente para projetos com status [!UICONTROL Atual] e que foram atualizados nos últimos três meses. Dependendo da carga do sistema e de outros fatores, o tempo de recálculo pode ser atrasado em mais de 24 horas.

     Neste caso, [!DNL Workfront] recalcula a linha do tempo de todos os projetos que têm um [!UICONTROL Tipo de Atualização] de [!UICONTROL Automático] ou [!UICONTROL Automático e Mediante Alteração].

   * **Quando o escopo de um projeto for alterado**: Para obter informações sobre o que constitui uma alteração de escopo de projeto, consulte [Recalcular linhas do tempo do projeto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

     Neste caso, [!DNL Workfront] recalcula a linha do tempo de todos os projetos que têm um Tipo de Atualização de [!UICONTROL Automático e Em Alteração] ou [!UICONTROL Somente em Alteração].
Para obter informações sobre Tipos de Atualização de Projeto, consulte [Visão geral sobre Tipos de Atualização de Projeto](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. Clique em **[!UICONTROL Salvar]**.

   A linha do tempo de todos os projetos no sistema é recalculada automaticamente com base no Tipo de atualização de cada projeto.

>[!IMPORTANT]
>
>Para os ambientes Visualização e Atualização personalizada da sandbox, o recálculo noturno é desativado e as linhas de tempo do projeto não são recalculadas automaticamente. Você deve recalcular manualmente a linha do tempo do projeto para os ambientes Pré-visualização e Atualização personalizada da sandbox. Para obter informações, consulte [Recalcular linhas do tempo do projeto](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md).


## Recalcular linhas do tempo para toda a instância [!DNL Workfront]

Você pode executar o diagnóstico [!UICONTROL Recalcular Linha do Tempo] para recalcular manualmente todas as linhas do tempo no sistema [!DNL Workfront]. Isso permite que todos os gerentes de projeto vejam a influência das alterações externas imediatamente nas datas planejadas e projetadas. Para obter mais informações, consulte [Usar Diagnóstico para acionar processos automatizados](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
