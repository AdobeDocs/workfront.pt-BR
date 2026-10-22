---
title: Visão geral da versão do primeiro trimestre de 2027
description: Esta página fornece informações sobre a funcionalidade incluída na versão do Primeiro trimestre de 2027. Essas melhorias estão previstas para serem disponibilizadas no ambiente de produção ao longo do trimestre.
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 18e1d35b98b8c1afc6f9c1b14dba73d160b7e420
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 30%
---

# Visão geral da versão do primeiro trimestre de 2027

Esta página fornece informações sobre a funcionalidade incluída na versão do Primeiro trimestre de 2027 programada para janeiro de 2027.

As melhorias nesta página estão disponíveis no ambiente de pré-visualização. Esta página será atualizada com melhorias adicionais à medida que a versão do Primeiro trimestre de 2027 se aproximar da versão de produção planejada.

>[!IMPORTANT]
>
>
>As versões mensais e trimestrais estão previstas para serem disponibilizadas na quinta-feira da segunda semana completa do mês, salvo indicação em contrário.
>
>| Versão mensal | Versão trimestral |
>|----|----|
>| <ul><li>2026.11 (12 de novembro de 2026)</li><li>2026.12 (17 de dezembro de 2026)</li><li>2027.01 (21 de janeiro de 2027)</li></ul> | <ul><li>2027.01 (21 de janeiro de 2027)</li></ul> |
>
>Para obter mais informações sobre o processo de lançamento rápido, consulte [Habilitar ou desabilitar o processo de lançamento rápido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Aprimoramentos do Adobe Workfront

* [Aprimoramentos de projeto](#project-enhancements)


### Aprimoramentos de projeto

<table>
    <tbody>
        <tr>
            <td><strong>Recurso</strong>
            </td>
            <td><strong>Pré-visualização</strong></td>
            <td><strong>Lançamento rápido</strong></td>
            <td><strong>Trimestralmente</strong></td>
        </tr>
        <tr>
            <td>
                <p><a href="/help/quicksilver/product-announcements/product-releases/27-q1-release-activity/27-q1-projects.md">Fixar threads no início das atualizações</a></p>
                <p>Agora é possível fixar as threads mais importantes na parte superior da área Atualizações em um projeto, tarefa, problema ou solicitação para que as informações principais permaneçam visíveis para a equipe.</p>
            </td>
            <td><p>15 de outubro de 2026</p></td>
            <td><p>12 de novembro de 2026</p></td>
            <td><p>21 de janeiro de 2027</p></td>
        </tr>
    </tbody>
</table>

## Notas de versão para outras áreas

* [Atividade de versão do Adobe Workfront Fusion](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).
* [Atividade de versão do Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

Ainda não há atualizações para o seguinte nesta versão:

* Planejador de cenários
* Proof
* Metas

## Anúncios

### Substituição de campos de taxa de custo e cobrança herdados nas exibições de lista de funções de trabalho

Com o tempo, introduzimos recursos aprimorados de gerenciamento de taxas e experiências dedicadas de Função de trabalho que fornecem uma abordagem mais completa e escalável para manter as informações de taxas. Como resultado, a administração de taxas está migrando para essas experiências dedicadas, em vez de fluxos de trabalho de gerenciamento baseados em lista.

Com a versão de janeiro de 2027, os campos herdados **Faturamento por hora** e **Custo por hora** não estarão mais disponíveis na API do Workfront ou nas exibições de lista de Funções de trabalho, incluindo as configurações Filtro/Exibição/Agrupamento (tanto referências diretas quanto colunas calculadas do modo de texto).

Como substituição nos relatórios, você pode usar o código recomendado do Modo de texto (use `costRates` ou `billingRates` conforme necessário):

    &quot;
    displayname=Test
    listdelimititer=&lt;br>
    listmethod=nested(costRates).lists
    type=iterate
    valueexpression=CONCAT({startDate},&quot; - &quot;,{endDate},&quot;: &quot;,{value})
    valueformat=HTML
    &quot;

Para gerenciar e revisar taxas de funções de trabalho, use as experiências dedicadas de gerenciamento de taxas:

* Acesse e gerencie taxas de funções de trabalho diretamente na página Função do trabalho > Taxas.
* Use Relatórios de Taxa para revisar, analisar e relatar informações de taxa em funções de trabalho.

Nenhuma ação é necessária para se preparar para a alteração. No entanto, os administradores que atualmente exibem os campos **Cobrança por Hora** e **Custo por Hora** nas exibições da lista de Funções de Trabalho devem atualizar seus fluxos de trabalho para usar as experiências de gerenciamento de taxa recomendadas descritas acima.

Para obter informações sobre taxas de funções de trabalho, consulte [Criar e gerenciar funções de trabalho](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

<!--

### Workfront Maintenance Updates

For information about the maintenance updates made during the First Quarter 2027 release, see [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

-->

### Atualizações de treinamento

Explore as últimas atualizações feitas nos programas de aprendizagem, caminhos de aprendizagem, vídeos e guias para cada versão do Adobe Workfront. Para obter mais informações, consulte a seção &quot;Novidades&quot; da [página de tutoriais do Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=pt-BR).
