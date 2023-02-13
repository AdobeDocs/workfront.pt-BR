---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Solução de problemas - [!DNL Workfront Proof] visualizador de prova
description: Se o conteúdo de prova não estiver sendo carregado e você só puder ver um visualizador de prova vazio, é provável que algo esteja bloqueando essa ação localmente. Experimente as soluções possíveis abaixo.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ce463565-d21e-4dbc-8de8-78bcbf16fb2c
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1278'
ht-degree: 0%

---

# Solução de problemas - [!DNL Workfront Proof] visualizador de prova

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

Se o conteúdo de prova não estiver sendo carregado e você só puder ver um visualizador de prova vazio, é provável que algo esteja bloqueando essa ação localmente. Experimente as soluções possíveis abaixo.

## Verifique seu navegador e [!DNL Flash Player] Versões estão atualizadas

Todos os desenvolvedores trabalham constantemente em seus aplicativos e lançam regularmente novos recursos e correções para seus produtos. Isso é para melhorar a experiência do usuário e manter o nível de segurança, para que seja a prática recomendada usar somente as versões mais recentes. Isso também ajuda a evitar conflitos entre os aplicativos.

### [!DNL Flash Player] Versão do plug-in

Para verificar seu [!DNL Flash Player] visita a versão do [[!DNL Adobe] site](http://www.adobe.com/software/flash/about/).

![ProofView_2.png](assets/proofview-2-350x199.png)

Se o número da sua versão for diferente do listado para a sua plataforma, acesse [[!DNL Flash Player] página de download](http://get.adobe.com/flashplayer/otherversions/) e obtenha a versão mais recente.

Observe: recomendamos usar o original [!DNL Adobe] assim, se o navegador usar uma solução integrada, desative-a e instale o plug-in [!DNL Adobe] solução.

### Versão do navegador

Atualmente, a maioria dos navegadores é atualizada automaticamente, mas se você estiver tendo problemas, vale a pena verificar qual versão está usando e fazer a atualização, se necessário.

No seu navegador, acesse [!UICONTROL Menu] e localize a [!UICONTROL Sobre] (em alguns casos, isso pode estar visível em [!UICONTROL Ajuda] ). No [!UICONTROL Sobre] você encontrará informações sobre a versão atual do navegador e também uma opção para atualizar/verificar atualizações.

Consulte no Chrome:

![ProofView_3.png](assets/proofview-3-350x206.png)

Assim que tiver o mais recente [!DNL Flash Player] versão do plug-in e do navegador instalada tenta reabrir sua prova e ver se o problema foi resolvido.

## Certifique-se de que seu local [!DNL Flash] O armazenamento está disponível

Nosso [!DNL Workfront Proof] O visualizador é baseado no Flash e armazenamos alguns dados sobre as provas (ou seja, comentários, blocos de prova, [!DNL Workfront Proof] Configurações do visualizador) no seu computador usando [!DNL Flash Player]. Se a variável [!DNL Workfront Proof] O visualizador é aberto, mas não há conteúdo dentro de você, para garantir que o Armazenamento do Flash esteja disponível em sua máquina e que [!DNL Workfront Proof] está autorizado a usá-lo.

Se houver algum armazenamento alocado, mas você estiver trabalhando com as provas maiores com várias páginas e os comentários tentarem aumentar a [!DNL Flash] Armazene e recarregue sua prova.

Consulte a [Problemas ao exibir provas - [!DNL Flash] Objetos compartilhados explicados](../../../workfront-proof/wp-tech-corner/troubleshooting/view-proof-flash-shared-object.md) para obter instruções detalhadas.

## Identifique onde o problema está

* As provas estão abrindo em um navegador diferente?
* Se você estiver usando um navegador diariamente e estiver tendo problemas para visualizar as provas, tente abrir a mesma prova em um navegador diferente no seu computador. Para fazer isso, basta copiar o link de prova da barra de URL do navegador principal e colá-lo em um navegador diferente. Se a prova for aberta, revise a configuração, os plug-ins e as extensões do navegador principal, pois podem estar interferindo.
* Não temos navegador preferível, mas se você tiver problemas de desempenho em seu navegador atual, recomendamos mudar para um navegador diferente.
* As provas estão abrindo em uma máquina diferente na sua localização?
Se a prova não estiver sendo aberta em nenhum navegador da máquina, tente abri-la em um computador diferente na sua localização e/ou fora dela. Isso permitirá determinar se um problema está relacionado a uma máquina específica ou se é algo em sua rede local.
Se o seu nível de segurança for maior, suas conexões com o [!DNL Workfront Proof] pode ser bloqueado por:

   * Seu software AV local
   * Sua solução de segurança de rede
   * Configuração de DNS, firewall ou proxy
   * Essas são as configurações que estão fora de nosso controle. Há várias soluções de segurança disponíveis e não podemos dizer quais são implementadas em sua rede e quais podem estar bloqueando conexões com o [!DNL Workfront Proof]. Também não cabe [!DNL Workfront Proof] para decidir sobre sua configuração de segurança interna. Se tiver problemas ao abrir as provas em várias máquinas na sua localização/rede, recomendamos que entre em contato com a sua equipe de TI para que ela possa verificar as configurações de rede e autorizar ou adicionar o [!DNL Workfront Proof] à lista de permissões, se necessário.

* As conexões com o [!DNL Workfront Proof] permitido na sua rede?
Dentro do Visualizador de prova, carregamos os blocos - fragmentos das páginas. Se esse conteúdo não carregar bem em sua extremidade, pode ser que algumas conexões com o [!DNL Workfront Proof] estão bloqueadas na sua rede. Certifique-se de que todas as conexões e todo o conteúdo de *.proofhq.com sejam adicionados à  de lista de permissões. Sua equipe de TI deve ser capaz de ajudar a verificar isso.

## Rever plug-ins

Se seu navegador e [!DNL Flash Player] O plug-in está atualizado e sua rede não está bloqueando as conexões com o [!DNL Workfront Proof] pode haver algo no seu navegador que esteja afetando a exibição das provas. Atualmente, há vários plug-ins e extensões disponíveis no navegador e alguns deles interferem ou estão em conflito com os outros.

A prática recomendada é remover todos os complementos desconhecidos e manter somente os que você usa e em que confia. Cada navegador deve fornecer opções para marcar/modificar/excluir os plug-ins e as extensões. Nosso [!DNL Workfront Proof] O visualizador é baseado em [!DNL Flash] e usamos o JavaScript para carregar o visualizador para que você deseje revisar especialmente os plug-ins que podem afetar eles.

Visite as páginas listadas abaixo para obter instruções mais detalhadas dos desenvolvedores sobre como desativar os complementos do navegador:

* Chrome: [plugins](https://support.google.com/chrome/answer/142064?hl=en-GB) / [extensões](https://support.google.com/chrome/answer/113907?hl=en-GB)
* Firefox: [complementos](https://support.mozilla.org/en-US/kb/disable-or-remove-add-ons)
* Internet Explorer: [complementos](http://windows.microsoft.com/en-GB/internet-explorer/manage-add-ons#ie=ie-11)
* Safari: [complementos](http://support.apple.com/en-gb/HT203353)

Se houver algum complemento específico interferindo no carregamento das provas, tente verificar os detalhes no console do navegador.

![ProofView_4.png](assets/proofview-4-350x57.png)

Na maioria dos navegadores mais recentes, há algumas ferramentas adicionais de desenvolvedores disponíveis e elas podem ser usadas para solução de problemas mais avançada.

Se estiver tendo problemas com a exibição das provas:

* Abra o console do navegador e recarregue a prova.
* Verifique se há alertas ou mensagens no console. Esses detalhes podem ajudar a identificar a causa raiz dos problemas.
* Peça à sua equipe de TI que analise os resultados. Devem poder aconselhar e ajudar a resolver o problema local.
* Compartilhe os resultados com nosso [Equipe de suporte](https://support.workfront.com/hc/en-us/requests/new). Teremos todo o prazer em ajudar.

Se não souber como abrir o console no navegador, consulte as etapas gravadas:

* [Firefox](http://screencast.com/t/eP6FRtk4vxWS)
* [Internet Explorer](http://screencast.com/t/bYzq1iQv)
* [Google Chrome](http://screencast.com/t/2anpeAzOOyj)
* [Safari](http://screencast.com/t/rnOvgl3GidjL)

Você também pode verificar a documentação do desenvolvedor do navegador para obter instruções mais detalhadas.

## Verificar configurações de conteúdo misto

Todas as conexões com [!DNL Workfront Proof] são por HTTPS. No entanto, no [!DNL Workfront Proof] No visualizador, carregamos os blocos por HTTP e os dados são protegidos com os tokens. Isso cria conteúdo misto, que pode estar bloqueando alguns dos navegadores ou soluções de segurança (por padrão ou de acordo com a configuração manual).

Se esse for o motivo pelo qual as provas não estão sendo abertas em seu computador (você deve ser capaz de ver os alertas relevantes no console do navegador) autorize essas conexões para [!DNL Workfront Proof] ou altere suas configurações para permitir conteúdo misto passivo em sua máquina. O conteúdo misto pode ser bloqueado pelo navegador, software AV, configuração de rede etc. para determinar a causa exata, entre em contato com a equipe de TI/administradores de rede. Eles também devem ser capazes de ajudar na ativação do conteúdo misto no computador.

Entre em contato com nosso [Equipe de suporte](https://support.workfront.com/hc/en-us/requests/new) se precisar de assistência do nosso lado.
