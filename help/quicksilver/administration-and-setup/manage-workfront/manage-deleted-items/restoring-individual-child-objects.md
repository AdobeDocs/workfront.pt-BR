---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Restauração de objetos filhos individuais
description: Este documento descreve como você pode obter ajuda para recuperar objetos filhos individuais que foram excluídos de seus ambientes de produção ou visualização do Adobe Workfront há menos de 30 dias.
feature: System Setup and Administration
role: Admin
exl-id: e2e4fbb7-5433-4d88-8e36-d82f4cc8a194
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 0%

---

# Restauração de objetos filhos individuais

Este documento descreve como você pode obter ajuda para recuperar objetos filhos individuais que foram excluídos de seus ambientes de produção ou visualização do Adobe Workfront há menos de 30 dias.

Um administrador do Workfront pode restaurar projetos, tarefas, problemas e documentos em cada instância do Workfront, conforme descrito em [Restaurar itens excluídos](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md). Mas somente a Equipe do Banco de Dados do Workfront pode restaurar objetos como tarefas, problemas, documentos, formulários personalizados, horas e notas independentemente do objeto pai.

Os dados do ambiente ativo estão disponíveis na Sandbox de visualização por até 7 dias. Isso significa que você pode exportar os dados independentes do ambiente Preview Sandbox usando os seguintes métodos:

* Início
* Criar um relatório e exportar os resultados

Para obter mais informações sobre como exportar dados do Workfront, consulte [Exportar dados](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

Você pode importar os dados exportados das seguintes maneiras:

* Manualmente, se você estiver usando relatórios exportados
* Em massa, se você estiver usando o Kick-Starts

   Para obter mais informações sobre como importar dados para o Workfront usando o Kick-Starts, consulte [Importar dados para o Adobe Workfront usando um modelo de Início rápido](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

O ambiente Sandbox de visualização é atualizado durante nossas janelas de manutenção durante o fim de semana.

Para obter mais informações sobre as janelas de manutenção do ambiente Preview Sandbox, consulte [trust.workfront.com](https://trust.workfront.com/).

>[!IMPORTANT]
>
>Os documentos constituem uma exceção a estes métodos de restauro. Você pode baixá-los manualmente no Ambiente de visualização e carregá-los novamente no ambiente de produção. Se quiser baixar e carregar documentos em massa, será necessário solicitar uma restauração de dados do Workfront.

## Informações necessárias para uma restauração de dados

Depois de determinar que um objeto excluído precisa ser restaurado pela Equipe do Banco de Dados, reúna quantas informações você tiver sobre ele. As seguintes informações são necessárias para que os administradores de banco de dados encontrem o objeto e iniciem uma restauração:

* Nome do objeto
* Tipo de objeto (tarefa, problema, projeto etc.)
* Data e hora estimadas da exclusão
* GUID do objeto (se possível)

   Consulte as seguintes informações ao localizar o GUID de um objeto:

   * O GUID pode ser encontrado fazendo referência a notificações por email acionadas por interação com o objeto (atribuições, comentários etc.)
   * Exemplo de um GUID encontrado no final de um URL: `yourdomain.my.workfront.com/issue/view?ID=568bfa96011220154c8ca4c4e691556b`

Depois de reunir essas informações ou se precisar de assistência, ligue para nossa equipe de suporte ao cliente em 844-306-HELP(4357) ou envie um ticket online.

## Processo de restauração de dados

1. Depois que a equipe de suporte ao cliente receber suas informações, ela será encaminhada para a equipe de suporte ao cliente.
1. Nossa Equipe de Suporte ao Cliente entrará em contato com a equipe de banco de dados.
1. Depois que a equipe de banco de dados tiver tido a chance de revisar os dados que estão sendo restaurados, poderá ser fornecida uma estimativa mais precisa para o ETA. Uma restauração geralmente leva três dias, mas pode demorar mais dependendo do tipo e do volume de dados que estão sendo restaurados.
1. A Equipe do Banco de Dados restaurará as informações no ambiente Preview Sandbox, onde você terá a chance de revisar os dados restaurados. Nossa equipe de suporte ao cliente informará quando os dados podem ser encontrados na sandbox de visualização.
1. Quando você estiver satisfeito com a restauração na sandbox, informe a nossa Equipe de Suporte ao Cliente e ela entrará em contato com a Equipe de Banco de Dados para notificá-la de que ela pode restaurar os dados para o seu ambiente de produção.
1. Você terá a chance de revisar os dados restaurados antes que a solicitação seja fechada.
