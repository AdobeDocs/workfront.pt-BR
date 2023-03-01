---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Executar relatórios em [!DNL Workfront Proof]
description: O Workfront Proof permite exibir relatórios para que você possa acompanhar o progresso do trabalho e a eficiência de suas equipes.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 342f9282-b6f5-425e-a7ef-e23bd011d284
source-git-commit: a0d76692f9e9d12ed0d538c1344638dbc208d625
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 0%

---

# Executar relatórios em [!DNL Workfront Proof]


>[!IMPORTANT]
>
>* <span class="previe">A funcionalidade de relatórios não está mais disponível no [!DNL Workfront Proof]. A guia de relatórios ainda é exibida, mas os dados não são precisos.</span>
> 
>* Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro do [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).


O Workfront Proof permite exibir relatórios para que você possa acompanhar o progresso do trabalho e a eficiência de suas equipes.

É possível visualizar facilmente o número de provas que foram criadas no [!DNL Workfront Proof] conta, quantas versões estão associadas a cada prova, o tempo de resposta e muito mais.

## Pré-requisitos

A disponibilidade de relatórios depende do seu tipo de [!DNL Workfront Proof] níveis de permissão de conta e usuário.

* [Pré-requisitos da conta](#account-prerequisites)
* [Pré-requisitos do usuário](#user-prerequisites)

### Pré-requisitos da conta {#account-prerequisites}

As informações de relatórios estão disponíveis somente com planos Premium.

### Pré-requisitos do usuário {#user-prerequisites}

As informações de relatórios estão disponíveis somente para usuários com acesso total a todas as provas em sua conta (ou seja, usuários com pelo menos [Perfis de permissões de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)).

Nesse painel, é possível

* Controlar o período de tempo dos dados exibidos
* Analisar alterações nas métricas ao longo do tempo
* Verificar os detalhes de um ponto selecionado ao passar o mouse sobre ele
* Verifique o número total de provas criadas no período selecionado
* Verifique o número médio de versões incluídas nos conjuntos completos de provas

## Exibição de relatórios {#viewing-reports}

1. Vá para a **[!UICONTROL Painéis]** página.
1. Clique em **[!UICONTROL Relatórios]** guia.\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. No **[!UICONTROL Período de tempo]** selecione se deseja exibir informações sobre provas criadas nas últimas 24 horas, 7 dias, 30 dias, 90 dias ou um período personalizado.\
   Se você selecionar um período personalizado, selecione as datas de início e término e clique em **[!UICONTROL Aplicar]**.\
   As seguintes informações são exibidas para o período selecionado:\
   **Prova criada:** Número de provas criadas dentro do período selecionado.\
   **Versões por prova:** Número médio de versões por prova para todas as provas concluídas (Aprovado ou Aprovado com Alterações) no período selecionado.\
   **Horário de retorno:** Tempo médio desde quando a primeira versão foi criada até o momento em que a decisão foi tomada na versão final.\
   **Hora da primeira atividade:** Tempo médio desde quando a prova foi criada até o momento da primeira atividade na prova.\
   **Provas com atraso:** Porcentagem média de provas concluídas (Aprovado ou Aprovado com alterações) que tinham pelo menos uma versão atrasada dentro do período selecionado.\
   **Comentários e respostas:** Número médio de comentários e respostas que foram feitos em todas as provas no período selecionado.

1. (Opcional) Selecione ou desmarque a opção **[!UICONTROL Mostrar intervalo mínimo-máximo]** opção para determinar se os valores mínimo e máximo são exibidos no gráfico.\
   Quando essa opção é selecionada, o sombreamento azul é exibido entre os valores mínimo e máximo registrados.

1. (Opcional) Você pode filtrar os dados exibidos, conforme descrito em [Filtrar relatórios](#filtering-reports).

## Filtrar relatórios {#filtering-reports}

Por padrão, os dados exibidos nos relatórios incluem todas as informações da [!DNL Workfront Proof] sistema. Você pode usar filtros para mostrar apenas as informações relevantes às suas necessidades.

Para filtrar informações sobre relatórios:

1. Vá para a **[!UICONTROL Painéis]** página.
1. Clique em **[!UICONTROL Relatórios]** guia.\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. Execute um relatório, conforme descrito em [Exibição de relatórios](#viewing-reports).
1. Clique em **[!UICONTROL Filtro]**.

1. No lado esquerdo da página, selecione uma das seguintes opções de filtro:\
   **[!UICONTROL Tipo de prova]:** Selecione o tipo de prova que deseja incluir no relatório.\
   **[!UICONTROL Decisões]:** Selecione as opções para determinar se apenas as provas que contêm determinadas decisões foram feitas.\
   **[!UICONTROL Destinatários]:** Selecione usuários individuais para exibir informações relacionadas às provas compartilhadas com os usuários selecionados.\
   **[!UICONTROL Proprietários da prova]:** Selecione usuários individuais para exibir informações relacionadas às provas de propriedade dos usuários selecionados.\
   **[!UICONTROL Criadores de provas]:** Selecione usuários individuais para exibir informações relacionadas às provas criadas pelos usuários selecionados.\
   **[!UICONTROL Contas]:** Selecione quais contas deseja incluir no relatório.

1. Clique em **[!UICONTROL Aplicar]**.
1. (Opcional) Selecione ou desmarque a opção **[!UICONTROL Mostrar intervalo mínimo-máximo]** opção para determinar se os valores mínimo e máximo são exibidos no gráfico.\
   Quando essa opção é selecionada, o sombreamento azul é exibido entre os valores mínimo e máximo registrados.

## Impressão de relatórios

1. Vá para a **[!UICONTROL Painéis]** página.
1. Clique em **[!UICONTROL Relatórios]** e clique em **[!UICONTROL Imprimir]**.\
   ![proof_reports_print.png](assets/proof-reports-print-350x191.png)

1. Selecione entre as várias opções de impressão disponíveis.\
   As opções de impressão variam de acordo com o navegador e a versão do navegador usada.
