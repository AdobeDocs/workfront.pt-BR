---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Experiência unificada do Adobe para perguntas frequentes
description: Alguns recursos são diferentes entre [!DNL Workfront] e Adobe Experience Cloud, e você pode ter algumas dúvidas como [!DNL Workfront] é migrada para a experiência unificada.
author: Lisa
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 0%

---

# [!DNL Adobe Unified Experience] Perguntas frequentes

O [!DNL Adobe Unified Experience] para [!DNL Workfront] permite gerenciar todos os [!DNL Adobe] aplicativos em um local com um único logon. O [!DNL Adobe] a área de navegação é integrada perfeitamente com [!DNL Workfront]. Alguns recursos são diferentes, e você pode ter algumas dúvidas ao [!DNL Workfront] é migrada para a experiência unificada.

Para obter informações sobre como fazer logon na [!DNL Adobe Unified Experience], consulte [[!DNL Adobe Unified Experience] para [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## Comparação de [!DNL Adobe Unified Experience] e [!DNL Workfront only] experiência

Somente clientes que usam o [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] pode acessar o [!DNL Adobe Unified Experience]. Os clientes que ainda não migraram verão a variável [!DNL Workfront only] sem a capacidade de alternar entre [!DNL Adobe] aplicativos.

Esta tabela descreve alguns recursos que diferem entre as duas experiências.

| [!DNL Adobe Unified Experience] | [!DNL Workfront] somente experiência |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] Menu principal] está à esquerda ![Menu principal](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront] Menu principal] está à direita ![Menu principal](assets/main-menu-icon.png) |
| Um único URL de logon está disponível para todos [!DNL Adobe Experience Cloud] aplicativos | Faça logon em [!DNL Workfront] com um [!DNL Workfront] URL |
| Um &quot;alternador de organização&quot; permite que você se mova entre [!DNL Workfront] organizações e ambientes | O &quot;alternador de organização&quot; não está disponível |
| A navegação inclui uma área de navegação de nível superior para [!DNL Adobe] produtos, [!DNL Adobe] notificações, ajuda e seu perfil de usuário, além do [!DNL Workfront] barra de navegação | A navegação inclui o [!DNL Workfront] somente barra de navegação |
| A ajuda pode ser acessada pelo [!UICONTROL Menu principal] e área de navegação superior | A ajuda pode ser acessada pelo [!UICONTROL Menu principal] e [!DNL Workfront] barra de navegação |

{style=&quot;table-layout:auto&quot;}

## Perguntas frequentes

**Como posso aprender mais sobre o [!DNL Adobe Admin Console]?**

Para obter informações sobre o [!DNL Admin Console], reveja estes artigos:

* [Prepare-se para a [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [Diferenças de administração baseadas em plataforma ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] visão geral](https://helpx.adobe.com/br/enterprise/using/admin-console.html)

**Como cliente, o que é necessário fazer para facilitar a migração?**

Os clientes existentes serão contatados para agendar migrações. Os colegas de suporte da equipe de migração guiarão os clientes pelo processo, recomendarão em [!DNL Admin Console] e forneça os links para a documentação necessária para tornar a mudança o mais simples e sem complicações possível.

* [[!DNL Adobe Workfront] Visão geral do suporte](https://experienceleague.adobe.com/docs/customer-one/using/workfront/overview.html)
* [[!DNL Workfront Admin Console] informações](https://experienceleague.adobe.com/docs/customer-one/using/workfront/landing.html)
* [[!DNL Adobe Business Platform] and [!DNL Admin Console] Perguntas frequentes](https://experienceleague.adobe.com/docs/customer-one/using/workfront/faq.html)

**Como você está lidando [!DNL Adobe Admin Console] para empresas que já têm isso ativado para IDs federadas de forma diferente do [!DNL Workfront] O SSO está configurado?**

[!DNL Adobe Admin Console] tem a opção de incluir [!DNL Workfront], substituindo SSO por IMS. Todo o provisionamento de usuário ocorre na [!DNL Admin Console]e os usuários verão a variável [!DNL Adobe] tela de logon para acessar [!DNL Experience Cloud] onde verão [!DNL Workfront] como uma opção (se lhes for concedido acesso a ela).

**Como isso afeta os clientes que já têm o painel de administração AEM para [!DNL Adobe Assets] - mas o SSO está configurado de forma diferente do[!DNL Workfront?]**

Uma vez [!DNL Workfront] é adicionado como um [!DNL Admin Console] aplicativo, você não deve ter que fazer mais nada por [!DNL Workfront] para aproveitar a configuração atual do SSO que você tem para [!DNL Adobe Assets].

**Como isso afeta aqueles configurados com SSO?**

O SSO é configurado no [!DNL Admin Console] e herdada pelo [!DNL Workfront] aplicativo.

**É o SSO com nossa [!DNL Active Directory] ainda será uma opção com o IMS?**

O IMS é um substituto do SSO e funciona principalmente da mesma forma. Todas as permissões de usuário são concedidas e provisionadas em [!DNL Adobe Admin Console]e o usuário visualizará a variável [!DNL Adobe] tela de login onde eles podem escolher &quot;[!UICONTROL Conta pessoal]&quot; ou &quot;[!UICONTROL Conta da Empresa]&quot; para fazer logon (se você tiver [!DNL Active Directory], a maioria fará logon com uma conta da empresa).

**Para aqueles que não usam SSO, o faz o [!DNL Workfront] alterar o URL de logon?**

O URL de logon será alterado; no entanto, o URL antigo será redirecionado para o novo URL de logon, portanto, você deve treinar novamente seus usuários para onde ir.

**Os aliases que configuramos ainda funcionarão ou serão [!DNL Workfront] links mudando com essa migração?**

[!DNL Workfront] redirecionamentos/aliases estão disponíveis para chegar à página inicial.

**Haverá um momento em que os redirecionamentos estão desativados? Ou sempre poderemos digitar my.company.workfront.com?**

Você sempre poderá usar quaisquer URLs personalizados. Depois de clicar em qualquer um desses links, você será direcionado para [!DNL Workfront] e mostrar um URL diferente. No entanto, é melhor [!DNL experience] para fazer logon em experience.adobe.com e marcar links de dentro [!DNL Experience Cloud]. Menos redirecionamento equivale a menos tempo de atraso/tempo de carregamento.

**Os links diretos para as filas de solicitação serão quebrados?**

Todos os links diretos devem redirecionar para os novos padrões de URL. No entanto, se tiver links distribuídos para pessoas, você deve enviar uma atualização para aproveitar o link direto e evitar atrasos na obtenção para a página esperada.

**Migraremos para [!DNL Experience Cloud] globalmente ou podemos selecionar para determinados usuários (nem todos os nossos usuários usam outros produtos do Adobe)?**

O todo [!DNL Workfront] a conta do cliente será migrada. Isso não pode ser feito usuários por usuários.

**Irá tudo [!DNL Workfront] os usuários precisam fazer logon via [!DNL Experience Cloud]? Ou apenas administradores?**

Sim, todos os usuários farão logon via [!DNL Experience Cloud]. O logon do IMS substituirá o SSO. É uma experiência muito semelhante, apenas uma tela de login diferente.

**Os usuários terão que vincular seus [!DNL Adobe] das suas contas [!DNL Workfront] contas, se já tiverem ambos?**

Sim, há um processo para isso e mais detalhes serão fornecidos quando chegar a hora de sua organização mudar para o IMS.

**O que acontece com o [!DNL Workfront] usuários que não têm um [!DNL Adobe] conta?**

Usuários aos quais não foi concedido acesso em [!DNL Adobe Admin Console] para entrar em [!DNL Workfront] deve criar um &quot;[!UICONTROL conta pessoal]&quot; ou um [!DNL Adobe] Conta de ID para fazer logon. Isso envia um email ao administrador para aprovar ou rejeitar sua solicitação e também permite que o administrador configure o tipo de acesso que esse usuário tem. Ao fazer logon, eles irão para experience.adobe.com, inserirão seu endereço de email e escolherão [!UICONTROL Conta pessoal]. A partir daí, eles poderão acessar [!DNL Workfront].

**E se não tivermos nenhuma [!DNL Adobe] produtos que não[!DNL Workfront?]**

Ainda é recomendável que sua organização migre para o [!DNL Adobe Unified Experience]. Você receberá um [!DNL Adobe] ID juntamente com os benefícios listados acima.

**Temos usuários externos incluídos em [!DNL Workfront] instância. Não gostaríamos que eles tivessem acesso a outros produtos incluídos no [!DNL Adobe]. Como limitar o acesso deles no console?**

[!DNL Admin Console] oferece aos administradores muito controle sobre o que os usuários podem ou não acessar. Sempre que um usuário externo quiser acesso, ele precisará criar um [!DNL Adobe] ID, que envia um email para o administrador. Em seguida, o administrador pode aceitar ou rejeitar o acesso a um produto e definir o que ele pode ou não acessar para os produtos de propriedade dessa organização. Então, o [!DNL Workfront] O Administrador do sistema pode acessar [!UICONTROL Usuários] área de [!DNL Workfront] para tornar as permissões mais granulares para o usuário externo.

**Administradores de grupo são usados para criar pessoas no [!DNL Workfront]. Com a mudança para [!DNL Experience Cloud], os administradores de grupo ainda poderão criar pessoas?**

Sim, a criação do usuário ainda é possível por meio de [!DNL Workfront]. Esses usuários podem ser adicionados a [!DNL Experience Cloud] automaticamente. Você também pode configurar os administradores do grupo como proprietários de produtos no [!DNL Admin Console] para permitir que eles atribuam [!DNL Workfront] aos usuários.

**Qual é o prazo para mudar para [!DNL Experience Cloud]?**

No momento, não há prazo para mudar para [!DNL Adobe Experience Cloud]. Estamos trabalhando com clientes para que eles escolham quando estão prontos para mudar.

**Será que a nossa equipe de apoio terá de fazer alguma coisa para esta mudança?**

Se a equipe de suporte for responsável pela criação de novos usuários, eles precisarão se familiarizar com o [!DNL Admin Console] interfaces usadas para criar usuários e atribuir um direito ao Workfront. Caso contrário, provavelmente não haverá mudanças significativas para sua equipe interna de suporte.

**Como isso afeta as integrações que temos por meio da função da API?**

O caminho do URL existente continuará disponível para o tráfego da API. Não é necessário fazer nada para atualizar os pontos de extremidade em suas integrações. No entanto, o logon direto por meio do nome de usuário e da senha não será suportado - é necessário usar uma chave de API, com a exceção de [!DNL Workfront Fusion] conectores.

**E sobre [!DNL Creative Cloud] usuários? Como a migração os afeta? Existem vantagens para eles?**

Não há impacto para [!DNL Creative Cloud] usuários com migração para [!DNL Adobe Unified Experience].

**Os logons serão alterados para [!DNL Workfront] usuários móveis?**

[!DNL Workfront] os usuários móveis não devem ser afetados pela migração para [!DNL Adobe Unified Experience].
