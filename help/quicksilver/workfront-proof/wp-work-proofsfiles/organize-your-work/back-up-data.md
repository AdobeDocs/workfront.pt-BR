---
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: Fazer Backup dos Dados [!DNL Workfront Proof]
description: Você pode solicitar um backup de todos os seus dados no  [!DNL Workfront Proof] usando a função de backup.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 3b831bb5-2d03-4d7e-ad1f-54ae95f05ccd
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 0%

---

# Fazer Backup Dos Dados Do [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

## Introdução aos backups

Você pode solicitar um backup de todos os seus dados no [!DNL Workfront Proof] usando a função de backup.

O backup é fornecido a você como um arquivo .zip. Inclui uma exportação XML de todos os seus dados (incluindo comentários e respostas para todas as versões de todas as provas); no entanto, não inclui os arquivos originais que você carregou como provas.

Cada arquivo .zip de backup criado para download tem um nome de arquivo exclusivo, como:

9789_05_05_2011_61703.zip

O nome do arquivo neste exemplo fornece as seguintes informações:

* 9789 é o identificador de conta do [!DNL Workfront Proof]
* 05_05_2011 é a data de criação, 5 maio 2011
* 61703 é um número aleatório atribuído pelo sistema

Essa convenção de nomenclatura facilita o armazenamento de todos os arquivos .zip de backup em um único local no computador e permite saber exatamente quando cada backup foi criado para você.

A função [!UICONTROL Backup] permite decidir como usar seus recursos:

* Permite liberar espaço de armazenamento sem perder as provas ativas ou arquivadas. Você pode solicitar um backup, excluir as provas e esvaziar a [Restaurar e Esvaziar a Lixeira em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).
* Permite que você acesse quaisquer arquivos originalmente carregados no [!DNL Workfront] Proof. Você pode baixá-los usando a função [!UICONTROL baixar arquivo original] antes de excluir as provas.

>[!NOTE]
>
>Considere o seguinte ao usar backups:
>
>* Os backups estão disponíveis em planos Enterprise e Unlimited. Entre em contato com nossa [equipe de vendas](mailto:sales@proofhq.com) para obter uma cotação.
>* O tipo de codificação de dados é definido como UTF-8 por padrão e recomendamos essa configuração. Este é o tipo de codificação mais comumente usado por aplicativos da Internet.
>* Você pode solicitar somente um [!DNL backup] de cada vez. Quando o arquivo de backup .zip estiver sendo processado, o link Solicitar novo backup na guia Backups não será exibido e a mensagem mostrada permanecerá inalterada. Para obter informações sobre como solicitar um backup, consulte [Solicitar um novo backup de dados em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/request-new-data-backup-in-wp.md).
>



## Backup dos dados

1. Clique em **[!UICONTROL Configurações da conta]** no canto superior direito da interface [!DNL Workfront Proof]. (1)
1. Clique na guia **[!UICONTROL Backups]**. (2)
1. Clique no link **[!UICONTROL Solicitar novo backup]** (3)

Quando o backup estiver pronto, ocorrerá o seguinte:

* Você receberá um email de [!DNL Workfront Proof] notificando-o sobre isso (&quot;O backup do [!DNL Workfront Proof] está pronto&quot;). O email contém um link de download para seus dados de backup.
* A guia Backup de [Configurações da conta](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) exibe um link de download para seus dados de backup.
* O link Solicitar novo backup (3) será exibido novamente na guia Backups

Seus dados estarão prontos para download como um arquivo zip. Você pode baixar o arquivo .zip de backup no email de notificação ou nas [!UICONTROL configurações da conta], conforme descrito nas seguintes seções:

* [Baixando o arquivo de backup .zip da notificação por email](#downloading-your-backup-zip-file-from-your-email-notification)
* [Baixando o arquivo .zip de backup nas configurações da conta](#downloading-your-backup-zip-file-from-the-account-settings)

![Request_Backup.png](assets/request-backup-350x167.png)

## Baixando o arquivo de backup .zip da notificação por email {#downloading-your-backup-zip-file-from-your-email-notification}

Quando o arquivo .zip de backup estiver pronto para ser baixado, você receberá um email de [!DNL Workfront Proof] com a linha de assunto &quot;Seu backup do [!DNL Workfront Proof] está pronto.&quot;

Para baixar o arquivo de backup .zip do email:

1. Clique no link de download no email.\
   ![Backup_mail.png](assets/backup-mail-350x120.png)\
   Se você não tiver feito logon no [!DNL Workfront Proof], uma nova janela do navegador será aberta e exibirá a página de logon.

## Baixando o arquivo .zip de backup nas configurações da conta {#downloading-your-backup-zip-file-from-the-account-settings}

Quando o arquivo .zip de backup estiver pronto para ser baixado, a guia [!UICONTROL Backup] indicará isso exibindo um link de download. Além disso, o link [!UICONTROL Solicitar novo backup] será exibido novamente.

1. Clique em **[!UICONTROL Configurações da conta]** no canto superior direito da interface [!DNL Workfront Proof]. (1)
1. Clique na guia **[!UICONTROL Backups]**. (2)\
   Se nenhum usuário da sua conta tiver solicitado backups, a guia [!UICONTROL Backups] indicará que você não tem backups. Se um usuário solicitou um backup, a guia exibe a data de criação e o link de download do último backup.

1. Clique no link **[!UICONTROL Baixar backup]**. (3)\
   ![Download_Backup.png](assets/download-backup-350x167.png) Uma tela Download de Arquivo é exibida, perguntando se você deseja Abrir ou Salvar o arquivo de download.

1. Clique em **[!UICONTROL Salvar]** e selecione o local no computador em que deseja salvar o arquivo .zip de backup.\
   A mensagem que identifica a data do backup mais recente permanece exibida na parte inferior da página [!UICONTROL Backup] até a próxima vez que você solicitar um backup. O link Download backup se aplica a esse último backup. Sempre que o link [!UICONTROL Solicitar novo backup] for exibido, você poderá clicar nele para solicitar outro backup.

## Noções básicas sobre os arquivos no arquivo de backup .zip

Seu arquivo .zip de backup contém sete arquivos CSV (valores separados por vírgulas ou delimitados por vírgulas) que incluem informações de suas provas ativas e arquivadas até o momento em que foi feito o backup dos dados:

* comments.csv - inclui comentários em provas
* comment_replies.csv - inclui respostas a comentários em provas organization.csv - inclui o identificador numérico e o nome da sua organização (sua conta)
* contacts.csv - inclui o identificador numérico, o nome e a organização de cada contato
* files.csv - inclui informações da página Detalhes da Prova ou da página Detalhes do Arquivo sobre provas ou arquivos carregados para [!DNL Workfront Proof]
* recipients.csv - inclui identificador numérico, função e decisões de cada pessoa especificada como revisor, revisor e aprovador, etc., quando as provas são carregadas para revisão em [!DNL Workfront Proof]
* users.csv - inclui identificadores numéricos e nomes de todos os usuários na conta

Você pode extrair esses arquivos do arquivo .zip de backup com qualquer utilitário zip usado e, em seguida, armazená-los no local de sua escolha no computador. Depois de salvar o arquivo zip e extrair os arquivos CSV individuais, é possível manipular as informações conforme desejado para a manutenção interna de registros.

Cada arquivo .zip de backup criado a seu pedido tem um nome distinto que inclui a data de criação do backup, mas os arquivos CSV incluídos em cada arquivo .zip de backup sempre têm os mesmos nomes. Você pode usar um dos métodos a seguir para garantir que seus arquivos de backup sejam distintos entre si:

* Crie uma nova pasta para cada arquivo .zip de backup e os arquivos CSV extraídos dela.
* Renomeie cada arquivo CSV individual para incluir a data do backup quando você o extrair do arquivo zip.

>[!NOTE]
>
>Se o [!DNL Microsoft Excel] estiver instalado no computador, o utilitário de extração poderá listar o tipo de arquivo para os arquivos CSV individuais como [!DNL Microsoft Office Excel] Arquivo de Valores Separados por Vírgula. Você pode abrir um arquivo CSV extraído usando [!DNL Excel] e salvar o arquivo como uma pasta de trabalho [!DNL Excel] (&#42;.xlsx) ou algum outro tipo de arquivo.
