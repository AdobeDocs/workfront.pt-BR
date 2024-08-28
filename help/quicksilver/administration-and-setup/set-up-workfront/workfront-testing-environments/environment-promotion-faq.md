---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Perguntas frequentes sobre a promoção do ambiente
description: Explore as perguntas frequentes sobre a promoção do ambiente Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e9794262-80cc-4641-a5c6-7130cf008ba2
source-git-commit: 2bbfd449d913a5134c9c36b1ee10567973c56eaa
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 3%

---

# Perguntas frequentes sobre a promoção do ambiente

Perguntas frequentes sobre a promoção do ambiente:

## A promoção entre domínios é permitida?

### Responder

Atualmente, a promoção de ambientes entre domínios não é suportada. Você deve promover entre ambientes no mesmo domínio.

## A plataforma de negócios/IMS do Adobe é um pré-requisito para a promoção do ambiente?

### Responder

Não. A Promoção de ambiente está disponível para instâncias do Workfront habilitadas para IMS e não IMS.

## Como podemos descobrir se nossa instância do Workfront está em uma licença Prime ou Ultimate?

### Responder

* Um administrador do Workfront pode localizar a licença de sua organização.

   1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique no ícone **[!UICONTROL Instalação]** ![Instalação](/help/_includes/assets/gear-icon-setup.png).
   1. Clique em **Sistema** no painel esquerdo
   1. Para exibir seu plano do Workfront, selecione **Licenças**.
Seu plano é exibido próximo ao canto superior direito da página.
      ![](assets/locate-plan.png)

  Ou
* Entre em contato com seu representante de conta da Workfront.

## A promoção do ambiente é bidirecional?

### Responder

Sim. Por exemplo, você pode promover de Sandbox para Produção, ou de Produção para Sandbox.

## O compartilhamento é suportado?

### Responder

Não, não há suporte para compartilhamento no momento.

## Quando um recurso de reversão pode ser disponibilizado?

### Responder

A reversão é uma prioridade e está em desenvolvimento no momento. Esperamos lançar a funcionalidade de reversão no terceiro ou quarto trimestre de 2024.

## Haverá uma opção para ignorar a promoção de componentes individuais? Onde as opções `Use Existing`, `Overwrite` e `Save with a new Name` existem, é possível adicionar `Skip` para que você possa ignorar a promoção de parâmetros individuais?

### Responder


* &quot;Usar existente&quot; é o mesmo que &quot;ignorar&quot; ou ignorar a implantação, pois ela mapeia para o objeto existente no ambiente de destino e não faz alterações.
* Para ignorar objetos, recomendamos remover
todos os objetos que você não deseja instalar diretamente do pacote promocional ou do ambiente de origem. Após remover os objetos, remonte o pacote.
