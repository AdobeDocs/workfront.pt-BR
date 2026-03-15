---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Perguntas frequentes sobre a experiência unificada da Adobe
description: Alguns recursos são diferentes entre o  [!DNL Workfront] e o Adobe Experience Cloud, e você pode ter algumas dúvidas à medida que sua instância [!DNL Workfront] é migrada para a experiência unificada.
author: Courtney
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '1397'
ht-degree: 1%

---

# [!DNL Adobe Unified Experience] Perguntas frequentes

The [!DNL Adobe Unified Experience] for [!DNL Workfront] allows you to manage all of your [!DNL Adobe] applications in one place with a single login. The [!DNL Adobe] navigation area is integrated seamlessly with [!DNL Workfront]. A few features are different, and you might have some questions as your [!DNL Workfront] instance is migrated to the unified experience.

For information about how to log in to the [!DNL Adobe Unified Experience], see [[!DNL Adobe Unified Experience] for [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## Comparison of [!DNL Adobe Unified Experience] and [!DNL Workfront only] experience

Only customers using the [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] can access the [!DNL Adobe Unified Experience]. Customers who have not yet migrated will see the [!DNL Workfront only] experience, without the ability to switch between [!DNL Adobe] applications.

Esta tabela descreve alguns recursos que diferem entre as duas experiências.

| [!DNL Adobe Unified Experience] | Somente experiência do [!DNL Workfront] |
| ---- | ----|
| O [!UICONTROL [!DNL Workfront] Menu Principal] está à esquerda do ![Menu Principal](assets/main-menu-icon-left-nav.png) | O [!UICONTROL [!DNL Workfront] Menu Principal] está à direita do ![Menu Principal](assets/main-menu-icon.png) |
| Uma única URL de logon está disponível para todos os aplicativos do [!DNL Adobe Experience Cloud] | Fazer logon em [!DNL Workfront] com uma URL [!DNL Workfront] personalizada |
| Um “alternador de organização” permite que você alterne entre [!DNL Workfront] organizações e ambientes | O “alternador de organização” não está disponível |
| A navegação inclui uma área de navegação de nível superior para produtos do [!DNL Adobe], notificações do [!DNL Adobe], ajuda e seu perfil de usuário, além da barra de navegação do [!DNL Workfront] | A navegação inclui somente a barra de navegação [!DNL Workfront] |
| A ajuda está acessível por meio do [!UICONTROL Menu Principal] e da área de navegação superior | A ajuda pode ser acessada pelo [!UICONTROL Menu Principal] e pela barra de navegação [!DNL Workfront] |
| O visualizador de provas é aberto em uma nova guia | O visualizador de provas é aberto dentro do Workfront |
| A URL usada para acessar o Workfront é `experience.adobe.com` | A URL usada para acessar o Workfront é `(CompanyName).my.workfront.adobe.com` |
| O formato da data (como MM/DD/AAAA) é baseado nas configurações de idioma da Experiência unificada. Se o usuário não atualizou as configurações de idioma, as configurações `en-US` serão usadas. | O formato da data (como MM/DD/AAAA) é baseado nas preferências do navegador |

{style="table-layout:auto"}

## Perguntas frequentes

### Como determinar se estou usando a Experiência unificada do Adobe ou o Adobe Workfront?

Para determinar se sua organização está na Experiência unificada da Adobe, examine o URL usado para acessar o Workfront.

| URL | Adobe Experience |
|------------|------------|
| (CompanyName).my.workfront.com | experiência com o Workfront |
| experience.adobe.com | Adobe Unified Experience |

### Como posso obter mais informações sobre o [!DNL Adobe Admin Console]?

Para obter informações sobre o [!DNL Admin Console], leia estes artigos:

* [Preparar para o(a) [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [Diferenças de administração baseadas em plataforma ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] visão geral](https://helpx.adobe.com/br/enterprise/using/admin-console.html)

### What do I as a customer need to do to facilitate the migration?

Os clientes existentes serão contatados para agendar migrações. Os colegas de suporte da equipe de migração guiarão os clientes pelo processo, aconselharão sobre a configuração do [!DNL Admin Console] e fornecerão links para a documentação necessária para fazer a migração da forma mais simples e descomplicada possível. Leia as [[!DNL Adobe Business Platform] e [!DNL Admin Console] Perguntas frequentes](https://experienceleague.adobe.com/pt-br/docs/support-resources/adobe-support-tools-guide/workfront/faq) para obter mais informações.

### Como você está lidando com o [!DNL Adobe Admin Console] para empresas que já têm esse recurso habilitado para federated IDs de forma diferente da configuração de SSO do [!DNL Workfront]?

[!DNL Adobe Admin Console] tem a opção de incluir [!DNL Workfront], substituindo o SSO por um Sistema Adobe Identity Management (IMS). Todo o provisionamento de usuários ocorre no [!DNL Admin Console], e os usuários verão a tela de logon do [!DNL Adobe] para chegar ao [!DNL Experience Cloud], onde verão o [!DNL Workfront] como uma opção (se tiverem acesso).

### How does this impact customers that already have the AEM admin panel for [!DNL Adobe Assets] – but the SSO is configured differently than [!DNL Workfront?]

Depois que [!DNL Workfront] for adicionado como um aplicativo [!DNL Admin Console], você não precisará fazer mais nada para [!DNL Workfront] para aproveitar a configuração de SSO existente para [!DNL Adobe Assets].

### Como isso afeta os configurados com SSO?

SSO está configurado no [!DNL Admin Console] e herdado pelo aplicativo [!DNL Workfront].

### O SSO com nosso [!DNL Active Directory] interno ainda será uma opção para o Identity Management System (IMS) da Adobe?

O IMS substitui o SSO e funciona basicamente da mesma maneira. Todas as permissões de usuário são concedidas e provisionadas em [!DNL Adobe Admin Console], e o usuário verá a tela de logon [!DNL Adobe], onde poderá escolher &quot;[!UICONTROL Conta Pessoal]&quot; ou &quot;[!UICONTROL Conta da Empresa]&quot; para fazer logon (se você tiver [!DNL Active Directory], a maioria fará logon com uma conta da empresa).

### Para aqueles que não estão usando SSO, a URL de logon [!DNL Workfront] muda?

O URL de logon será alterado; no entanto, o URL antigo será redirecionado para o novo URL de logon, para que você deve treinar novamente os usuários para onde ir.

### Os aliases configurados ainda funcionarão ou os links [!DNL Workfront] estão sendo alterados com essa migração?

[!DNL Workfront] redirecionamentos/aliases estão disponíveis para acessar a página inicial.

### Haverá um momento em que os redirecionamentos serão desativados? Or will we always be able to type in my.company.workfront.com?

You&#39;ll always be able to use any custom URLs. After you click any of those links, it will direct you to [!DNL Workfront] and show a different URL. No entanto, é melhor [!DNL experience] fazer logon em experience.adobe.com e marcar links de dentro de [!DNL Experience Cloud]. Less redirecting equals less lag time/loading time.

### Os links diretos para as filas de solicitações serão desfeitos?

Todos os links diretos devem ser redirecionados para os novos padrões de URL. No entanto, se você tiver distribuído links para pessoas, deverá enviar uma atualização para aproveitar o link direto e evitar atrasos no acesso à página esperada.

### Will we migrate to [!DNL Experience Cloud] globally or can we select for certain users (not all our users even use other Adobe products)?

The entire [!DNL Workfront] customer account will be migrated. It cannot be done on a user-by-user basis.

### Will all [!DNL Workfront] users have to log in via [!DNL Experience Cloud]? Or just administrators?

Yes, all users will log in via [!DNL Experience Cloud]. The Adobe Identity Management System (IMS) login will replace SSO. É uma experiência muito parecida, apenas uma tela de login diferente.

### Os usuários precisarão vincular suas contas do [!DNL Adobe] às suas contas do [!DNL Workfront] se já tiverem ambas?

Sim, há um processo para isso, e mais detalhes serão fornecidos quando for a hora de sua organização migrar para o IMS.

### O que acontece com os usuários do [!DNL Workfront] que não têm uma conta do [!DNL Adobe]?

Os usuários que não receberam acesso em [!DNL Adobe Admin Console] para entrar em [!DNL Workfront] devem criar uma “[!UICONTROL conta pessoal]” ou uma conta de ID [!DNL Adobe] para poderem fazer logon. Isso envia um email ao administrador para aprovar ou rejeitar a solicitação e, além disso, permite que o administrador configure o tipo de acesso que esse usuário tem. Ao fazer logon, eles acessarão experience.adobe.com, inserirão seus endereços de email e escolherão [!UICONTROL Conta Pessoal]. A partir daí, eles poderão acessar [!DNL Workfront].

### E se não tivermos nenhum produto do [!DNL Adobe] além do [!DNL Workfront?]

Ainda é recomendável que sua organização migre para o [!DNL Adobe Unified Experience]. Você receberá uma ID do [!DNL Adobe] juntamente com os benefícios listados acima.

### Temos usuários externos incluídos em nossa instância [!DNL Workfront]. Não queremos que eles tenham acesso a nenhum outro produto incluído no [!DNL Adobe]. Como limitaríamos o acesso deles dentro do console?

[!DNL Admin Console] dá aos administradores muito controle sobre o que os usuários podem ou não acessar. Sempre que um usuário externo quiser acesso, precisará criar uma ID do [!DNL Adobe], que envia um email para o administrador. O administrador pode então aceitar ou rejeitar o acesso a um produto e definir o que ele pode/não pode acessar para produtos de propriedade dessa organização. Em seguida, o Administrador do Sistema do [!DNL Workfront] pode acessar a área [!UICONTROL Usuários] do [!DNL Workfront] para criar permissões mais granulares para o usuário externo.

### Administradores de grupo são usados para criar pessoas em [!DNL Workfront]. Com a mudança para [!DNL Experience Cloud], os administradores de grupo ainda poderão criar pessoas?

Sim, a criação de usuários ainda é possível através de [!DNL Workfront]. Esses usuários podem ser adicionados a [!DNL Experience Cloud] automaticamente. Você também pode configurar seus administradores de grupo como proprietários de produtos no [!DNL Admin Console] para permitir que eles atribuam [!DNL Workfront] a usuários.

### Qual é o prazo para mudar para [!DNL Experience Cloud]?

Não há prazo no momento para mover para [!DNL Adobe Experience Cloud]. Estamos trabalhando com os clientes para permitir que eles escolham quando estiverem prontos para migrar.

### Nossa equipe de suporte precisará fazer algo para essa alteração?

Se a equipe de suporte for responsável pela criação de novos usuários, precisará se familiarizar com as interfaces [!DNL Admin Console] usadas para criar usuários e atribuir um direito ao Workfront. Caso contrário, provavelmente não haverá alterações significativas para sua equipe interna de suporte.

### Como isso afeta as integrações que temos por meio da função de API?

O caminho de URL existente continuará disponível para o tráfego da API. Não é necessário fazer nada para atualizar os endpoints nas integrações. No entanto, o logon direto por meio do nome de usuário e senha não será suportado - você deve usar uma chave de API, com a exceção de [!DNL Workfront Fusion] conectores.

### What about [!DNL Creative Cloud] users? How does the migration affect them? Are there any advantages for them?

There is no impact to [!DNL Creative Cloud] users with the migration to [!DNL Adobe Unified Experience].

### Os logons serão alterados para [!DNL Workfront] usuários de dispositivos móveis?

[!DNL Workfront] usuários móveis não devem ser afetados pela migração para [!DNL Adobe Unified Experience].

### O JumpSeat não está funcionando com o [!DNL Adobe Unified Experience]. Como posso resolver isso?

O JumpSeat funciona com [!DNL Adobe Unified Experience], mas requer uma atualização de configuração. Usando o painel de administração JumpSeat, altere a URL do aplicativo de `workfront.com` para terminar com `.workfront.adobe.com`
