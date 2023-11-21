---
title: Visão geral do campo
description: Você pode adicionar novos campos no Adobe Maestri que refletem o ciclo de vida da sua organização. Os campos são atributos de tipos de registro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 6d1d3d82e15f4232ff81294d9094c2683b01ca89
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 2%

---

# Visão geral do campo

<!--
title: Field overview
description: You can add new fields in Adobe Maestro that reflect your organization's lifecycle. Fields are attributes of record types. 
hidefromtoc: yes
author: Alina
feature: Work Management (***************WE NEED A NEW ONE HERE***********)
role: User, Admin
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>As informações neste artigo referem-se ao Adobe Maestro, que é uma nova oferta da Adobe Workfront.
>
>Atualmente, o Adobe Maestro faz parte de um programa beta aberto a um número limitado de clientes. Você deve ser um cliente do Workfront para usar os recursos do Maestro.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

Você pode adicionar novos campos no Adobe Maestri que refletem o ciclo de vida da sua organização. Os campos são atributos de tipos de registro.


## Considerações sobre campos Maestro

* Você pode criar campos somente a partir da exibição de tabela de uma página do tipo registro. Os campos são exibidos como colunas na exibição de tabela. Todos os campos associados a um tipo de registro também são exibidos na página Detalhes de cada registro desse tipo.

  Para obter informações sobre o gerenciamento de colunas de tabela (ou campos de registro), consulte [Gerenciar a exibição de tabela](../views/manage-the-table-view.md).

  Para obter informações sobre como gerenciar campos, consulte também os seguintes artigos:

   * [Editar campos](../fields/edit-fields.md)
   * [Excluir campos](../fields/delete-fields.md)

* Os campos associados a um tipo de registro estão disponíveis para serem associados a todos os registros desse tipo. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* Campos associados a um tipo de registro não podem ser adicionados a outro tipo de registro. <!-- this will change when they open the Field library tab when creating a field-->

* Você pode criar campos manual ou automaticamente das seguintes maneiras:

   * Manual:

      * Adicionando colunas na visualização Tabela de uma página do tipo registro. As colunas da tabela são os campos associados ao tipo de registro. São os mesmos campos exibidos na página Detalhes de um registro.

        Não é possível criar campos a partir da página Detalhes de um registro.

        Este artigo descreve como criar campos manualmente.

      * Conectando tipos de registro. Você pode criar campos de registro vinculados ao adicionar uma nova conexão entre dois tipos de registro Maestri ou um tipo de registro e tipos de objeto de outras aplicações.

        <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

        Para obter mais informações sobre como conectar tipos de registros Maestri, consulte [Conectar tipos de registro](../architecture/connect-record-types.md).

      * Importando tipos de registro usando um arquivo Excel ou CSV. Para obter mais informações, consulte [Criar tipos de registro](../architecture/create-record-types.md).

   * Automaticamente:

      * Por padrão, sempre que você cria um tipo de registro.

        A seguir estão campos padrão criados por padrão para cada novo tipo de registro operacional:

         * Nome
         * Descrição
         * Data de início
         * Data Final
         * Status. Os valores padrão para status de registro são:
            * Desenvolvimento
            * Planejado
            * Ativo
            * Concluídos
            * Em Espera

           É possível adicionar mais valores ou renomear os existentes.

        A seguir estão os campos padrão criados por padrão para cada novo tipo de registro de taxonomia:

         * Nome <!--will more be added? If not, consider rephrasing this bullet-->

      * Ao criar um espaço de trabalho a partir de um modelo. O Maestri cria campos para tipos de registros operacionais e taxonomias quando você cria um espaço de trabalho a partir de um modelo. Para obter informações, consulte [Criar espaços de trabalho](../architecture/create-workspaces.md).

* Os campos maestro não são acessíveis pela Workfront.

* Os campos do Workfront podem ser acessados pelo Maestro somente quando você conecta tipos de registro do Maestri com tipos de objeto do Workfront e adiciona campos vinculados ou de pesquisa a partir de objetos do Workfront. Para obter informações, consulte [Conectar tipos de registro](../architecture/connect-record-types.md).

* É possível exibir e atualizar as configurações dos campos que você ou qualquer outro usuário criou. <!--this will change with access/ permissions-->

* É possível ter até 500 campos para um tipo de registro.

* Os nomes de campos podem ter até 250 caracteres.

* Ao excluir um tipo de registro operacional, taxonomia ou espaço de trabalho, todos os campos associados a eles e aos valores dos campos também são excluídos e não podem ser recuperados. <!-- this might change with a possible recycle bin solution?!-->