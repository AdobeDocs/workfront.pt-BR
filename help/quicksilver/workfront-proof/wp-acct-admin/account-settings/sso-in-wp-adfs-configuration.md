---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: 'Logon Único em  [!DNL Workfront Proof]: configuração do AD FS'
description: Se você for um administrador no servidor AD, poderá instalar e configurar o AD FS.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 670422e9-5db8-4f06-baf8-1f9ce83873fe
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# Logon Único em [!DNL Workfront Proof]: configuração do AD FS

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

Se você for um administrador no servidor AD, poderá instalar e configurar o AD FS.

## Instalando e Configurando o AD FS

1. Baixe o [AD FS 2.0](http://www.microsoft.com/en-us/download/details.aspx?id=10909) no computador.
1. Abra o arquivo AdfsSetup.exe baixado para iniciar o Assistente de Instalação do ADFS (Ative Diretory Federation Services).
1. Na tela Função do Servidor, selecione uma das opções (você precisa, no mínimo, de um Servidor de Federação).
1. Se você não quiser expor o IIS em seu servidor AD para a Internet (portas 80 e 443 para HTTP e HTTPS), primeiro poderá configurar um Servidor de Federação por trás do firewall e, em seguida, criar um segundo Proxy de Servidor de Federação que passe as solicitações pelo firewall para o Servidor de Federação.
1. Depois de concluir a instalação do AD FS, selecione **[!UICONTROL Iniciar o snap-in de Gerenciamento do AD FS 2.0]** e clique em **[!UICONTROL Concluir]**. Depois que isso for concluído, a janela Gerenciamento do AD FS 2.0 deverá ser aberta imediatamente. Caso contrário, você poderá abri-lo em **[!UICONTROL Iniciar]** > **[!UICONTROL Ferramentas Administrativas]** > **[!UICONTROL Gerenciamento do AD FS 2.0]**. Este é o principal aplicativo de controle do AD FS.

1. Comece clicando em Assistente de Configuração do Servidor de Federação do AD FS 2.0.
Isso ajudará você a configurar o AD FS e conectá-lo à Internet via IIS e ao AD.
1. Se você estiver configurando um novo servidor AD FS, selecione **[!UICONTROL Criar um novo Serviço de Federação]**.
1. Selecione **[!UICONTROL Servidor de federação autônomo]** (para fins de teste e avaliação).

1. Para alta disponibilidade e balanceamento de carga, clique em Novo farm de servidores de federação.
1. Especifique o nome do Serviço de Federação.
Por padrão, o assistente de configuração recupera o certificado SSL associado ao Site Padrão no IIS e usará o nome do assunto especificado. Se você usar um certificado curinga, precisará inserir o nome do Serviço de Federação.
Se não houver um certificado SSL configurado no IIS, o assistente de configuração pesquisará no armazenamento de certificados do computador local se há certificados válidos. Eles são exibidos na lista suspensa Certificado SSL. Se nenhum certificado for encontrado, você poderá usar o Gerador de Certificados do Servidor no IIS para criar um.

1. Continue com a configuração e clique em **[!UICONTROL Fechar]** depois que ela for concluída.

## Configurando [!DNL Workfront Proof] Logon Único

Se você for um administrador [!DNL Workfront Proof], poderá configurar o Logon único no lado [!DNL Workfront Proof]. Para obter mais informações, consulte [Logon único [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

1. Clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações de Conta]** e abra a guia **[!UICONTROL Logon único]**.

1. Na caixa **URL do SSO**, cole sua ID de entidade.
Veja a seguir um exemplo de uma ID de entidade:
http://*&lt;adfs.your-company.com>*/adfs/services/trust
Sua ID de entidade pode ser encontrada no arquivo XML de Metadados de Federação.
   ![ProofHQ_configuration_02.png](assets/proofhq-configuration-02-350x80.png)

1. Os Metadados de Federação são encontrados no snap-in do AD FS 2.0 > Serviço > pasta Pontos de Extremidade. Na seção Metadados, localize aquele com o tipo de Metadados da Federação. Para exibir metadados, cole esse endpoint no navegador. Você também pode acessar este link diretamente: https://*&lt;adfs.your-company.com>*/FederationMetadata/2007-06/FederationMetadata.xml depois de substituir o {adfs.your-company.com} pelos seus próprios detalhes.
1. Na caixa **[!UICONTROL URL de Logon]**, cole seu logon com SSO.
1. Veja a seguir um exemplo de logon com SSO:
1. http://*&lt;adfs.your-company.com>*/adfs/ls.
1. Este link pode estar localizado no arquivo XML de Metadados de Federação.
   ![ProofHQ_configuration_03.png](assets/proofhq-configuration-03-350x90.png)

1. Na caixa **[!UICONTROL URL de logoff]**, digite o link e salve.
Este é um exemplo de um URL de logout:
https://*&lt;adfs.your-company.com>*/adfs/ls/?wa=wsignout1.0

   1. Acesse seu gerenciador do AD FS > Relações de Confiança > Relações de Confiança de Terceiras Partes Confiáveis - Propriedades de ProofHQ.
   1. Nos Pontos de Extremidade, clique em [!UICONTROL Adicionar e entrada] com os seguintes detalhes:

      * Tipo de Ponto de Extremidade = Logout SAML
      * Vinculação = POST
      * URL = https://*&lt;adfs.your-company.com*>/adfs/ls/?wa=wsignout1.0
      * Esta etapa pode ser concluída após a configuração do Objeto de Confiança de Terceira Parte Confiável (veja abaixo) no AD FS.
   1. Na caixa **[!UICONTROL Impressão digital do certificado]**, insira os dados do certificado.
   1. Vá para o snap-in do ADFS 2.0 navegue até Serviço > Certificados > Assinatura de token.
   1. Clique com o botão direito do mouse nessa entrada para exibir o certificado.
   1. Na guia [!UICONTROL Detalhes do Certificado], copie a Impressão Digital e cole-a na guia de configuração **[!UICONTROL Logon Único do Workfront Proof]**.

   1. Os caracteres de impressão digital podem ser separados por dois pontos ou espaços, mas recomendamos removê-los. Se você tiver algum problema com a configuração de Logon único, entre em contato com a equipe de Suporte ao cliente.


## Adicionando um objeto de confiança de terceira parte confiável

Quando a configuração for concluída, você precisará trabalhar na seção Confianças da Terceira Parte Confiável no AD FS.

1. Navegue até a pasta **[!UICONTROL Relações de Confiança]** > **[!UICONTROL Relações de Confiança de Terceira Parte Confiável]** e clique em **[!UICONTROL Adicionar uma Confiança de Terceira Parte Confiável]** para iniciar o assistente de configuração.

1. Selecione sua fonte de dados.
Todos os metadados da sua conta [!DNL ProofHQ] estão localizados em um link como este:
https://`<yoursubdomain*>`.proofhq.com/saml/module.php/saml/sp/metadata.php/phq
Isso configurará a maior parte da Terceira Parte Confiável.

   >[!NOTE]
   >
   >* Se tiver problemas com o estabelecimento da conexão do URL, salve os metadados como um arquivo e escolha importar dados de um arquivo.
   >* Quando você tiver um domínio Personalizado completo (por exemplo, www.your-proofing.com) configurado em sua conta do [!DNL ProofHQ], substitua toda a parte &quot;{yoursubdomain}.proofhq.com&quot; pelo seu próprio domínio para criar o link de metadados do [!DNL ProofHQ].


## Configurando Regras de Declaração

Quando a configuração do Objeto de Confiança de Terceira Parte Confiável estiver concluída, você estará pronto para configurar as regras de declaração para concluir a configuração. Você configurará duas regras de reclamação para o ProofHQ: E-mail e ID de nome.

1. Abra a caixa de diálogo **[!UICONTROL Editar Regras de Declaração]**.
1. Vá para **[!UICONTROL ProofHQ Confiança da Terceira Parte Confiável]** e clique em **[!UICONTROL Editar Regras de Declaração]** (1).\
   A janela pop-up deverá ser aberta automaticamente se você tiver selecionado essa opção ao final da configuração da relação de confiança.

1. Clique em **[!UICONTROL Adicionar Regra]** (2) para abrir a janela de configuração da declaração.

   * Email (Enviar Atributos LDAP como modelo de regra de Declarações)
   * NameID (Transformar um modelo de regra de Declaração de Entrada)
