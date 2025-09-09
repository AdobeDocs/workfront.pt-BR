---
title: Visão geral do campo
description: Você pode adicionar novos campos no Adobe Workfront Planning que reflitam o ciclo de vida de sua organização. Os campos são atributos de tipos de registro.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: 3667359ba2c6ea0aab3ce6845f1a537183f304ec
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 2%

---


# Visão geral do campo

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

Você pode adicionar novos campos no Adobe Workfront Planning que reflitam o ciclo de vida de sua organização. Os campos são atributos de tipos de registro.


## Considerações sobre campos do Adobe Workfront Planning

* Você pode criar campos somente a partir da exibição de tabela de uma página do tipo registro. Os campos são exibidos como colunas na exibição de tabela. Todos os campos associados a um tipo de registro também são exibidos na página de registro.

  Para obter informações sobre como gerenciar colunas de tabela (ou campos de registro), consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md).

  Para obter informações sobre como gerenciar campos, consulte também os seguintes artigos:

   * [Editar configurações de campo](/help/quicksilver/planning/fields/edit-fields.md)
   * [Excluir campos](/help/quicksilver/planning/fields/delete-fields.md)

* Os campos associados a um tipo de registro estão disponíveis para serem associados a todos os registros desse tipo. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* Campos associados a um tipo de registro não podem ser adicionados a outro tipo de registro. <!-- this will change when they open the Field library tab when creating a field-->

* Você pode criar campos manual ou automaticamente das seguintes maneiras:

   * Manualmente:

      * Ao adicionar colunas na exibição de tabela de uma página do tipo registro. As colunas da tabela são os campos associados ao tipo de registro. São os mesmos campos exibidos na página de um registro.

        Não é possível criar campos a partir da página do registro.

      * Ao conectar tipos de registro. É possível criar campos de registro vinculados ao adicionar uma nova conexão entre dois tipos de registro ou um tipo de registro e tipos de objeto de outros aplicativos.

        Para obter mais informações sobre como conectar tipos de registro, consulte [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md).

      * Ao importar campos existentes do Workfront.

        Para obter informações, consulte [Importar campos do Adobe Workfront](/help/quicksilver/planning/fields/import-fields-from-workfront.md).


   * Automaticamente:

      * Ao criar um tipo de registro:

         * Nome
         * Descrição
         * Data de início
         * Data final
         * Status. Os valores padrão para status de registro são:
            * Desenvolvimento
            * Planejado
            * Ativo
            * Concluídos
            * Em Espera

        É possível adicionar mais valores ou renomear os existentes.

      * Ao criar um espaço de trabalho a partir de um modelo.

        Para obter informações, consulte [Criar espaços de trabalho](/help/quicksilver/planning/architecture/create-workspaces.md).

      * Ao importar tipos de registro usando um arquivo Excel ou CSV.

        Para obter mais informações, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

* Os campos do Workfront Planning não podem ser acessados no Workfront.

* Os campos do Workfront podem ser acessados no Workfront Planning somente quando você conecta tipos de registro a tipos de objeto do Workfront e adiciona campos vinculados ou de pesquisa a partir de objetos do Workfront. Para obter informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).

* É possível exibir e atualizar as configurações dos campos criados por você ou por qualquer outro usuário, se você tiver permissões de gerenciamento para o espaço de trabalho e o tipo de registro ao qual o campo pertence.

* É possível ter até 500 campos para um tipo de registro.

* Os nomes de campos podem ter até 250 caracteres.

* Ao excluir um tipo de registro ou espaço de trabalho, todos os campos associados a eles e aos valores dos campos também são excluídos e não podem ser recuperados. <!-- this might change with a possible recycle bin solution?!-->
* Quando você exclui campos que fazem parte de uma expressão de fórmula, o campo de fórmula é alterado.
* Quando você altera uma expressão de fórmula e esse campo de fórmula é referenciado em outros campos de fórmula, as fórmulas adicionais também são afetadas.
