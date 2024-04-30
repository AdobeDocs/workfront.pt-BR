---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Experiência unificada do Adobe para perguntas frequentes
description: Alguns recursos são diferentes entre [!DNL Workfront] e Adobe Experience Cloud, e você pode ter algumas perguntas como [!DNL Workfront] é migrada para a experiência unificada.
author: Nolan
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '1289'
ht-degree: 0%

---

# [!DNL Adobe Unified Experience] Perguntas frequentes

A variável [!DNL Adobe Unified Experience] para [!DNL Workfront] O permite gerenciar todos os seus [!DNL Adobe] aplicativos em um único local com um único logon. A variável [!DNL Adobe] de navegação está integrado perfeitamente com [!DNL Workfront]. Alguns recursos são diferentes e você pode ter algumas perguntas como [!DNL Workfront] é migrada para a experiência unificada.

Para obter informações sobre como fazer logon na [!DNL Adobe Unified Experience], consulte [[!DNL Adobe Unified Experience] para [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## Comparação de [!DNL Adobe Unified Experience] e [!DNL Workfront only] experiência

Somente clientes que usam o [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] pode acessar o [!DNL Adobe Unified Experience]. Os clientes que ainda não migraram verão a [!DNL Workfront only] experiência, sem a capacidade de alternar entre [!DNL Adobe] aplicativos.

Esta tabela descreve alguns recursos que diferem entre as duas experiências.

| [!DNL Adobe Unified Experience] | [!DNL Workfront] somente experiência |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] Menu principal] está à esquerda ![Menu principal](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront] Menu principal] está à direita ![Menu principal](assets/main-menu-icon.png) |
| Um único URL de logon está disponível para todos [!DNL Adobe Experience Cloud] aplicativos | Efetue logon no [!DNL Workfront] com um personalizado [!DNL Workfront] URL |
| Um &quot;alternador de organização&quot; permite mover entre [!DNL Workfront] organizações e ambientes | O &quot;alternador de organização&quot; não está disponível |
| A navegação inclui uma área de navegação de nível superior para [!DNL Adobe] produtos, [!DNL Adobe] notificações, ajuda e perfil do usuário, além da [!DNL Workfront] barra de navegação | A navegação inclui o [!DNL Workfront] somente barra de navegação |
| A ajuda pode ser acessada pelo [!UICONTROL Menu principal] e área de navegação superior | A ajuda pode ser acessada pelo [!UICONTROL Menu principal] e [!DNL Workfront] barra de navegação |

{style="table-layout:auto"}

## Perguntas frequentes

### Como determinar se estou usando a Experiência unificada do Adobe ou o Adobe Workfront?

Para determinar se sua organização está no Adobe Unified Experience, examine o URL que você usa para acessar o Workfront.

| URL | Experiência do Adobe |
|------------|------------|
| (NomeEmpresa).my.workfront.com | experiência com o Workfront |
| experience.adobe.com | Experiência unificada do Adobe |

### Como posso saber mais sobre o [!DNL Adobe Admin Console]?

Para obter informações sobre o [!DNL Admin Console], leia estes artigos:

* [Prepare-se para o [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [Diferenças de administração baseadas em plataforma ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] visão geral](https://helpx.adobe.com/br/enterprise/using/admin-console.html)

### O que eu, como cliente, preciso fazer para facilitar a migração?

Os clientes existentes serão contatados para agendar as migrações. Os colegas de suporte da equipe de migração guiarão os clientes pelo processo, darão conselhos sobre [!DNL Admin Console] e fornecer links para a documentação necessária para tornar a mudança o mais simples e simples possível.

* [[!DNL Adobe Workfront] Visão geral do suporte](https://experienceleague.adobe.com/docs/customer-one/using/workfront/overview.html)
* [[!DNL Workfront Admin Console] informações](https://experienceleague.adobe.com/docs/customer-one/using/workfront/landing.html)
* [[!DNL Adobe Business Platform] e [!DNL Admin Console] Perguntas frequentes](https://experienceleague.adobe.com/docs/customer-one/using/workfront/faq.html)

### Como você está lidando com [!DNL Adobe Admin Console] para empresas que já têm esse recurso habilitado para IDs federadas de forma diferente da [!DNL Workfront] SSO configurado?

[!DNL Adobe Admin Console] tem a opção de incluir [!DNL Workfront], substituindo SSO por IMS. Todo o provisionamento de usuários acontece no [!DNL Admin Console], e os usuários verão a variável [!DNL Adobe] tela de logon para acessar o [!DNL Experience Cloud] onde verão [!DNL Workfront] como opção (se tiverem acesso a ela).

### Como isso afeta os clientes que já têm o painel de administração do AEM para [!DNL Adobe Assets] - mas o SSO é configurado de forma diferente da [!DNL Workfront?]

Uma vez [!DNL Workfront] é adicionado como um [!DNL Admin Console] aplicativo, não é necessário fazer mais nada para [!DNL Workfront] para aproveitar a configuração de SSO existente para [!DNL Adobe Assets].

### Como isso afeta os configurados com SSO?

O SSO está configurado no [!DNL Admin Console] e herdado pela [!DNL Workfront] aplicação.

### É SSO com nosso interno [!DNL Active Directory] ainda será uma opção com o IMS?

O IMS substitui o SSO e funciona basicamente da mesma maneira. Todas as permissões do usuário são concedidas e provisionadas no [!DNL Adobe Admin Console], e o usuário verá a variável [!DNL Adobe] tela de logon onde eles podem escolher &quot;[!UICONTROL Conta pessoal]&quot; ou &quot;[!UICONTROL Conta da Empresa]&quot; para fazer logon (se você tiver [!DNL Active Directory], a maioria fará logon com uma conta da empresa).

### Para aqueles que não estão usando SSO, o [!DNL Workfront] alteração do URL de logon?

O URL de logon será alterado; no entanto, o URL antigo será redirecionado para o novo URL de logon, para que você deve treinar novamente os usuários para onde ir.

### Os aliases configurados ainda funcionarão ou serão [!DNL Workfront] links mudando com esta migração?

[!DNL Workfront] redirecionamentos/aliases estão disponíveis para acessar a página inicial.

### Haverá um momento em que os redirecionamentos serão desativados? Ou sempre poderemos digitar my.company.workfront.com?

Você sempre poderá usar URLs personalizados. Depois de clicar em qualquer um desses links, ele direcionará você para [!DNL Workfront] e mostrar um URL diferente. No entanto, é melhor [!DNL experience] para fazer logon em experience.adobe.com e marcar links em [!DNL Experience Cloud]. Menos redirecionamento equivale a menos tempo de atraso/tempo de carregamento.

### Os links diretos para as filas de solicitações serão desfeitos?

Todos os links diretos devem redirecionar para os novos padrões de URL. No entanto, se você tiver distribuído links para pessoas, deverá enviar uma atualização para aproveitar o link direto e evitar atrasos para chegar à página esperada.

### Migraremos para o [!DNL Experience Cloud] globalmente ou podemos selecionar para determinados usuários (nem todos os nossos usuários usam outros produtos Adobe)?

Todo o [!DNL Workfront] A conta do cliente será migrada. Isso não pode ser feito em uma base usuário por usuário.

### Será que [!DNL Workfront] os usuários precisam fazer logon via [!DNL Experience Cloud]? Ou apenas administradores?

Sim, todos os usuários farão logon via [!DNL Experience Cloud]. O logon IMS substituirá o SSO. É uma experiência muito semelhante, apenas uma tela de logon diferente.

### Os usuários terão que vincular seus [!DNL Adobe] para as suas [!DNL Workfront] contas se elas já tiverem ambas?

Sim, há um processo para isso, e mais detalhes serão fornecidos quando for a hora de sua organização migrar para o IMS.

### O que acontece com o [!DNL Workfront] usuários que não têm um [!DNL Adobe] conta?

Usuários que não receberam acesso no [!DNL Adobe Admin Console] para entrar no [!DNL Workfront] deve criar um &quot;[!UICONTROL conta pessoal]&quot; ou um [!DNL Adobe] Conta de ID para fazer logon. Isso envia um email ao administrador para aprovar ou rejeitar a solicitação e, além disso, permite que o administrador configure o tipo de acesso que esse usuário tem. Ao fazer logon, eles vão para experience.adobe.com, inserem seu endereço de email e escolhem [!UICONTROL Conta pessoal]. A partir daí, eles poderão acessar [!DNL Workfront].

### E se não tivermos nenhum [!DNL Adobe] outros produtos que não [!DNL Workfront?]

Ainda é recomendável que sua organização migre para a [!DNL Adobe Unified Experience]. Você receberá um [!DNL Adobe] junto com os benefícios listados acima.

### Temos usuários externos incluídos em nosso [!DNL Workfront] instância. Não queremos que eles tenham acesso a nenhum outro produto incluído na [!DNL Adobe]. Como limitaríamos o acesso deles dentro do console?

[!DNL Admin Console] O fornece aos administradores muito controle sobre o que os usuários podem ou não acessar. Sempre que um usuário externo desejar acesso, ele precisará criar um [!DNL Adobe] ID, que envia um email para o administrador. O administrador pode então aceitar ou rejeitar o acesso a um produto e definir o que ele pode/não pode acessar para produtos de propriedade dessa organização. Em seguida, a variável [!DNL Workfront] O administrador do sistema pode entrar no [!UICONTROL Usuários] área de [!DNL Workfront] para criar permissões mais granulares para o usuário externo.

### Administradores de grupo são usados para criar pessoas no [!DNL Workfront]. Com a mudança para [!DNL Experience Cloud], os administradores de grupo ainda poderão criar pessoas?

Sim, a criação de usuários ainda é possível por meio do [!DNL Workfront]. Esses usuários podem ser adicionados a [!DNL Experience Cloud] automaticamente. Você também pode configurar seus administradores de grupo como proprietários de produtos na [!DNL Admin Console] para permitir que eles atribuam [!DNL Workfront] aos usuários.

### Qual é o prazo para mudar para o [!DNL Experience Cloud]?

No momento, não há prazo para mudar para [!DNL Adobe Experience Cloud]. Estamos trabalhando com os clientes para permitir que eles escolham quando estiverem prontos para migrar.

### Nossa equipe de suporte precisará fazer algo para essa alteração?

Se a equipe de suporte for responsável por criar novos usuários, será necessário que eles se familiarizem com o [!DNL Admin Console] interfaces usadas para criar usuários e atribuir um direito ao Workfront. Caso contrário, provavelmente não haverá alterações significativas para sua equipe interna de suporte.

### Como isso afeta as integrações que temos por meio da função de API?

O caminho de URL existente continuará disponível para o tráfego da API. Não é necessário fazer nada para atualizar os endpoints nas integrações. No entanto, o login direto por meio do nome de usuário e senha não será suportado - você deve usar uma chave de API, com a exceção de [!DNL Workfront Fusion] conectores.

### E quanto ao [!DNL Creative Cloud] usuários? Como a migração os afeta? Há vantagens para eles?

Não há impacto para [!DNL Creative Cloud] usuários com a migração para [!DNL Adobe Unified Experience].

### Os logons serão alterados para [!DNL Workfront] usuários de dispositivos móveis?

[!DNL Workfront] usuários móveis não devem ser afetados pela migração para o [!DNL Adobe Unified Experience].
