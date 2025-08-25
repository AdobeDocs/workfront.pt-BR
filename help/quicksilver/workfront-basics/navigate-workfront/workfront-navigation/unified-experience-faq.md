---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Perguntas frequentes sobre a experiência unificada da Adobe
description: Alguns recursos são diferentes entre o [!DNL Workfront] e o Adobe Experience Cloud, e você pode ter algumas dúvidas à medida que sua instância do [!DNL Workfront] for migrada para a experiência unificada.
author: Nolan
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: a25eb28800ca8bbeeffedb521b3d72c8df71c697
workflow-type: tm+mt
source-wordcount: '1397'
ht-degree: 0%

---

# [!DNL Adobe Unified Experience] Perguntas frequentes

O [!DNL Adobe Unified Experience] for [!DNL Workfront] permite gerenciar todos os aplicativos do [!DNL Adobe] em um único local. A área de navegação do [!DNL Adobe] é perfeitamente integrada ao [!DNL Workfront]. Alguns recursos são diferentes e você pode ter algumas dúvidas à medida que a instância do [!DNL Workfront] for migrada para a experiência unificada.

Para obter informações sobre como fazer logon no [!DNL Adobe Unified Experience], consulte [[!DNL Adobe Unified Experience] for [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## Comparação da experiência [!DNL Adobe Unified Experience] e [!DNL Workfront only]

Somente os clientes que usam o [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] podem acessar o [!DNL Adobe Unified Experience]. Os clientes que ainda não migraram verão a experiência [!DNL Workfront only], sem a capacidade de alternar entre os aplicativos [!DNL Adobe].

Esta tabela descreve alguns recursos que diferem entre as duas experiências.

| [!DNL Adobe Unified Experience] | Somente experiência [!DNL Workfront] |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] O Menu Principal] está à esquerda de ![Menu Principal](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront] O Menu Principal] está à direita de ![Menu Principal](assets/main-menu-icon.png) |
| Uma única URL de logon está disponível para todos os aplicativos do [!DNL Adobe Experience Cloud] | Fazer logon em [!DNL Workfront] com uma URL [!DNL Workfront] personalizada |
| Um &quot;alternador de organização&quot; permite mover entre [!DNL Workfront] organizações e ambientes | O &quot;alternador de organização&quot; não está disponível |
| A navegação inclui uma área de navegação de nível superior para [!DNL Adobe] produtos, [!DNL Adobe] notificações, ajuda e seu perfil de usuário, além da barra de navegação [!DNL Workfront] | A navegação inclui somente a barra de navegação [!DNL Workfront] |
| A ajuda pode ser acessada pelo [!UICONTROL Menu Principal] e pela área de navegação superior | A ajuda pode ser acessada pelo [!UICONTROL Menu Principal] e pela barra de navegação [!DNL Workfront] |
| O visualizador de provas é aberto em uma nova guia | O visualizador de provas é aberto dentro do Workfront |
| A URL usada para acessar o Workfront é `experience.adobe.com` | A URL usada para acessar o Workfront é `(CompanyName).my.workfront.com` |
| O formato da data (como MM/DD/AAAA) é baseado nas configurações de idioma da Experiência unificada. Se o usuário não atualizou as configurações de idioma, as configurações `en-US` serão usadas. | O formato da data (como MM/DD/AAAA) é baseado nas preferências do navegador |

{style="table-layout:auto"}

## Perguntas frequentes

### Como determinar se estou usando a Experiência unificada do Adobe ou o Adobe Workfront?

Para determinar se sua organização está na Experiência unificada da Adobe, examine o URL usado para acessar o Workfront.

| URL | Experiência do Adobe |
|------------|------------|
| (NomeEmpresa).my.workfront.com | experiência com o Workfront |
| experience.adobe.com | Experiência unificada da Adobe |

### Como posso obter mais informações sobre o [!DNL Adobe Admin Console]?

Para obter informações sobre o [!DNL Admin Console], leia estes artigos:

* [Preparar para o(a) [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [Diferenças de administração baseadas em plataforma ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] visão geral](https://helpx.adobe.com/br/enterprise/using/admin-console.html)

### O que eu, como cliente, preciso fazer para facilitar a migração?

Os clientes existentes serão contatados para agendar as migrações. Os colegas de suporte da equipe de migração guiarão os clientes pelo processo, orientarão a configuração do [!DNL Admin Console] e fornecerão links para a documentação necessária para tornar a mudança o mais simples e simples possível.

* [[!DNL Adobe Workfront] Visão geral do suporte](https://experienceleague.adobe.com/pt-br/docs/customer-one/using/workfront/overview)
* [[!DNL Workfront Admin Console] informações](https://experienceleague.adobe.com/pt-br/docs/customer-one/using/workfront/landing)
* [[!DNL Adobe Business Platform] e [!DNL Admin Console] Perguntas frequentes](https://experienceleague.adobe.com/pt-br/docs/customer-one/using/workfront/faq)

### Como você está lidando com [!DNL Adobe Admin Console] para empresas que já têm isso habilitado para IDs federadas de forma diferente da configuração do SSO [!DNL Workfront]?

[!DNL Adobe Admin Console] tem a opção de incluir [!DNL Workfront], substituindo SSO pelo Identity Management System (IMS) da Adobe. Todo o provisionamento de usuários acontece no [!DNL Admin Console], e os usuários verão a tela de logon [!DNL Adobe] chegar ao [!DNL Experience Cloud], onde verão [!DNL Workfront] como uma opção (se tiverem acesso a ela).

### Como isso afeta os clientes que já têm o painel de administração do AEM para [!DNL Adobe Assets], mas o SSO é configurado de forma diferente do [!DNL Workfront?]

Depois que [!DNL Workfront] for adicionado como um aplicativo [!DNL Admin Console], você não precisará fazer mais nada para [!DNL Workfront] para aproveitar a configuração de SSO existente para [!DNL Adobe Assets].

### Como isso afeta os configurados com SSO?

SSO está configurado no [!DNL Admin Console] e herdado pelo aplicativo [!DNL Workfront].

### O SSO com nosso [!DNL Active Directory] interno ainda será uma opção para o Identity Management System (IMS) da Adobe?

O IMS substitui o SSO e funciona basicamente da mesma maneira. Todas as permissões de usuário são concedidas e provisionadas em [!DNL Adobe Admin Console], e o usuário verá a tela de logon [!DNL Adobe], onde poderá escolher &quot;[!UICONTROL Conta Pessoal]&quot; ou &quot;[!UICONTROL Conta da Empresa]&quot; para fazer logon (se você tiver [!DNL Active Directory], a maioria fará logon com uma conta da empresa).

### Para aqueles que não estão usando SSO, a URL de logon [!DNL Workfront] muda?

O URL de logon será alterado; no entanto, o URL antigo será redirecionado para o novo URL de logon, para que você deve treinar novamente os usuários para onde ir.

### Os aliases configurados ainda funcionarão ou os links [!DNL Workfront] estão sendo alterados com essa migração?

[!DNL Workfront] redirecionamentos/aliases estão disponíveis para acessar a página inicial.

### Haverá um momento em que os redirecionamentos serão desativados? Ou sempre poderemos digitar my.company.workfront.com?

Você sempre poderá usar URLs personalizados. Após clicar em qualquer um desses links, você será direcionado para [!DNL Workfront] e exibirá uma URL diferente. No entanto, é melhor [!DNL experience] fazer logon em experience.adobe.com e marcar links de dentro de [!DNL Experience Cloud]. Menos redirecionamento equivale a menos tempo de atraso/tempo de carregamento.

### Os links diretos para as filas de solicitações serão desfeitos?

Todos os links diretos devem redirecionar para os novos padrões de URL. No entanto, se você tiver distribuído links para pessoas, deverá enviar uma atualização para aproveitar o link direto e evitar atrasos para chegar à página esperada.

### Migraremos para o [!DNL Experience Cloud] globalmente ou podemos selecionar para determinados usuários (nem todos os nossos usuários usam outros produtos da Adobe)?

A conta de cliente [!DNL Workfront] inteira será migrada. Isso não pode ser feito em uma base usuário por usuário.

### Todos os [!DNL Workfront] usuários terão que fazer login via [!DNL Experience Cloud]? Ou apenas administradores?

Sim, todos os usuários farão logon via [!DNL Experience Cloud]. O logon do Adobe Identity Management System (IMS) substituirá o SSO. É uma experiência muito semelhante, apenas uma tela de logon diferente.

### Os usuários terão que vincular suas contas do [!DNL Adobe] às suas contas do [!DNL Workfront] se já tiverem ambas?

Sim, há um processo para isso, e mais detalhes serão fornecidos quando for a hora de sua organização migrar para o IMS.

### O que acontece com os usuários [!DNL Workfront] que não têm uma conta [!DNL Adobe]?

Os usuários aos quais não foi concedido acesso em [!DNL Adobe Admin Console] para entrar em [!DNL Workfront] devem criar uma &quot;[!UICONTROL conta pessoal]&quot; ou uma conta de ID [!DNL Adobe] para poderem fazer logon. Isso envia um email ao administrador para aprovar ou rejeitar a solicitação e, além disso, permite que o administrador configure o tipo de acesso que esse usuário tem. Ao fazer logon, eles irão para experience.adobe.com, digitarão seu endereço de email e escolherão [!UICONTROL Conta pessoal]. A partir daí, eles poderão acessar [!DNL Workfront].

### E se não tivermos nenhum produto do [!DNL Adobe] diferente do [!DNL Workfront?]

Ainda é recomendável que sua organização migre para o [!DNL Adobe Unified Experience]. Você receberá uma ID de [!DNL Adobe] juntamente com os benefícios listados acima.

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

### E quanto aos usuários [!DNL Creative Cloud]? Como a migração os afeta? Há vantagens para eles?

Não há impacto para [!DNL Creative Cloud] usuários com a migração para [!DNL Adobe Unified Experience].

### Os logons serão alterados para [!DNL Workfront] usuários de dispositivos móveis?

[!DNL Workfront] usuários móveis não devem ser afetados pela migração para [!DNL Adobe Unified Experience].

### O JumpSeat não está funcionando com o [!DNL Adobe Unified Experience]. Como posso resolver isso?

O JumpSeat funciona com [!DNL Adobe Unified Experience], mas requer uma atualização de configuração. Usando o painel de administração JumpSeat, altere a URL do aplicativo de `workfront.com` para terminar com `.workfront.adobe.com`
