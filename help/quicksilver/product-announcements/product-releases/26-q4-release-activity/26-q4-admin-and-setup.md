---
title: Aprimoramentos do administrador do quarto trimestre de 2026
description: Aprimoramentos do administrador do quarto trimestre de 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 71bd341da0b506429ab25726ae3be82829034f9f
workflow-type: tm+mt
source-wordcount: '832'
ht-degree: 1%

---

# Aprimoramentos do administrador do quarto trimestre de 2026

Esta página descreve as melhorias de Administrador feitas com a versão do Quarto trimestre de 2026 no ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de produção, conforme indicado.

Para obter uma lista de todas as alterações disponíveis neste momento do ciclo de lançamento do quarto trimestre de 2026, consulte [Visão geral da versão do quarto trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

## Os administradores de grupo podem gerenciar perfis empresariais

>[!NOTE]
>
>Visualização: 30 de julho de 2026>Versão rápida de produção: 13 de agosto de 2026>Produção para todos: 15 de outubro de 2026

Os administradores de grupo agora podem criar, editar e excluir perfis de negócios para os grupos que administram, sem exigir acesso de Administrador do sistema. Isso dá às organizações mais flexibilidade para delegar o gerenciamento de perfis empresariais no nível do grupo.

Para obter mais informações, consulte [Exibir e gerenciar perfis comerciais](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-business-profiles.md).

## Suporte a modelo de layout para exibições em listas aprimoradas

>[!NOTE]
>
>Visualização: 30 de julho de 2026>Versão rápida de produção: 13 de agosto de 2026>Produção para todos: 15 de outubro de 2026

As exibições para listas aprimoradas agora são compatíveis no nível do sistema por meio de um modelo de layout. Você pode ocultar exibições do sistema existentes, atribuir uma exibição específica como padrão e adicionar uma exibição personalizada à lista de exibições do sistema.

Exemplos de listas aprimoradas no modelo de layout são **Todas as solicitações** e **Atribuições avançadas**. Uma lista aprimorada tem um rótulo &quot;Nova experiência&quot; ao lado das exibições.

Para obter informações, consulte [Personalizar Filtros, Exibições e Agrupamentos usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Edição em massa de campos de pesquisa externos

>[!NOTE]
>
>Visualização: 30 de julho de 2026>Versão rápida de produção: 13 de agosto de 2026>Produção para todos: 15 de outubro de 2026

As caixas de diálogo de edição em massa agora permitem a edição de campos de pesquisa externos. Isso não era possível anteriormente.

Nas situações em que um campo de pesquisa é dependente de outro campo de pesquisa, o campo com a dependência não pode ser editado em massa, a menos que o primeiro campo seja o mesmo para todos os objetos que estão sendo editados.

Por exemplo, uma lista de países depende da seleção feita para uma região. Se a região de um projeto for a Ásia e a região de outro projeto for a Europa, e você editar ambos os projetos em massa, o campo de país não estará disponível porque as regiões não correspondem. Se você editar a região para que seja a mesma para ambos os projetos, também poderá selecionar um país para usar em ambos os projetos.

Para obter informações sobre campos de pesquisa externos, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-external-lookup-fields).

## Lógica avançada compatível com a pré-visualização do designer de formulário personalizado

>[!NOTE]
>
>Visualização: 30 de julho de 2026>Versão rápida de produção: 13 de agosto de 2026>Produção para todos: 15 de outubro de 2026

O modo de visualização do designer de formulário personalizado agora é compatível com opções lógicas avançadas, incluindo lógica de exibição avançada, lógica de valor padrão, lógica de validação, lógica de formatação e lógica de editabilidade. Você pode testar as fórmulas lógicas na pré-visualização de formulário e ajustá-las conforme necessário no construtor de lógicas. Você também pode selecionar um objeto de teste (projeto, tarefa, problema, etc.) para visualizar o formulário com dados contextuais reais.

Anteriormente, somente as opções básicas de exibição e lógica de salto eram compatíveis com o modo de visualização.

Observe que esses tipos lógicos só estão disponíveis para organizações nos pacotes Prime ou Ultimate do Workflow: exibição avançada, valor padrão, formatação condicional e capacidade de edição.

Para obter mais informações, consulte [Adicionar regras de lógica a formulários e campos personalizados](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md) e [Organizar e visualizar um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).

## Controle de alterações para revisão e aprovação unificadas

>[!NOTE]
>
>Visualização: 30 de julho de 2026>Versão rápida de produção: 13 de agosto de 2026>Produção para todos: 15 de outubro de 2026

A página Histórico de alterações no Workfront agora captura a atividade em fluxos de trabalho unificados de revisão e aprovação, fornecendo aos administradores uma trilha de governança completa para eventos de ciclo de vida de revisão e documento.

Agora, as ações de aprovação, preparo e participante são rastreadas. Essas ações podem incluir:

* Tomada de decisão de aprovação no visualizador Frame.io
* Criação ou exclusão de uma aprovação
* Atualizar um documento, como renomear, mover ou excluí-lo

Cada entrada inclui os campos rastreados padrão: data e hora, operação, nome de usuário (ou &quot;gerado pelo sistema&quot;) e nome do objeto. As atividades do MCP são capturadas, incluindo qual LLM (como Claude) fez a atualização. Os comentários do visualizador Frame.io não estão incluídos.

Para obter mais informações, consulte [Exibir e gerenciar o histórico de alterações](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md).

## Definir um aplicativo personalizado como página de aterrissagem no modelo de layout

>[!NOTE]
>
>Visualização: 30 de julho de 2026>Versão rápida de produção: 13 de agosto de 2026>Produção para todos: 15 de outubro de 2026

Agora é possível definir um aplicativo personalizado como página de aterrissagem em um modelo de layout. Os aplicativos personalizados que já foram adicionados ao menu principal estão disponíveis para uso como uma página de aterrissagem.

Os aplicativos personalizados devem ser criados separadamente antes de serem disponibilizados como Menu principal ou Opções de página de aterrissagem.

Para obter mais informações, consulte [Personalizar a página de aterrissagem usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md) e [Criar aplicativos personalizados para o Workfront com o Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

## Configurar campos rastreados no histórico de alterações

>[!NOTE]
>
>Visualização: 30 de julho de 2026>Versão rápida de produção: 13 de agosto de 2026>Produção para todos: 15 de outubro de 2026

Você pode adicionar campos que deseja rastrear para um tipo específico de objeto em todo o Workfront. Quando os usuários alteram informações nesse campo, o sistema registra informações sobre a alteração como uma entrada no histórico de alterações.

Anteriormente, a tela Configuração para definir os campos rastreados era somente visualização.

Para obter mais informações, consulte [Configurar campos para acompanhar no histórico de alterações](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/configure-fields-in-change-history.md).

## Acesso administrativo ao histórico de alterações adicionado aos níveis de acesso

>[!NOTE]
>
>Visualização: 30 de julho de 2026>Versão rápida de produção: 13 de agosto de 2026>Produção para todos: 15 de outubro de 2026

No nível de acesso Padrão, agora é possível definir se os usuários com esse nível devem ter acesso à Lista do histórico de alterações. A opção **Alterar histórico** está disponível na seção **Permitir acesso administrativo para** no nível de acesso.

Para obter mais informações, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md) e [Exibir e gerenciar o histórico de alterações](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md).


