---
title: Melhorias na geração de relatórios no segundo trimestre de 2026
description: Melhorias na geração de relatórios no segundo trimestre de 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4bc2fee9-fa86-41c7-80e7-44bf3e8077d8
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 64ee7798e79324af0ab48af91f49d04d94ece3a9
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 8%

---

# Melhorias na geração de relatórios no segundo trimestre de 2026

Esta página descreve os aprimoramentos de relatórios feitos com a versão do segundo trimestre de 2026 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de produção, conforme indicado.

Para obter uma lista de todas as alterações disponíveis neste momento no ciclo de lançamento do Segundo trimestre de 2026, consulte [Visão geral da versão do Segundo trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Executar relatórios como um usuário específico nos painéis do Canvas

>[!NOTE]
>
>Visualização: 2 de abril de 2026
>Versão rápida de produção: quinta-feira, 15 de abril de 2026
>Produção para todos: sexta-feira, 16 de abril de 2026
>
>Painéis do Canvas atualmente está na versão beta.

Agora é possível configurar relatórios nos painéis do Canvas para serem executados como um usuário específico. Quando ativado, o relatório exibe os dados com base no acesso do usuário selecionado, em vez das permissões do visualizador.

Isso garante dados mais consistentes e confiáveis em visualizadores de painel, mesmo quando o acesso aos espaços de trabalho do Planning, tipos de registro ou configurações de autorização é diferente.

Para obter mais informações, consulte [Criar um relatório de KPI em um Painel da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md), [Criar um relatório de gráfico em um Painel da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md) ou [Criar um relatório de tabela em um Painel da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md).

## A Entrega De Relatório Agendado Agora Aceita Emails Baseados Em Link

>[!NOTE]
>
>Visualização: 2 de abril de 2026
>Versão rápida de produção: quinta-feira, 15 de abril de 2026
>Produção para todos: sexta-feira, 16 de abril de 2026

O Workfront agora inclui um novo tipo de entrega de link para relatórios agendados. Em vez de gerar e anexar um arquivo, essa opção envia um email contendo um link direto para o relatório no Workfront, permitindo que os destinatários visualizem os dados mais atuais no aplicativo.

A opção Vincular agora é o tipo de delivery padrão para regras de delivery de relatórios agendados recém-criadas, enquanto os formatos baseados em arquivos existentes (HTML, PDF, Excel e TSV) permanecem disponíveis.

Com essa alteração, também atualizamos a aparência do email de entrega do relatório.

Para obter mais informações, consulte [Agendar uma entrega automática de relatório](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

## Novas Opções de Autenticação para Conexão de Conexão de Dados

>[!NOTE]
>
>Visualização: 12 de março de 2026
>Versão rápida de produção: sexta-feira, 12 de março de 2026
>Produção para todos: sexta-feira, 16 de abril de 2026

Agora você pode autenticar para a Conexão de dados usando chaves RSA ou conexões de tokens de acesso programático (PAT), adicionando alternativas mais seguras e flexíveis às credenciais tradicionais de nome de usuário/senha.

Essas novas opções permitem que as organizações mantenham conexões estáveis do Power BI, Tableau e outras ferramentas de BI de terceiros sem depender de métodos de logon baseados no usuário.

>[!IMPORTANT]
>
>Em junho de 2026, as credenciais de nome de usuário/senha serão necessárias para usar a autenticação multifator (MFA). Recomendamos a transição para autenticação baseada em RSA ou PAT para contas de usuário de serviço usadas para carregar dados do Data Connect para ferramentas de visualização, processadores de dados e scripts de terceiros que não funcionarão com MFA no processo de autenticação.

## Rótulos de campo personalizados exibidos ao criar relatórios

>[!NOTE]
>
>Visualização: 26 de fevereiro de 2026
>Versão rápida de produção: sexta-feira, 12 de março de 2026
>Produção para todos: sexta-feira, 16 de abril de 2026

O rótulo de campo personalizado agora é exibido antes do nome do campo e do objeto nas ferramentas de criação de relatório, ajudando a localizar campos mais facilmente. Os rótulos de campo também são exibidos ao definir filtros, visualizações e agrupamentos em listas.

O rótulo de campo personalizado destina-se à interface do sistema, enquanto o nome do campo é usado com frequência para fins de API e armazenamento de back-end, e pode não ser tão útil ao localizar um campo.

Para obter mais informações, consulte [Criar um relatório personalizado](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Pastas de Relatórios Compartilháveis

>[!NOTE]
>
>Visualização: 26 de fevereiro de 2026
>Versão rápida de produção: sexta-feira, 12 de março de 2026
>Produção para todos: sexta-feira, 16 de abril de 2026

Agora é possível organizar e compartilhar relatórios usando pastas de relatórios compartilháveis. Esse novo recurso ajuda as equipes que gerenciam grandes volumes de relatórios a manter um controle de acesso escalável e consistente:

* **Criar estruturas de pastas organizadas**: os administradores do sistema podem criar pastas de nível superior, e os usuários com acesso de gerenciamento podem criar subpastas de até quatro níveis de profundidade.
* **Controles de permissão granulares**: compartilhe pastas com dois níveis de permissão:
   * Exibição: os usuários podem abrir relatórios e compartilhar pastas
   * Gerenciar: Os usuários podem editar os detalhes da pasta, adicionar/remover itens e receber automaticamente acesso de gerenciamento a todos os relatórios na pasta
* **Permissões herdadas**: permissões em cascata de pastas pai para todas as subpastas e relatórios dentro da árvore de pastas
* **Experiência de lista aprimorada**: ao habilitar pastas compartilháveis, você terá acesso à experiência de lista aprimorada. Para obter mais informações, consulte [Usar listas aprimoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


Para obter mais informações, consulte [Usar pastas de relatórios compartilháveis](/help/quicksilver/reports-and-dashboards/reports/report-usage/use-sharable-report-folders.md).

## Rótulos de data aprimorados para agrupamentos de gráfico nos painéis da tela de desenho

>[!NOTE]
>
>Visualização: 26 de fevereiro de 2026
>Versão rápida de produção: sexta-feira, 12 de março de 2026
>Produção para todos: sexta-feira, 16 de abril de 2026

>[!NOTE]
>
>Painéis do Canvas atualmente está na versão beta.

Os gráficos que agrupam dados por data agora exibem rótulos de data mais claros e legíveis. Com essa atualização, os rótulos de data se ajustam dinamicamente com base na opção Agrupar por selecionada, como dia, semana, mês ou ano, facilitando a leitura e a interpretação rápida dos gráficos:

<table> <tbody> <tr> <td>Day</td> <td>Exibe a data completa. Exemplo: 12/3/2026</td> </tr> <tr> <td>Semana</td> <td>Exibe uma data de início da semana formatada. Exemplo, 8 de março de 2026</td> </tr> <tr> <td>Month</td> <td>Exibe o mês e o ano. Exemplo em março de 2026</td> </tr> <tr> <td>Year</td> <td>Exibe somente o ano. Exemplo: 2026</td> </tr> </tbody> </table>

Anteriormente, os agrupamentos de gráfico sempre mostravam a data de início do período selecionado em um formato numérico.
