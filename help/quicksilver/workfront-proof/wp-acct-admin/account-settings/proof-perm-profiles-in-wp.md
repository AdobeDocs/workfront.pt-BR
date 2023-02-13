---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Perfis de permissões de prova na Workfront Proof
description: Como administrador do Workfront ou administrador da Workfront Proof, você pode atribuir um Perfil de Permissões de Prova a um usuário para especificar os recursos de prova que o usuário terá para todas as provas no sistema. Para obter informações sobre como configurar o Perfil de permissão de prova de um usuário, consulte Configurar o perfil de permissão de prova de um usuário na Workfront Proof .
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 249aa332-c051-49ac-be85-264d8babfcad
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '1769'
ht-degree: 1%

---

# Perfis de prova de permissões em [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

Como um [!DNL Workfront] administrador ou [!DNL Workfront Proof] administrador, é possível atribuir um Perfil de permissões de prova a um usuário para especificar os recursos de prova que o usuário terá para todas as provas no sistema. Para obter informações sobre como configurar o Perfil de Permissão de Prova de um usuário, consulte [Configure o Perfil de permissão de prova do usuário em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/config-user-pref-in-wp.md).

>[!NOTE]
>
>Você também pode fazer o seguinte:
>
>* Conceda aos usuários funções específicas em provas individuais. Para obter mais informações sobre funções de prova, consulte [Gerenciar funções de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).
>* Crie perfis personalizados para usuários em sua organização. Para obter mais informações, consulte [Configurar perfis personalizados em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).
>


A tabela a seguir exibe as permissões disponíveis com cada Perfil de permissões de prova.

| **Itens próprios** |  |  |  |  | **Itens de outros usuários** |  |  | **Admin** | **Faturamento** |
|---|---|---|---|---|---|---|---|---|---|
|  | **Adicionar** | **Exibir** | **Editar** | **Excluir** | **Exibir** | **Editar** | **Excluir** | **Editar e excluir** | **Editar** |
| Administrador de faturamento | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |
| Admin | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |
| Supervisor | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |
| Gerente | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |   |   |   |
| Observador |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |
| Visitante |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

Considere o seguinte sobre funções e permissões:

* As permissões de perfil atribuídas se relacionam somente aos usuários e itens em sua própria conta. A exceção é no caso das contas Satélite, em que o Administrador e o Administrador de Faturamento das contas principais (hub) podem acessar e gerenciar as configurações da conta e o faturamento dessas contas a partir do nível da conta do hub.
* Os administradores e administradores de faturamento podem excluir usuários. Isso só pode ser feito nas configurações da conta.
* Ao faturar administradores e administradores exibem provas de propriedade de outros usuários em suas contas, eles as visualizam com a função de um revisor.
* Usando a função Somente leitura, os Administradores e Administradores de Faturamento podem acessar provas em pastas compartilhadas com eles ou em pastas criadas por eles.

As seções a seguir descrevem cada perfil e as permissões associadas ao perfil em um padrão [!DNL Workfront Proof] configuração:

* [Administrador de Faturamento](#billing-administrator)
* [Administrador](#administrator)
* [Supervisor](#supervisor)
* [Gerente](#manager)
* [Observador](#observer)
* [Visitante](#visitor)
* [Convidado](#guest)

## Administrador de Faturamento {#billing-administrator}

Os administradores de faturamento têm acesso a [Configurações da conta em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) and [The [!DNL Workfront Proof] Página de Faturamento](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)e ter as seguintes permissões:

![](assets/cleaner2.png)Pode gerar provas, carregar arquivos e criar pastas. Para obter mais informações, consulte [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Fazer upload de arquivos e conteúdo da Web para [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)e [Criar pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Pode exibir, editar e excluir provas e arquivos criados por elas.

![](assets/cleaner2.png)Pode exibir, editar e excluir provas e arquivos criados por todos os usuários na organização.

![](assets/cleaner2.png)Pode excluir as pastas públicas de outros usuários. Para obter mais informações, consulte [Gerenciar pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Tem direitos de edição em todas as provas criadas na conta.

![](assets/cleaner2.png)Pode ser definido como o proprietário da zona de transferência. Para obter mais informações, consulte [Configure a área suspensa em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Pode acessar a página de faturamento e editar os detalhes de faturamento. Para obter mais informações, consulte [O [!DNL Workfront Proof] Página de Faturamento](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

![](assets/cleaner2.png)Pode acessar a página Configurações da conta e editar os detalhes da conta. Para obter mais informações, consulte [Configurações da conta em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)Pode esvaziar o lixo. Para obter mais informações, consulte [Restaure e esvazie a lixeira no [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)Pode adicionar, editar e excluir usuários.

![](assets/cleaner2.png)Pode criar grupos e adicionar novos contatos.

![](assets/cleaner2.png)Pode excluir contatos.

![](assets/cleaner2.png)Pode editar provas se não houver respostas.

![](assets/no2.png)Não é possível editar respostas de prova.

![](assets/no2.png)Não é possível excluir as pastas privadas de outros Usuários. Para obter mais informações, consulte [Gerenciar pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

Para obter informações sobre as configurações da conta, consulte [Configurações da conta em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

Para obter informações sobre Faturamento, consulte [O [!DNL Workfront Proof] Página de Faturamento](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### Administrador {#administrator}

Os administradores têm acesso ao [Configurações da conta](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings)e ter as seguintes permissões:

![](assets/cleaner2.png)Pode criar provas, carregar arquivos e criar pastas. Para obter mais informações, consulte [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Fazer upload de arquivos e conteúdo da Web para [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)e [Criar pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Pode exibir, editar e excluir provas e arquivos que eles criaram.

![](assets/cleaner2.png)Pode exibir, editar e excluir provas e arquivos criados por todos os usuários na organização.

![](assets/cleaner2.png)Pode excluir as pastas públicas de outros usuários. Para obter mais informações, consulte [Gerenciar pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Tem direitos de edição em todas as provas criadas na conta.

![](assets/cleaner2.png)Pode ser definido como o proprietário da zona de transferência. Para obter mais informações, consulte [Configure a área suspensa em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Pode acessar a página Configurações da conta e editar os detalhes da conta. Para obter mais informações, consulte [Configurações da conta em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)Pode esvaziar o lixo. Para obter mais informações, consulte [Restaure e esvazie a lixeira no [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)Pode adicionar, editar e excluir usuários.

![](assets/cleaner2.png)Pode criar grupos e adicionar novos contatos.

![](assets/cleaner2.png)Pode excluir contatos.

![](assets/cleaner2.png)Pode editar provas se não houver respostas.

![](assets/no2.png)Não é possível editar respostas de prova.

![](assets/no2.png)Não é possível excluir as pastas privadas de outros Usuários. Para obter mais informações, consulte [Gerenciar pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Não é possível acessar a página Faturamento ou editar os detalhes de faturamento. Para obter mais informações, consulte [O [!DNL Workfront Proof] Página de Faturamento](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### Supervisor {#supervisor}

Os supervisores têm as seguintes permissões:

![](assets/cleaner2.png)Pode criar provas, carregar arquivos e criar pastas. Para obter mais informações, consulte [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Fazer upload de arquivos e conteúdo da Web para [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)e [Criar pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Podem exibir, editar e excluir provas e arquivos criados.

![](assets/cleaner2.png)Pode exibir, editar e excluir provas e arquivos criados por todos os usuários na organização.

![](assets/cleaner2.png)Pode excluir as pastas públicas de outros usuários. Para obter mais informações, consulte [Gerenciar pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Tem direitos de edição em todas as provas criadas na conta.

![](assets/cleaner2.png)Pode ser definido como o proprietário da zona de transferência. Para obter mais informações, consulte [Configure a área suspensa em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Pode criar grupos e adicionar novos contatos.

![](assets/cleaner2.png)Pode excluir contatos.

![](assets/cleaner2.png)Pode editar provas se não houver respostas.

![](assets/no2.png)Não é possível editar respostas de prova.

![](assets/no2.png)Não é possível excluir as pastas privadas de outros Usuários. Para obter mais informações, consulte [Pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/folders.md).

![](assets/no2.png)Não é possível acessar a página Faturamento ou as configurações da Conta. Para obter mais informações, consulte [O [!DNL Workfront Proof] Página de Faturamento](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) e [Configurações da conta em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Não é possível adicionar, editar ou excluir usuários.

![](assets/no2.png)Não é possível esvaziar a lixeira. Para obter mais informações, consulte [Restaure e esvazie a lixeira no [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

### Gerente {#manager}

Os gerentes têm as seguintes permissões:

![](assets/cleaner2.png)Pode criar provas, carregar arquivos e criar pastas. Para obter mais informações, consulte [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Fazer upload de arquivos e conteúdo da Web para [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)e [Criar pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Pode exibir, editar e excluir suas próprias provas e arquivos que eles criam ou possuem.

![](assets/cleaner2.png)Pode ver, revisar e aprovar provas de outros usuários que são compartilhados explicitamente com eles (direitos somente leitura para tudo em uma pasta compartilhada). Para obter mais informações, consulte [Gerenciar funções de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Pode criar grupos e adicionar um novo contato.

![](assets/no2.png)Não é possível exibir, editar ou excluir provas e arquivos criados por outros usuários na organização.

![](assets/no2.png)Não é possível editar provas ou respostas.

![](assets/no2.png)Não é possível excluir as pastas privadas de outros Usuários. Para obter mais informações, consulte [Gerenciar pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Não é possível excluir as pastas públicas de outros usuários. Para obter mais informações, consulte [Gerenciar pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Não é possível acessar a página Faturamento ou as configurações da Conta. Para obter mais informações, consulte [O [!DNL Workfront Proof] Página de Faturamento](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) e [Configurações da conta em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Não pode ser definido como o proprietário do Dropzone. Para obter mais informações, consulte [Configure a área suspensa em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Não é possível esvaziar a lixeira. Para obter mais informações, consulte [Restaure e esvazie a lixeira no [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Não é possível adicionar, editar ou excluir usuários.

![](assets/no2.png)Não é possível excluir contatos.

### Observador {#observer}

Os observadores têm as seguintes permissões:

![](assets/cleaner2.png)Pode ver, revisar e aprovar provas de outros usuários que são compartilhados explicitamente com eles (direitos somente leitura para tudo em uma pasta compartilhada). Para obter mais informações, consulte [Gerenciar funções de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Pode exibir arquivos que são compartilhados explicitamente com eles.

![](assets/cleaner2.png) Pode visualizar contatos e grupos

![](assets/no2.png)Não é possível criar provas, carregar ficheiros e criar pastas. Para obter mais informações, consulte [Fazer upload de arquivos e conteúdo da Web para [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)Não é possível exibir, editar ou excluir provas e arquivos criados por outros usuários na organização.

![](assets/no2.png)Não é possível editar provas ou respostas.

![](assets/no2.png)Não é possível excluir nenhum item criado na organização.

![](assets/no2.png)Não é possível acessar a página Faturamento ou as configurações da Conta. Para obter mais informações, consulte [O [!DNL Workfront Proof] Página de Faturamento](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) e [Configurações da conta em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Não pode ser definido como o proprietário do Dropzone. Para obter mais informações, consulte [Configure a área suspensa em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Não é possível esvaziar a lixeira. Para obter mais informações, consulte [Restaure e esvazie a lixeira no [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Não é possível adicionar, editar ou excluir usuários.

![](assets/no2.png)Não é possível criar grupos ou adicionar novos contatos.

![](assets/no2.png)Não é possível excluir contatos.

>[!NOTE]
>
>Os menus e as funções disponíveis para os Observadores são limitados.
>
>* Os observadores não visualizam o menu Cabeçalho ou o menu verde Novo no painel
>* Os observadores não veem os seguintes links em suas Configurações: Configurações da conta, Faturamento
>


### Visitante {#visitor}

Os visitantes têm as seguintes permissões:

![](assets/cleaner2.png)Pode ver, revisar e aprovar provas de outros usuários que são compartilhados explicitamente com eles (direitos somente leitura para tudo em uma pasta compartilhada). Para obter mais informações, consulte [Gerenciar funções de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Pode exibir arquivos que são compartilhados explicitamente com eles.

![](assets/no2.png) Não é possível visualizar contatos e grupos

![](assets/no2.png)Não é possível criar provas, carregar ficheiros e criar pastas. Para obter mais informações, consulte [Fazer upload de arquivos e conteúdo da Web para [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)Não é possível exibir, editar ou excluir provas e arquivos criados por outros usuários na organização.

![](assets/no2.png)Não é possível editar provas ou respostas.

![](assets/no2.png)Não é possível excluir nenhum item criado na organização.

![](assets/no2.png)Não é possível acessar a página Faturamento ou as configurações da Conta. Para obter mais informações, consulte [O [!DNL Workfront Proof] Página de Faturamento](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) e [Configurações da conta em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Não pode ser definido como o proprietário do Dropzone. Para obter mais informações, consulte [Configure a área suspensa em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Não é possível esvaziar a lixeira. Para obter mais informações, consulte [Restaure e esvazie a lixeira no [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Não é possível adicionar, editar ou excluir usuários.

![](assets/no2.png)Não é possível criar grupos ou adicionar novos contatos.

![](assets/no2.png)Não é possível excluir contatos.

>[!NOTE]
>
>Os menus e as funções disponíveis para os Visitantes são limitados.
>
>* Os visitantes não visualizam o menu Cabeçalho ou o menu verde Novo no painel
>* Os visitantes não veem os seguintes links em suas Configurações: Configurações da conta, Faturamento
>


### Convidado {#guest}

O perfil Convidado é usado para conceder acesso a provas para revisores que não têm sua própria conta Workfront Proof. Os convidados podem acessar provas compartilhadas com eles diretamente por meio de suas notificações pessoais por email.

![](assets/cleaner2.png)Pode exibir, revisar e aprovar provas que são explicitamente compartilhadas com eles.

![](assets/cleaner2.png)Pode exibir arquivos que são compartilhados explicitamente com eles.

![](assets/no2.png)Não é possível acessar o Painel.

![](assets/no2.png)Não é possível ter pastas compartilhadas com elas. Para obter mais informações, consulte [Gerenciar pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Não pode ser adicionado como Autores ou Moderadores às provas. Para obter mais informações, consulte [Gerenciar funções de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

>[!NOTE]
>
>Os convidados não são usuários da Workfront Proof, portanto, não podem ver todas as provas compartilhadas com eles em seus próprios painéis.

## Editar o perfil de permissão de prova de um usuário

Os administradores e administradores de faturamento podem editar os perfis de permissão de todos os usuários na conta.

1. Para encontrar o usuário a ser editado, execute um dos seguintes procedimentos:

   * Navegar para **[!UICONTROL Configurações da conta]**, em seguida, clique no botão **[!UICONTROL Usuários]** guia .

   * Vá para o **[!UICONTROL Contatos]** página.

1. Clique no nome do usuário cujas permissões você deseja editar. ![](assets/screenshot-2018-03-30-14-16-05a-350x69.png)

1. Clique no botão **[!UICONTROL Perfil de permissões]** e selecione um novo perfil de permissão. :

   ![Captura de tela_2018-03-30_14-18-03.png](assets/screenshot-2018-03-30-14-18-03a.png)

   Os perfis de permissão são Administrador, Supervisor, Gerenciador e Observador.

1. Clique em qualquer lugar fora do menu para salvar.

>[!NOTE]
>
>Os administradores não podem atribuir o perfil Administrador de Faturamento. Você pode encontrar uma lista de alterações de Perfil nos seguintes logs:
>
>* Os registros de atividades da Conta
>* O log de perfil do usuário (acessível somente a esse usuário)
>


Para obter mais informações sobre logs de atividades, consulte [Noções básicas sobre o [!DNL Workfront Proof] Trilha de auditoria de atividade](../../../workfront-proof/wp-work-proofsfiles/basic-features/activity-audit-trail.md).
