---
title: Aprimoramentos no Painel e no Relatório do primeiro trimestre de 2025
description: Aprimoramentos no Painel e no Relatório do primeiro trimestre de 2025
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 3c0b4797-594c-44d0-b3ad-a64384b6c4a8
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 14%

---

# Aprimoramentos no Painel e no Relatório do primeiro trimestre de 2025

Esta página descreve todos os aprimoramentos de relatório e painel de controle feitos com a versão do primeiro trimestre de 2025 para o ambiente de Visualização. Essas melhorias serão disponibilizadas no ambiente de produção, conforme indicado.

Para obter uma lista de todas as alterações disponíveis neste momento no ciclo de lançamento do primeiro trimestre de 2025, consulte [Visão geral de lançamentos do primeiro trimestre de 2025](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md).

## Novas entidades disponíveis na Conexão de Dados

>[!NOTE]
>
>Versão prévia: 15 de janeiro de 2025; Versão de produção para todos os clientes: 15 de janeiro de 2025

Adicionamos suporte para as seguintes entidades no Data Connect:

* Usuário da equipe do projeto
* Função de usuário da equipe do projeto
* Horas Orçadas Relatáveis
* Contagem de Estatísticas de Exibição de Relatório
* Gerenciador de Recursos
* Nota em Rich Text

Acrescentamos ainda apoio às seguintes entidades específicas de cada agência:

* Perfis comerciais
* Regra de negócios
* Localização
* Categoria de recurso não trabalhista
* Local do usuário

Para obter mais informações, consulte o [dicionário de dados do Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md).

## Limite de 25 relatórios, páginas externas ou calendários nos painéis

>[!NOTE]
>
>Versão prévia: 16 de dezembro de 2024; Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)

Para manter o desempenho do painel, implementamos um limite para o número total de relatórios, páginas externas ou calendários que podem ser colocados em um painel. Ao criar um novo painel, um máximo de 25 itens pode ser adicionado.

Os painéis de controle existentes que excederem esse limite exibirão um aviso informando que apenas os 25 primeiros itens serão exibidos e, uma vez editado, o painel de controle não poderá ser salvo até que o número de itens incluídos seja reduzido para 25 ou menos.

Para obter mais informações, consulte [Criar um painel](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Botão de criação de conta do leitor de primeira vez para Conexão de Dados

>[!NOTE]
>
>Versão de produção para todos os clientes: 14 de novembro de 2024

Os administradores que acessam o Data Connect pela primeira vez agora recebem a opção de criar uma nova conta do leitor de Snowflake clicando em um único botão. O processo leva alguns minutos para ser concluído, mas não requer nenhuma ação adicional.

Para obter mais informações sobre a configuração da Conexão de Dados, consulte [Criar uma conta de leitor para o Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).
