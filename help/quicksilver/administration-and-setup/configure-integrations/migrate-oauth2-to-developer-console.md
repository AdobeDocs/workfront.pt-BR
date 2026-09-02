---
title: Migração do Workfront OAuth2 para o Adobe Developer Console
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: O serviço de aplicativo OAuth2 personalizado herdado da Workfront está sendo removido. Saiba o que está mudando, quem é afetado e como migrar suas integrações personalizadas para o Adobe Developer Console.
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
source-git-commit: db7e6a6fa0c5fc5332213c388d9b4db3a5c59f53
workflow-type: tm+mt
source-wordcount: '1473'
ht-degree: 1%

---

# Migração do Workfront OAuth2 para o Adobe Developer Console

O serviço de aplicativo OAuth2 personalizado herdado da Workfront (as integrações configuradas em **Configuração** > **Sistema** > **OAuth2**) estão sendo removidas. A partir de agora, todas as integrações personalizadas autenticadas no Workfront devem usar o fluxo de autenticação do Adobe Developer Console (developer.adobe.com).

Essa alteração afeta qualquer ferramenta de integração, script ou de terceiros personalizada que seja autenticada no momento usando uma ID de cliente OAuth2 emitida pela Workfront e um segredo. Isso não afeta o logon no Workfront nem as integrações padrão gerenciadas pela Adobe, como as integrações em pacotes do Microsoft Teams ou do Slack, que o Adobe está migrando separadamente.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso do Adobe Workfront</td> 
   <td><p>Administrador de sistema</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Direitos do Adobe Developer Console</td> 
   <td><p>Os direitos de administrador da Organização IMS são necessários para acessar o Adobe Developer Console para Workfront. Isso é mais abrangente do que uma função de administrador de produto do Workfront, pois gerencia toda a organização da Adobe e todos os produtos nela contidos.</p></td> 
  </tr> 
 </tbody> 
</table>

+++

## Datas principais

| Data | Marco | O que isso significa para você |
|---|---|---|
| 1 de novembro de 2026 | Criação de novo aplicativo desabilitada | Não é mais possível criar novos aplicativos OAuth2 personalizados no Workfront. Os aplicativos existentes continuam a funcionar. |
| 1 de fevereiro de 2027 | Serviço herdado desativado | Os aplicativos OAuth2 personalizados existentes param de funcionar. Qualquer integração que não tenha migrado para o Adobe Developer Console perde acesso à API do Workfront no momento. |

>[!IMPORTANT]
>
>Recomendamos planejar e concluir sua migração antes de 1º de novembro de 2026, para que suas integrações continuem sendo executadas sem interrupção e para que você não migre para o prazo final de 1º de fevereiro de 2027.

## Organizações afetadas

Sua organização é afetada por essa alteração se tiver qualquer integração, script ou ferramenta que se conecte ao Workfront usando uma ID de cliente OAuth2 personalizada e um segredo emitido pela tela de configuração herdada do OAuth2 da Workfront. Exemplos comuns incluem:

* Integrações personalizadas que sua equipe de engenharia mantém com a API do Workfront.
* Conectores de terceiros ou criados por parceiros configurados com uma ID de cliente emitida pela Workfront. Recomendamos verificar com seu fornecedor se não tiver certeza de como a integração é autenticada.
* Automação interna, relatórios ou scripts de sincronização de dados que chamam a API do Workfront diretamente.

Se você não souber se sua organização tem algum desses aplicativos, o administrador do Workfront pode verificar a lista de aplicativos do OAuth2 em **Configuração** > **Sistema** > **OAuth2** para ver o que está registrado no momento. Para obter informações, consulte [Exibir e gerenciar aplicativos OAuth2 personalizados](/help/quicksilver/administration-and-setup/configure-integrations/manage-custom-oauth2-apps.md).

## Entender os tipos de autenticação do Adobe Developer Console

O Adobe Developer Console oferece suporte a mais de uma maneira de autenticação. Você pode selecionar o tipo que corresponde a como a integração funciona:

* **Autenticação de Servidor para Servidor**: para um aplicativo em execução em seu back-end que chama APIs do Adobe em nome de sua organização, sem o envolvimento de usuários finais. Essa é a correspondência mais próxima do padrão herdado do Workfront OAuth2 trabalhada com IDs de clientes e segredos, e é o tipo que a maioria das integrações, scripts e automações personalizadas do Workfront deve usar.
* **Autenticação de Usuário**: para casos em que um usuário do Adobe precisa entrar e consentir para que seu aplicativo possa exibir ou editar seus dados. Se a integração precisar agir em nome de um usuário do Workfront conectado específico em vez de em sua organização como um todo, use esse tipo.

  Se você escolher Autenticação de usuário, há três outras opções, dependendo da arquitetura do seu aplicativo:

  * **Aplicativo Web OAuth**: para aplicativos com uma interface de front-end e um servidor back-end. O servidor armazena com segurança o segredo do cliente e busca tokens.
  * **Aplicativo de Página Única do OAuth**: para aplicativos Web somente de navegador sem servidor back-end. O próprio aplicativo web busca tokens.
  * **Aplicativo Nativo OAuth**: para aplicativos móveis ou de desktop que são executados nativamente em um dispositivo e não têm servidor de back-end. O aplicativo nativo busca tokens.

A maioria das organizações que está migrando uma integração de back-end, script ou automação do serviço OAuth2 herdado deseja a Autenticação de servidor para servidor.

## Comparação de recursos: OAuth2 herdado vs. Adobe Developer Console

O serviço Workfront OAuth2 herdado (encontrado em **Configuração** > **Sistema** > **Aplicativos OAuth2**) oferece três tipos de aplicativos, com um limite de 10 aplicativos OAuth2 por instância do Workfront. Veja como esses aspectos se comparam ao Adobe Developer Console:

| Tipo de Workfront herdado | Método de fluxo/autenticação | Equivalente do Developer Console | Ajustar |
|---|---|---|---|
| Aplicativo de máquina para máquina (CLIs, daemons, scripts de back-end) | JWT com par de chave pública/privada | Autenticação de servidor para servidor | O mesmo objetivo de não envolver o usuário final, mas o mecanismo muda. O fluxo herdado usa um par de chaves públicas/privadas e o JWT, enquanto o servidor para servidor usa uma ID do cliente e um segredo do cliente com uma concessão de credenciais do cliente OAuth. Esta não é uma troca de credencial suspensa. O código de autenticação da integração precisa ser alterado, não apenas os valores de credencial. Para obter informações, consulte [Usando o fluxo JWT para aplicativos OAuth 2 personalizados](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md). |
| Aplicativo Web (aplicativos do lado do servidor: Go, Java, .NET, Node, PHP) | Fluxo de código de autorização OAuth 2.0 | OAuth Web App (em Autenticação de Usuário) | Correspondência 1:1 mais próxima. Isso tem o mesmo fluxo e a mesma forma básica com que um servidor de back-end armazena o segredo do cliente. Para obter informações, consulte [Fluxo de código de autorização para aplicativos OAuth 2 personalizados](/help/quicksilver/wf-api/api/oauth-app-code-token-flow.md). |
| Aplicativo web de página única (JS, Angular, React, Vue) | Fluxo de código de autorização com PKCE, sem segredo do cliente | Aplicativo de página única OAuth (em Autenticação do usuário) | A correspondência 1:1 mais próximaTem o mesmo fluxo secreto baseado em PKCE. Para obter informações, consulte [Usando o fluxo PKCE para aplicativos OAuth 2](/help/quicksilver/wf-api/api/oauth-app-pkce-flow.md). |
| (nenhum equivalente herdado) | — | Aplicativo OAuth nativo (em Autenticação do usuário) | Esse é um novo recurso. O Workfront OAuth2 herdado não tem um tipo dedicado para aplicativos móveis ou de desktop nativos. |

<!--

>[!NOTE]
>
>A few legacy capabilities don't have a confirmed equivalent yet in Adobe Developer Console, and are being validated with the Developer Console team:
>
>* Per-app controls the legacy UI offers: refresh token rotation toggle, absolute vs. inactivity refresh token expiration, custom logo, privacy policy URL, and developer contact fields.
>* Whether Developer Console enforces a cap on credentials or projects similar to the legacy 10-app-per-instance limit.
>* Whether a JWT/key pair-based option remains available anywhere in Developer Console for Machine to Machine customers, or whether all such integrations must move to the client-secret-based Server-to-Server grant.

-->

## Procedimento de migração

### Se você for um Administrador de sistema da Workfront

>[!NOTE]
>
>Se você for um administrador de produto do Workfront, mas não um administrador de organização, precisará trabalhar com o administrador de organização para concluir essa migração ou solicitar que seja feita uma.

1. Faça logon em [developer.adobe.com](https://developer.adobe.com) e crie um novo Projeto. Os projetos são a forma como o console organiza diferentes integrações ou aplicativos clientes.
1. No Projeto, adicione uma API e selecione **Adobe Workfront**. Essa API está na categoria Experience Cloud. Todas as APIs do Workfront, incluindo Planejamento, Fluxo de trabalho, Revisão e aprovações, compartilham essa única API.
1. Selecione a opção de autenticação de **Servidor para Servidor** e escolha a instância correta se sua Organização IMS tiver mais de uma instância Workfront.

   Para obter orientação sobre como escolher um tipo de autenticação, consulte [Entender os tipos de autenticação do Adobe Developer Console](#understand-adobe-developer-console-authentication-types) neste artigo.
1. Na página Projeto, abra os detalhes da nova credencial do servidor para servidor OAuth e encontre a ID do cliente, o segredo do cliente e as informações necessárias para gerar tokens de acesso.
1. Atualize sua integração, script ou ferramenta para autenticar com essas novas credenciais no lugar da ID antiga do cliente OAuth2 da Workfront e do segredo.
1. Confirme o acesso no Workfront. A criação do cliente da API o adiciona automaticamente como o usuário do Workfront &quot;`techacct`&quot;. Por padrão, ele é adicionado como um Colaborador com acesso limitado, mas você pode ajustar o nível de acesso como faria para qualquer outro usuário.
1. (Opcional) Para conceder os direitos de administrador de usuário do `techacct`, adicione o email da Conta técnica como administrador do Perfil de produto relevante no Admin Console.
1. Teste a integração de ponta a ponta.
1. Desative a entrada de aplicativo OAuth2 antiga no Workfront depois de confirmar que a nova conexão está funcionando.

Para obter detalhes completos passo a passo e capturas de tela, consulte [Obtendo acesso](https://developer.adobe.com/workfront-apis/guides/gaining_access/) na documentação do Developer Console da Adobe.

### Se você não for um Administrador do sistema

É necessário executar um loop no administrador da organização de IMS para concluir a migração, já que a configuração da nova credencial no Adobe Developer Console exige esse nível de acesso. Se você gerenciar ou manter uma integração, mas souber quem é o administrador da organização IMS, entre em contato com uma das seguintes pessoas:

* Sua equipe de conta da Workfront
* Sua equipe interna de TI
* Seu contato de engenharia

## Se você não migrar

As integrações que ainda usam o padrão herdado ID/segredo do cliente OAuth2 após 1º de fevereiro de 2027 deixam de ser capazes de se autenticar na API do Workfront e qualquer fluxo de trabalho, sincronização ou automação dependente falha. Não há extensão planejada após essa data, portanto, migre suas integrações bem antes dela.

## Perguntas frequentes

**Isso afeta as integrações em pacotes fornecidas pela Adobe, como o Slack ou o Microsoft Teams?**

Não. Os aplicativos globais gerenciados pela Adobe estão sendo migrados diretamente pela Adobe e não exigem nenhuma ação da sua parte.

**Minha integração existente deixará de funcionar antes de 1º de fevereiro de 2027?**

Não. Os aplicativos OAuth2 personalizados existentes continuarão a funcionar normalmente até 1º de fevereiro de 2027. Somente a capacidade de criar novos aplicativos OAuth2 personalizados será afetada, a partir de 1º de novembro de 2026.

**Há um custo para migrar?**

Não, não há custo adicional associado à autenticação por meio do Adobe Developer Console.

**Onde posso obter ajuda?**

Entre em contato com a equipe de conta da Workfront ou abra um caso de suporte se tiver dúvidas sobre a integração ou linha do tempo específica. Para obter a apresentação oficial e atualizada da configuração com capturas de tela, consulte [Obtendo acesso](https://developer.adobe.com/workfront-apis/guides/gaining_access/) na documentação do Developer Console do Adobe.
