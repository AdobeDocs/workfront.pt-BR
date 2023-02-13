---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: '"Logon único" [!DNL Workfront Proof]: Configuração do AD FS'''
description: Se for um administrador no servidor AD, poderá instalar e configurar o AD FS.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 670422e9-5db8-4f06-baf8-1f9ce83873fe
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# Logon único [!DNL Workfront Proof]: Configuração do AD FS

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

Se for um administrador no servidor AD, poderá instalar e configurar o AD FS.

## Instalar e configurar o AD FS

1. Baixar [AD FS 2.0](http://www.microsoft.com/en-us/download/details.aspx?id=10909) ao seu computador.
1. Abra o arquivo AdfsSetup.exe baixado para iniciar o Assistente de Instalação do ADFS (Ative Diretory Federation Services).
1. Na tela Função do Servidor, selecione uma das opções (você precisa, no mínimo, de um Servidor de Federação).
1. Se não quiser expor o IIS no servidor AD à Internet (portas 80 e 443 para HTTP e HTTPS), primeiro poderá configurar um Servidor de Federação atrás do firewall e, em seguida, criar um segundo Proxy do Servidor de Federação que passe as solicitações através do firewall para o Servidor de Federação.
1. Depois de concluir a configuração do AD FS, selecione **[!UICONTROL Inicie o snap-in Gerenciamento do AD FS 2.0]**, depois clique em **[!UICONTROL Concluir]**. Uma vez concluída, a janela Gerenciamento do AD FS 2.0 deve ser aberta imediatamente. Caso contrário, você pode abri-lo a partir de **[!UICONTROL Iniciar]** > **[!UICONTROL Ferramentas administrativas]** > **[!UICONTROL Gerenciamento do AD FS 2.0]**. Este é o principal aplicativo de controle AD FS.

1. Comece clicando em Assistente de Configuração do Servidor de Federação do AD FS 2.0.
Isso o ajudará a configurar o AD FS e conectá-lo à Internet via IIS e AD.
1. Se estiver a configurar um novo servidor AD FS, selecione **[!UICONTROL Criar um novo Serviço de Federação]**.
1. Selecionar **[!UICONTROL Servidor de federação independente]** (para fins de ensaio e avaliação).

1. Para obter alta disponibilidade e balanceamento de carga, clique em New federation server farm.
1. Especifique o nome do Serviço de Federação.
Por padrão, o assistente de configuração recupera o certificado SSL vinculado ao Site Padrão no IIS e usará o nome do assunto especificado lá. Se você usar um certificado curinga, precisará inserir o nome do Serviço de Federação.
Se não houver um certificado SSL configurado no IIS, o assistente de configuração pesquisará no armazenamento de certificados do computador local quaisquer certificados válidos. Eles são exibidos no menu suspenso Certificado SSL . Se não houver certificados encontrados, você pode usar o Gerador de certificados do servidor no IIS para criar um.

1. Continue com a configuração e clique em **[!UICONTROL Fechar]** após a conclusão.

## Configuração [!DNL Workfront Proof] Logon único

Se você for um [!DNL Workfront Proof] administrador, você pode configurar o Logon único na [!DNL Workfront Proof] lado. Para obter mais informações, consulte [Logon único [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

1. Clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações da conta]**, em seguida, abra o **[!UICONTROL Logon único]** guia .

1. No **URL SSO** , cole sua ID de entidade.
Este é um exemplo de uma ID de entidade: http://*&lt;adfs.your-company.com>*/adfs/services/trust Sua ID de entidade pode ser encontrada no arquivo XML de metadados de federação.
   ![ProofHQ_configuration_02.png](assets/proofhq-configuration-02-350x80.png)

1. Os Metadados de Federação são encontrados no snap-in do AD FS 2.0 > Serviço > Pasta de Endpoints. Na seção Metadados , localize aquele com o tipo de Metadados de Federação . Para exibir metadados, cole esse terminal no navegador. Você também pode acessar este link diretamente: https://*&lt;adfs.your-company.com>*/FederationMetadata/2007-06/FederationMetadata.xml depois de substituir o {adfs.your-company.com} por seus próprios detalhes.
1. No **[!UICONTROL URL de logon]** , cole seu logon SSO.
1. Este é um exemplo de um logon SSO:
1. http://*&lt;adfs.your-company.com>*/adfs/ls.
1. Esse link pode ser localizado no arquivo XML de Metadados de Federação.
   ![ProofHQ_configuration_03.png](assets/proofhq-configuration-03-350x90.png)

1. No **[!UICONTROL URL de logout]** digite o link e salve.
Este é um exemplo de URL de Logout: https://*&lt;adfs.your-company.com>*/adfs/ls/?wa=wsignout1.0

   1. Vá para o gerenciador do AD FS > Relacionamentos de confiança > Confianças de terceiros confiáveis - Propriedades do ProofHQ.
   1. Em Endpoints, clique em [!UICONTROL Adicionar e inserir] com os seguintes detalhes:

      * Tipo de Endpoint = Logout SAML
      * Vínculo = POST
      * URL = https://*&lt;adfs.your-company.com span=&quot;&quot; id=&quot;1&quot; translate=&quot;no&quot; />>/adfs/ls/?wa=wsignout1.0*
      * Esta etapa pode ser concluída após a configuração da Confiança da terceira parte confiável (veja abaixo) em seu AD FS.
   1. No **[!UICONTROL Impressão digital do certificado]** , insira os dados do certificado.
   1. Vá para o snap-in ADFS 2.0 e navegue até Serviço > Certificados > Assinatura de token.
   1. Clique com o botão direito do mouse nessa entrada para exibir o certificado.
   1. No [!UICONTROL Detalhes do certificado] copie a impressão digital e cole na guia **[!UICONTROL Logon único na prova do Workfront]** guia configuração .

   1. Os caracteres de impressão digital podem ser separados por dois pontos ou espaços, mas recomendamos removê-los. Se você tiver problemas com sua configuração de Logon único, entre em contato com a equipe de suporte ao cliente.


## Adicionar uma Confiança de Terceiros Confiantes

Quando a configuração estiver concluída, você precisará trabalhar na seção Confianças da terceira parte no seu AD FS.

1. Navegar para **[!UICONTROL Relacionamentos de Confiança]** > **[!UICONTROL Confianças de terceiros confiáveis]** e, em seguida, clique em **[!UICONTROL Adicionar uma Confiança de Terceiros Confiantes]** para iniciar o assistente de configuração.

1. Selecione sua fonte de dados.
Todos os metadados para seu [!DNL ProofHQ] está localizada em um link como este: https://`<yoursubdomain*>`.proofhq.com/saml/module.php/saml/sp/metadata.php/phq Isso configurará a maioria da confiança da terceira parte confiável.

   >[!NOTE]
   >
   >* Em caso de problemas ao estabelecer a conexão do URL, salve os metadados como um arquivo e escolha importar dados de um arquivo.
   >* Quando você tem um domínio Personalizado completo (por exemplo, www.your-proofing.com) configurado em [!DNL ProofHQ] substitua a conta inteira da parte &quot;{yoursubdomain}.proofhq.com&quot; por seu próprio domínio para criar seu [!DNL ProofHQ] link de metadados.



## Configuração das Regras de Reivindicação

Quando a configuração da Confiança da terceira parte confiável estiver concluída, você estará pronto para configurar as regras de solicitação para concluir a configuração. Você irá configurar duas regras de solicitação para o ProofHQ: E-mail e ID do nome.

1. Abra o **[!UICONTROL Editar regras de solicitação]** caixa de diálogo.
1. Ir para **[!UICONTROL Confiança de terceiros confiáveis no ProofHQ]**, depois clique em **[!UICONTROL Editar regras de solicitação]** (1)\
   A janela pop-up deve ser aberta automaticamente se você tiver selecionado essa opção ao final da configuração da confiança.

1. Clique em **[!UICONTROL Adicionar regra]** (2) para abrir a janela de configuração da declaração.

   * E-mail (Enviar atributos LDAP como modelo de regra de Reivindicações)
   * NameID (Transformar um modelo de regra de Solicitação de Entrada)
