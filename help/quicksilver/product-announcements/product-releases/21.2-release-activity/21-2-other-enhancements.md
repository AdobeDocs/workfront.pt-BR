---
content-type: release-notes
keywords: notas,trimestral,atualização,versão
navigation-topic: 2021-2-release-activity
title: 21.2 Outras melhorias
description: Esta página descreve todas as Outras melhorias feitas com a versão 21.2 para o ambiente de Visualização. Esses aprimoramentos serão disponibilizados no ambiente de produção na semana de 10 de maio de 2021. Para obter uma lista de todas as alterações disponíveis com a versão 21.2, consulte Visão geral da versão 21.2.
author: Luke
feature: Product Announcements
exl-id: f136c08b-63c0-4e1e-a048-09eb84a0ed54
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 21.2 Outras melhorias

Esta página descreve todas as Outras melhorias feitas com a versão 21.2 para o ambiente de Visualização. Esses aprimoramentos serão disponibilizados no ambiente de produção na semana de 10 de maio de 2021. Para obter uma lista de todas as alterações disponíveis com a versão 21.2, consulte [Visão geral da versão 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Agora somos oficialmente Adobe Workfront

A Workfront foi renomeada para Adobe Workfront.

As áreas mais importantes no aplicativo Adobe Workfront e em nossos sites voltados para o cliente foram atualizadas. Outras áreas serão atualizadas em breve.

**Áreas atualizadas**

* Tela de logon, navegação superior, prova
* Interface do usuário de modelos de layout, Menu principal, Exportação personalizada do Forms (disponível somente na nova experiência do Adobe Workfront)
* Aplicativo móvel Workfront (iOS e Android)

Áreas em breve

* Aplicativos de prova para desktop e dispositivos móveis
* Exportações de PDF para listas e relatórios
* Ícone Favicon na guia do navegador

**Áreas atualizadas posteriormente**

* Notificações de email

## Validação da  de lista de permissões de email

>[!NOTE]
>
>Disponível somente na nova experiência do Adobe Workfront.

Se você usar a  de lista de permissões de email, os endereços de email de usuário novos e atualizados agora serão validados em relação à lista de permissões. Ao adicionar um novo usuário ou editar um usuário existente e inserir um domínio de email que não esteja na lista de permissões, uma mensagem notifica você que o usuário não receberá mensagens de email. Você ainda pode salvar o perfil do usuário, mas deve adicionar o domínio à  de lista de permissões para que o usuário receba emails.

Para obter mais informações, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Nova aparência para cabeçalhos de objetos

>[!NOTE]
>
>Esse recurso foi lançado no ambiente de produção em 10 de março de 2020.
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Para reforçar ainda mais a hierarquia de informações e ajudar os usuários a entender mais claramente em que página estão, cada cabeçalho de objeto agora tem:

* Ícones coloridos e mais modernos para cada tipo de objeto
* O tipo de objeto listado acima do nome do objeto
* Um estilo de fonte e tamanho de texto atualizados
* Outras alterações de estilo menores

Anteriormente, não havia nenhum ícone e um selo com o nome do objeto aparecia à direita do título do objeto.

Os cabeçalhos de página de áreas na nova experiência do Workfront, como Análise aprimorada, Gerenciamento de recursos e outras, também têm essa aparência atualizada.

Para saber mais sobre os novos cabeçalhos de objetos na nova experiência do Workfront, consulte [Novos cabeçalhos de objeto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

![](assets/product-announcement-object-header-350x179.png)

## Atualizações das respostas de pesquisa do status do objeto

O Workfront agora armazena os status de objetos de uma nova maneira.

Essas alterações não afetam como as solicitações de pesquisa de status são feitas. No entanto, as solicitações de API que contêm uma pesquisa de status de objeto retornarão uma lista incompleta de status de grupo.

Para obter mais informações, consulte [Alterações na API principal: Respostas de pesquisa de status](../../../wf-api/api/api-changes-search.md) .

## Cargas de assinatura do evento atualizadas para incluir todos os campos que terminam na ID

Todas as cargas de assinatura do evento agora contêm todos os campos que terminam em &quot;ID&quot;.

É importante observar que cada objeto tem seu próprio conjunto exclusivo de campos associados, que inclui um conjunto exclusivo de campos associados que terminam na ID. Isso significa que, embora cada carga contenha todos os campos associados desse objeto que terminam em ID, cada objeto tem um conjunto diferente de campos que terminam em ID.

## Beta de blueprints agora disponível na Visualização

>[!NOTE]
>
>Essa funcionalidade não estará disponível no ambiente de Produção até a versão 21.3, no final deste ano. Disponível somente na nova experiência do Adobe Workfront.

O Blueprints fornece blocos básicos para ajudá-lo a criar um sistema de gerenciamento de trabalho que cresce com você. Os administradores de sistema podem navegar pelo catálogo de blueprints e instalar modelos de projeto prontos para uso.

Para obter mais informações, consulte [Blueprints](../../../administration-and-setup/blueprints/blueprints.md).
