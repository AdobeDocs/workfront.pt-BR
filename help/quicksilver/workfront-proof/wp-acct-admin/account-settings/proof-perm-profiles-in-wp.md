---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Perfis de permissões de prova no Workfront Proof
description: Como administrador do Workfront ou administrador do Workfront Proof, você pode atribuir um Perfil de permissões de prova a um usuário para especificar os recursos de prova que o usuário terá para todas as provas no sistema. Para obter informações sobre como configurar o perfil de permissão de prova de um usuário, consulte Configurar o perfil de permissão de prova de um usuário no Workfront Proof.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 249aa332-c051-49ac-be85-264d8babfcad
source-git-commit: ddaee5b339982c826c14b67775d81f3a2bd7bc37
workflow-type: tm+mt
source-wordcount: '1924'
ht-degree: 0%

---

# Perfis de Permissões de Prova em [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

Como administrador do [!DNL Workfront] ou administrador do [!DNL Workfront Proof], você pode atribuir um Perfil de Permissões de Prova a um usuário para especificar os recursos de prova que o usuário terá para todas as provas no sistema. Para obter informações sobre como configurar o Perfil de Permissão de Prova de um usuário, consulte [Configurar o Perfil de Permissão de Prova de um usuário em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/config-user-pref-in-wp.md).

>[!NOTE]
>
>Você também pode fazer o seguinte:
>
>* Conceda aos usuários funções específicas em provas individuais. Para obter mais informações sobre funções de prova, consulte [Gerenciar funções de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).
>* Crie perfis personalizados para usuários em sua organização. Para obter mais informações, consulte [Configurar perfis personalizados em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).
>

A tabela a seguir exibe as permissões disponíveis com cada Perfil de permissões de prova.

| **Próprios itens** |  |  |  |  | **Itens de Outros Usuários** |  |  | **Administrador** | **Faturamento** |
|---|---|---|---|---|---|---|---|---|---|
|   | **Adicionar** | **Exibir** | **Editar** | **Excluir** | **Exibir** | **Editar** | **Excluir** | **Editar e Excluir** | **Editar** |
| Administrador de Cobrança | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) |
| Admin | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) |   |
| Supervisor | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) |   |   |
| Gerente | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) | ![Marca de seleção](assets/cleaner2.png) |   |   |   |   |   |
| Observador |   | ![Marca de seleção](assets/cleaner2.png) |   |   |   |   |   |   |   |
| Visitante |   | ![Marca de seleção](assets/cleaner2.png) |   |   |   |   |   |   |   |

{style="table-layout:auto"}

Considere o seguinte sobre funções e permissões:

* As permissões de perfil atribuídas se relacionam somente aos usuários e itens em sua própria conta do. A exceção é no caso de contas satélite, em que o administrador e o administrador de faturamento das contas principais (hub) podem acessar e gerenciar as configurações de conta e o faturamento dessas contas do nível da conta de hub.
* Administradores de cobrança e administradores podem excluir usuários. Isso só pode ser feito nas Configurações de conta.
* Quando os Administradores de Faturamento e os Administradores visualizam provas que são de propriedade de outros usuários em suas contas, eles as visualizam com a função de Revisor.
* Usando a função Somente leitura, administradores de faturamento e administradores podem acessar provas em pastas compartilhadas com eles ou em pastas criadas por eles.

As seções a seguir descrevem cada perfil e as permissões associadas ao perfil em uma configuração padrão do [!DNL Workfront Proof]:

* [Administrador de Cobrança](#billing-administrator)
* [Administrador](#administrator)
* [Supervisor](#supervisor)
* [Gerente](#manager)
* [Observador](#observer)
* [Visitante](#visitor)
* [Convidado](#guest)

## Administrador de Cobrança {#billing-administrator}

Os Administradores de Cobrança têm acesso às [configurações da conta em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) and [The [!DNL Workfront Proof] Página de Cobrança](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) e têm as seguintes permissões:

![Marca de seleção](assets/cleaner2.png)Pode gerar provas, carregar arquivos e criar pastas. Para obter mais informações, consulte [Gerar Provas [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Carregar Arquivos e Conteúdo da Web para [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) e [Criar Pastas [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![Marca de seleção](assets/cleaner2.png)Pode exibir, editar e excluir as próprias provas e arquivos que criam.

![Marca de seleção](assets/cleaner2.png)Pode exibir, editar e excluir provas e arquivos criados por todos os usuários na organização.

![Marca de seleção](assets/cleaner2.png)Pode excluir as pastas públicas de outros usuários. Para obter mais informações, consulte [Gerenciar pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![Marca de seleção](assets/cleaner2.png)Tem direitos de edição em todas as provas criadas na conta.

![Marca de seleção](assets/cleaner2.png)Pode ser definida como o proprietário da Dropzone. Para obter mais informações, consulte [Configurar a zona de destino em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![Marca de seleção](assets/cleaner2.png)Pode acessar a página de cobrança e editar os detalhes da cobrança. Para obter mais informações, consulte [A [!DNL Workfront Proof] Página de Faturamento](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

![Marca de seleção](assets/cleaner2.png)Pode acessar a página Configurações da conta e editar os detalhes da conta. Para obter mais informações, consulte [Configurações da conta em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![Marca de seleção](assets/cleaner2.png)Pode esvaziar a lixeira. Para obter mais informações, consulte [Restaurar e esvaziar a Lixeira em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![Marca de seleção](assets/cleaner2.png)Pode adicionar, editar e excluir usuários.

![Marca de seleção](assets/cleaner2.png)Pode criar grupos e adicionar novos contatos.

![Marca de seleção](assets/cleaner2.png)Pode excluir contatos.

![Marca de seleção](assets/cleaner2.png)Pode editar provas se não houver respostas sobre elas.

![X vermelho](assets/no2.png)Não é possível editar respostas de prova.

![X Vermelho](assets/no2.png)Não é possível excluir as pastas particulares de outros Usuários. Para obter mais informações, consulte [Gerenciar pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

Para obter informações sobre configurações de conta, consulte [Configurações de conta em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

Para obter informações sobre cobrança, consulte [A [!DNL Workfront Proof] Página de cobrança](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### Administrador {#administrator}

Administradores têm acesso a [Configurações da conta](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings)e têm as seguintes permissões:

![Marca de seleção](assets/cleaner2.png)Pode criar provas, carregar arquivos e criar pastas. Para obter mais informações, consulte [Gerar Provas [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Carregar Arquivos e Conteúdo da Web para [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) e [Criar Pastas [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![Marca de seleção](assets/cleaner2.png)Pode exibir, editar e excluir provas e arquivos que criaram.

![Marca de seleção](assets/cleaner2.png)Pode exibir, editar e excluir provas e arquivos criados por todos os usuários na organização.

![Marca de seleção](assets/cleaner2.png)Pode excluir as pastas públicas de outros usuários. Para obter mais informações, consulte [Gerenciar pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![Marca de seleção](assets/cleaner2.png)Tem direitos de edição em todas as provas criadas na conta.

![Marca de seleção](assets/cleaner2.png)Pode ser definida como o proprietário da Dropzone. Para obter mais informações, consulte [Configurar a zona de destino em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![Marca de seleção](assets/cleaner2.png)Pode acessar a página Configurações da conta e editar os detalhes da conta. Para obter mais informações, consulte [Configurações da conta em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![Marca de seleção](assets/cleaner2.png)Pode esvaziar a lixeira. Para obter mais informações, consulte [Restaurar e esvaziar a Lixeira em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![Marca de seleção](assets/cleaner2.png)Pode adicionar, editar e excluir usuários.

![Marca de seleção](assets/cleaner2.png)Pode criar grupos e adicionar novos contatos.

![Marca de seleção](assets/cleaner2.png)Pode excluir contatos.

![Marca de seleção](assets/cleaner2.png)Pode editar provas se não houver respostas sobre elas.

![X vermelho](assets/no2.png)Não é possível editar respostas de prova.

![X Vermelho](assets/no2.png)Não é possível excluir as pastas particulares de outros Usuários. Para obter mais informações, consulte [Gerenciar pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![X Vermelho](assets/no2.png)Não é possível acessar a página Cobrança ou editar os detalhes de cobrança. Para obter mais informações, consulte [A [!DNL Workfront Proof] Página de Faturamento](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### Supervisor {#supervisor}

Os supervisores têm as seguintes permissões:

![Marca de seleção](assets/cleaner2.png)Pode criar provas, carregar arquivos e criar pastas. Para obter mais informações, consulte [Gerar Provas [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Carregar Arquivos e Conteúdo da Web para [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) e [Criar Pastas [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![Marca de seleção](assets/cleaner2.png)Pode exibir, editar e excluir as próprias provas e arquivos que criaram.

![Marca de seleção](assets/cleaner2.png)Pode exibir, editar e excluir provas e arquivos criados por todos os usuários na organização.

![Marca de seleção](assets/cleaner2.png)Pode excluir as pastas públicas de outros usuários. Para obter mais informações, consulte [Gerenciar pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![Marca de seleção](assets/cleaner2.png)Tem direitos de edição em todas as provas criadas na conta.

![Marca de seleção](assets/cleaner2.png)Pode ser definida como o proprietário da Dropzone. Para obter mais informações, consulte [Configurar a zona de destino em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![Marca de seleção](assets/cleaner2.png)Pode criar grupos e adicionar novos contatos.

![Marca de seleção](assets/cleaner2.png)Pode excluir contatos.

![Marca de seleção](assets/cleaner2.png)Pode editar provas se não houver respostas sobre elas.

![X vermelho](assets/no2.png)Não é possível editar respostas de prova.

![X Vermelho](assets/no2.png)Não é possível excluir as pastas particulares de outros Usuários. Para obter mais informações, consulte [Pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/folders.md).

![X Vermelho](assets/no2.png)Não é possível acessar a página de Faturamento ou as configurações de Conta. Para obter mais informações, consulte [A [!DNL Workfront Proof] Página de Faturamento](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) e [Configurações de conta em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![X Vermelho](assets/no2.png)Não é possível adicionar, editar ou excluir usuários.

![X Vermelho](assets/no2.png)Não é possível esvaziar a lixeira. Para obter mais informações, consulte [Restaurar e esvaziar a Lixeira em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

### Gerente {#manager}

Os gerentes têm as seguintes permissões:

![Marca de seleção](assets/cleaner2.png)Pode criar provas, carregar arquivos e criar pastas. Para obter mais informações, consulte [Gerar Provas [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Carregar Arquivos e Conteúdo da Web para [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) e [Criar Pastas [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![Marca de seleção](assets/cleaner2.png)Pode exibir, editar e excluir suas próprias provas e seus arquivos.

![Marca de seleção](assets/cleaner2.png)Pode ver, revisar e aprovar provas de outros usuários que estejam compartilhados explicitamente com eles (direitos somente leitura para tudo em uma pasta compartilhada). Para obter mais informações, consulte [Gerenciar funções de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![Marca de seleção](assets/cleaner2.png)Pode criar grupos e adicionar um novo contato.

![X vermelho](assets/no2.png)Não é possível exibir, editar ou excluir provas e arquivos criados por outros usuários na organização.

![X vermelho](assets/no2.png)Não é possível editar provas ou respostas.

![X Vermelho](assets/no2.png)Não é possível excluir as pastas particulares de outros Usuários. Para obter mais informações, consulte [Gerenciar pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![X Vermelho](assets/no2.png)Não é possível excluir as pastas públicas de outros Usuários. Para obter mais informações, consulte [Gerenciar pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![X Vermelho](assets/no2.png)Não é possível acessar a página de Faturamento ou as configurações de Conta. Para obter mais informações, consulte [A [!DNL Workfront Proof] Página de Faturamento](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) e [Configurações de conta em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![X Vermelho](assets/no2.png)Não pode ser definido como o proprietário da Dropzone. Para obter mais informações, consulte [Configurar a zona de destino em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![X Vermelho](assets/no2.png)Não é possível esvaziar a lixeira. Para obter mais informações, consulte [Restaurar e esvaziar a Lixeira em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![X Vermelho](assets/no2.png)Não é possível adicionar, editar ou excluir usuários.

![X Vermelho](assets/no2.png)Não é possível excluir contatos.

### Observador {#observer}

Os observadores têm as seguintes permissões:

![Marca de seleção](assets/cleaner2.png)Pode ver, revisar e aprovar provas de outros usuários que estão explicitamente compartilhados com eles (direitos somente leitura para tudo em uma pasta compartilhada). Para obter mais informações, consulte [Gerenciar funções de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![Marca de seleção](assets/cleaner2.png)Pode exibir arquivos compartilhados explicitamente com eles.

![Marca de seleção](assets/cleaner2.png) Pode exibir contatos e grupos

![X vermelho](assets/no2.png)Não é possível criar provas, carregar arquivos e criar pastas. Para obter mais informações, consulte [Fazer upload de arquivos e conteúdo da Web para [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![X vermelho](assets/no2.png)Não é possível exibir, editar ou excluir provas e arquivos criados por outros usuários na organização.

![X vermelho](assets/no2.png)Não é possível editar provas ou respostas.

![X Vermelho](assets/no2.png)Não é possível excluir itens criados na organização.

![X Vermelho](assets/no2.png)Não é possível acessar a página de Faturamento ou as configurações de Conta. Para obter mais informações, consulte [A [!DNL Workfront Proof] Página de Faturamento](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) e [Configurações de conta em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![X Vermelho](assets/no2.png)Não pode ser definido como o proprietário da Dropzone. Para obter mais informações, consulte [Configurar a zona de destino em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![X Vermelho](assets/no2.png)Não é possível esvaziar a lixeira. Para obter mais informações, consulte [Restaurar e esvaziar a Lixeira em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![X Vermelho](assets/no2.png)Não é possível adicionar, editar ou excluir usuários.

![X Vermelho](assets/no2.png)Não é possível criar grupos ou adicionar novos contatos.

![X Vermelho](assets/no2.png)Não é possível excluir contatos.

>[!NOTE]
>
>Os menus e as funções disponíveis para os Observadores são limitados.
>
>* Os observadores não veem o menu Cabeçalho ou o menu Novo verde em seus painéis
>* Os observadores não veem os seguintes links em suas Configurações: Configurações da conta, Faturamento
>

### Visitante {#visitor}

Os visitantes têm as seguintes permissões:

![Marca de seleção](assets/cleaner2.png)Pode ver, revisar e aprovar provas de outros usuários que estejam compartilhados explicitamente com eles (direitos somente leitura para tudo em uma pasta compartilhada). Para obter mais informações, consulte [Gerenciar funções de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![Marca de seleção](assets/cleaner2.png)Pode exibir arquivos compartilhados explicitamente com eles.

![X Vermelho](assets/no2.png) Não é possível exibir contatos e grupos

![X vermelho](assets/no2.png)Não é possível criar provas, carregar arquivos e criar pastas. Para obter mais informações, consulte [Fazer upload de arquivos e conteúdo da Web para [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![X vermelho](assets/no2.png)Não é possível exibir, editar ou excluir provas e arquivos criados por outros usuários na organização.

![X vermelho](assets/no2.png)Não é possível editar provas ou respostas.

![X Vermelho](assets/no2.png)Não é possível excluir itens criados na organização.

![X Vermelho](assets/no2.png)Não é possível acessar a página de Faturamento ou as configurações de Conta. Para obter mais informações, consulte [A [!DNL Workfront Proof] Página de Faturamento](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) e [Configurações de conta em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![X Vermelho](assets/no2.png)Não pode ser definido como o proprietário da Dropzone. Para obter mais informações, consulte [Configurar a zona de destino em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![X Vermelho](assets/no2.png)Não é possível esvaziar a lixeira. Para obter mais informações, consulte [Restaurar e esvaziar a Lixeira em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![X Vermelho](assets/no2.png)Não é possível adicionar, editar ou excluir usuários.

![X Vermelho](assets/no2.png)Não é possível criar grupos ou adicionar novos contatos.

![X Vermelho](assets/no2.png)Não é possível excluir contatos.

>[!NOTE]
>
>Os menus e funções disponíveis para os visitantes são limitados.
>
>* Os visitantes não veem o menu Cabeçalho ou o menu Novo verde em seu Painel
>* Os visitantes não veem os seguintes links em suas Configurações: Configurações da conta, Faturamento
>

### Convidado {#guest}

O perfil Convidado é usado para conceder acesso a provas para revisores que não têm sua própria conta do Workfront Proof. Os visitantes podem acessar provas compartilhadas diretamente com eles por meio de suas notificações pessoais por email.

![Marca de seleção](assets/cleaner2.png)Pode exibir, revisar e aprovar provas que são compartilhadas explicitamente com elas.

![Marca de seleção](assets/cleaner2.png)Pode exibir arquivos compartilhados explicitamente com eles.

![X Vermelho](assets/no2.png)Não é possível acessar o Painel.

![X Vermelho](assets/no2.png)Não é possível ter pastas compartilhadas com ele. Para obter mais informações, consulte [Gerenciar pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![X vermelho](assets/no2.png)Não pode ser adicionado como autores ou moderadores nas provas. Para obter mais informações, consulte [Gerenciar funções de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

>[!NOTE]
>
>Os convidados não são usuários do Workfront Proof, portanto, não podem ver todas as provas compartilhadas com eles em seu próprio Painel.

## Editar o perfil de permissão de prova de um usuário

Os administradores e os administradores de cobrança podem editar os perfis de permissão de todos os usuários na conta.

1. Para localizar o usuário a ser editado, siga um destes procedimentos:

   * Navegue até **[!UICONTROL Configurações da conta]** e clique na guia **[!UICONTROL Usuários]**.

   * Vá para a página **[!UICONTROL Contatos]**.

1. Clique no nome do usuário cujas permissões você deseja editar. ![Selecionar usuário](assets/screenshot-2018-03-30-14-16-05a-350x69.png)

1. Clique no menu suspenso **[!UICONTROL Perfil de permissões]** e selecione um novo perfil de permissão. :

   ![Perfil de permissões](assets/screenshot-2018-03-30-14-18-03a.png)

   Os perfis de permissão são Administrador, Supervisor, Gerente e Observador.

1. Clique em qualquer lugar fora do menu para salvar.

>[!NOTE]
>
>Os administradores não podem atribuir o perfil de administrador de cobrança. Você pode encontrar uma lista de alterações de perfil nos seguintes logs:
>
>* Os logs de atividade da conta
>* O log de perfil do usuário (acessível somente a esse usuário)
>

Para obter mais informações sobre logs de atividades, consulte [Noções básicas sobre a [!DNL Workfront Proof] Trilha de Auditoria de Atividades](../../../workfront-proof/wp-work-proofsfiles/basic-features/activity-audit-trail.md).
