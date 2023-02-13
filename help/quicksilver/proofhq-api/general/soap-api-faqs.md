---
title: Perguntas frequentes sobre API SOAP
description: Perguntas frequentes sobre API SOAP
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
exl-id: fcf89bd6-0e07-42a7-9ae3-9a1309e51946
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 0%

---

# Perguntas frequentes sobre API SOAP

## Como criar minha primeira prova de arquivo?

Ela executa três etapas simples:

**Etapa 1**: Faça upload do arquivo para a Workfront Proof enviando-o por meio de uma solicitação de publicação para  [https://soap.proofhq.com/upload.php](https://soap.proofhq.com/upload.php). Nós lhe devolveremos o hash do arquivo - isso é muito importante! Observe que nesse estágio você não verá nada em sua conta, tudo o que você fez até agora é enviar o arquivo, mas não nos disse o que fazer com ele.

**Etapa 2**: Se você ainda não tiver uma ID de sessão, obtenha-a usando os métodos doLogin() ou getSessionID() . Use a primeira para &quot;fazer logon&quot; usando o endereço de email e a senha de um usuário, ou o último método, se você tiver o endereço de email e o token de autenticação do usuário.

**Etapa 3:** Agora é hora de criar sua prova. Use o método createProof() e envie pelo menos os campos obrigatórios (atualmente, há apenas 5 deles). Defina o parâmetro Hash como o hash do arquivo retornado durante a &quot;Etapa 1&quot;, pois assim podemos determinar qual arquivo usar ao criar sua prova.

Agora, se você fizer logon em sua conta, verá a prova.

## Como criar minha primeira prova de instantâneo da Web?

São necessárias duas etapas simples:

**Etapa 1**: Se você ainda não tiver uma ID de sessão, obtenha uma usando os métodos doLogin() ou getSessionID() . Use a primeira para &quot;fazer logon&quot; usando o endereço de email e a senha de um usuário, ou o último método, se você tiver o endereço de email e o token de autenticação do usuário.

**Etapa 2:**Agora é hora de criar sua prova. Use o método createProof() e envie pelo menos os campos obrigatórios (atualmente, há apenas 5 deles). Defina o parâmetro Hash como &quot;Web&quot; e o parâmetro SourceName como o URL da página da Web que deseja capturar.

Agora, se você fizer logon em sua conta, verá a prova.

## Qual é a diferença entre uma prova e uma versão?

Nas versões da Workfront Proof são exibidas como uma única Prova. Clicar em uma versão específica na interface do usuário da Web exibirá os detalhes dessa versão. Na realidade, cada versão é uma prova separada e a interface do usuário da Web a exibe juntos.

Da perspectiva da API, cada versão é uma prova separada e as provas são vinculadas pelas IDs.

**createProof()** sempre criará **versão 1** da prova. Vamos supor que, para nosso exemplo, a ID retornada para esta prova &quot;100&quot;.

Ao usar **createProofVersion()** sempre envie a ID da versão anterior. Se desejarmos criar **versão 2** na prova &quot;100&quot;, nós **transmitir &quot;100&quot; para o ParentFileID** parâmetro. Isso informa ao sistema que essa prova deve ser da versão 2 do conjunto. O método retornará uma ID de prova exclusiva, por exemplo, digamos que seja &quot;101&quot;.

Se uma terceira versão, ou seja, **versão 3** é obrigatório, você chamará **createProofVersion()** novamente e desta vez **transmitir &quot;101&quot; para o ParentFileID** o que garantirá que a lista vinculada de versões seja criada corretamente.

## Preciso obter uma nova ID de sessão antes de cada chamada?

É importante observar que cada ID de sessão é essencialmente um usuário que executa as ações. 

Você não precisa obter uma nova ID de sessão antes de cada chamada para a API e ela permanecerá válida por 24 horas. O tempo de expiração é redefinido sempre que você faz uma chamada para a API .

## O que é uma prova / URL pessoal?

**Equipe/Público**: Cada versão de prova tem um URL exclusivo da Equipe (Público). Se estiver habilitado, a prova será aberta no modo somente leitura. Você pode obter o URL da equipe usando o [getProofURL()](http://api.proofhq.com/home/proofs/getproofurl) método .

**Pessoal**: Um URL pessoal é exclusivo para cada revisor e versão de prova. Se um conjunto de provas contiver 3 versões e um revisor estiver em todas as versões, o revisor terá 3 URLs pessoais exclusivos. Um URL pessoal abre a versão de prova com o revisor já identificado e, portanto, deve ser mantido seguro e não compartilhado. Os URLs pessoais podem ser obtidos chamando a função [getProofReviewers()](http://api.proofhq.com/home/proofs/getproofreviewers) e iterando em cada  [SOAPRecepientObject](http://api.proofhq.com/home/objects/soaprecipientobject) e obter o parâmetro &quot;proof_url&quot;.

## >Como incluir parâmetros personalizados ao abrir a miniprova?

A prova em miniatura permite incorporar a ferramenta de prova em sua própria página. Um parâmetro &quot;referenciador&quot; pode ser incluído como parte da prova mínima para fornecer um URL de redirecionamento quando um usuário clicar no botão fechar na prova em miniatura. Você pode incluir qualquer número de parâmetros personalizados como parte dessa URL de redirecionamento, anexando-os usando o caractere &#39;&amp;&#39; escape, por exemplo %26.

Por exemplo, o URL de prova em minúsculas
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com&customparam1=somevalue&customparam2=` deve ser codificado como 
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com%26customparam1=somevalue%26customparam2=` para que os parâmetros personalizados sejam transmitidos.

## Como criar um cliente do Java Web Service?

[Este vídeo](http://screencast.com/t/xsSNrqs5b) mostra como você pode criar um cliente do Java Web Service usando o Eclipse e a definição do WSDL da prova da Workfront.
