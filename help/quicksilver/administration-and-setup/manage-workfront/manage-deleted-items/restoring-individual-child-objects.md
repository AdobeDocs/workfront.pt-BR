---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Restauração de objetos filho individuais
description: Este documento descreve como obter ajuda para recuperar objetos secundários individuais que foram excluídos dos ambientes de produção ou pré-visualização do Adobe Workfront menos de 30 dias antes.
feature: System Setup and Administration
role: Admin
exl-id: e2e4fbb7-5433-4d88-8e36-d82f4cc8a194
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 0%

---

# Restauração de objetos filho individuais

Este documento descreve como obter ajuda para recuperar objetos secundários individuais que foram excluídos dos ambientes de produção ou pré-visualização do Adobe Workfront menos de 30 dias antes.

Um administrador do Workfront pode restaurar projetos, tarefas, problemas e documentos em cada instância do Workfront, conforme descrito em [Restaurar itens excluídos](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md). Mas somente a Equipe de banco de dados do Workfront pode restaurar objetos como tarefas, problemas, documentos, formulários personalizados, horas e observações, independentemente do objeto principal.

Os dados de seu ambiente ativo estão disponíveis na sandbox de visualização por até 7 dias. Isso significa que você pode exportar os dados independentes do ambiente Visualizar sandbox usando os seguintes métodos:

* Início
* Criação de um relatório e exportação de resultados

Para obter mais informações sobre como exportar dados do Workfront, consulte [Exportar dados](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

Você pode importar os dados exportados das seguintes maneiras:

* Manualmente, se você estiver usando relatórios exportados
* Em massa, se você estiver usando o Kick-Starts

  Para obter mais informações sobre como importar dados para o Workfront usando o Kick-Starts, consulte [Importar dados para o Adobe Workfront usando um modelo de Kick-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

O ambiente de Visualização da sandbox é atualizado durante nossas janelas de manutenção durante o fim de semana.

Para obter mais informações sobre as janelas de manutenção do ambiente de Pré-visualização da Sandbox, consulte [o site de status do Adobe](https://status.adobe.com/pt).

>[!IMPORTANT]
>
>Os documentos são uma exceção a esses métodos de restauração. Você pode baixá-los manualmente no Ambiente de visualização e fazer upload deles novamente no ambiente de produção. Se você deseja baixar e carregar documentos em massa, será necessário solicitar uma restauração de dados da Workfront.

## Informações necessárias para uma restauração de dados

Depois de determinar que um objeto excluído precisa ser restaurado pela Equipe do banco de dados, colete o máximo de informações possível sobre ele. As seguintes informações são necessárias para que os administradores de banco de dados localizem o objeto e iniciem uma restauração:

* Nome do objeto
* Tipo de objeto (tarefa, problema, projeto etc.)
* Data e hora estimadas da exclusão
* GUID do objeto (se possível)

  Consulte as seguintes informações ao localizar o GUID de um objeto:

   * O GUID pode ser encontrado referenciando notificações por email acionadas pela interação com o objeto (atribuições, comentários, etc.)
   * Exemplo de GUID encontrado no final de uma URL: `yourdomain.my.workfront.com/issue/view?ID=568bfa96011220154c8ca4c4e691556b`

Depois de obter essas informações ou se precisar de assistência, ligue para nossa Equipe de suporte ao cliente pelo telefone 844-306-HELP(4357) ou envie um tíquete online.

## Processo de restauração de dados

1. Depois que nossa Equipe de suporte ao cliente receber suas informações, ela as encaminhará para nossa Equipe de suporte ao cliente.
1. Nossa equipe de suporte ao cliente entrará em contato com nossa equipe de banco de dados.
1. Depois que a equipe do banco de dados tiver tido a chance de revisar os dados que estão sendo restaurados, uma estimativa mais precisa para o ETA pode ser fornecida. Uma restauração geralmente leva três dias, mas pode demorar mais, dependendo do tipo e do volume de dados que está sendo restaurado.
1. A equipe do banco de dados restaurará as informações para o ambiente de Pré-visualização da sandbox, onde você terá a chance de revisar os dados restaurados. Nossa equipe de suporte ao cliente informará quando os dados poderão ser encontrados na sandbox de visualização.
1. Quando estiver satisfeito com a restauração na sandbox, informe à nossa Equipe de suporte ao cliente que eles entrarão em contato com nossa Equipe de banco de dados para notificá-los de que podem restaurar os dados para o ambiente de produção.
1. Você terá a chance de revisar os dados restaurados antes de fechar a solicitação.
