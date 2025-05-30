---
title: Perguntas frequentes sobre a API do SOAP
description: Perguntas frequentes sobre a API do SOAP
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: fcf89bd6-0e07-42a7-9ae3-9a1309e51946
source-git-commit: 79b6370ec3283922a16435e8eb8069f7f9560c55
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Perguntas frequentes sobre a API do SOAP

## Como crio minha primeira prova de arquivo?

São necessárias 3 etapas simples:

**Etapa 1**: carregue o arquivo para o Workfront Proof enviando-o por meio de uma solicitação Post para  [https://soap.proofhq.com/upload.php](https://soap.proofhq.com/upload.php). Retornaremos o hash do arquivo - isso é muito importante! Observe que, neste momento, você não verá nada em sua conta. Tudo o que você fez até agora foi nos enviar o arquivo, mas não nos disse o que fazer com ele.

**Etapa 2**: se você ainda não tiver uma ID de Sessão, obtenha-a usando os métodos doLogin() ou getSessionID(). Use o primeiro para &quot;fazer logon&quot; usando o endereço de email e a senha de um usuário ou o último método se você tiver o endereço de email e o token de autenticação do usuário.

**Etapa 3:** Agora é hora de criar sua prova. Use o método createProof() e envie pelo menos os campos obrigatórios (atualmente, há apenas 5 deles). Defina o parâmetro Hash para o hash de arquivo retornado durante a &quot;Etapa 1&quot;, pois isso permite determinar qual arquivo usar ao criar sua prova.

Se agora você fizer logon na sua conta, verá a prova.

## Como criar minha primeira prova de instantâneo da Web?

São necessárias 2 etapas simples:

**Etapa 1**: se você ainda não tiver uma ID de Sessão, obtenha-a usando os métodos doLogin() ou getSessionID(). Use o primeiro para &quot;fazer logon&quot; usando o endereço de email e a senha de um usuário ou o último método se você tiver o endereço de email e o token de autenticação do usuário.

**Etapa 2:**&#x200B;agora é hora de criar sua prova. Use o método createProof() e envie pelo menos os campos obrigatórios (atualmente, há apenas 5 deles). Defina o parâmetro Hash como &quot;web&quot; e o parâmetro SourceName como o URL da página da Web que você deseja capturar.

Se agora você fizer logon na sua conta, verá a prova.

## Qual é a diferença entre uma prova e uma versão?

Nas versões do Workfront Proof, são exibidas como uma única Prova. Clicar em uma versão específica na interface da Web exibirá os detalhes dessa versão. Na realidade, cada versão é uma prova separada e a interface do usuário da Web as exibe juntas.

Da perspectiva da API, cada versão é uma prova separada e as provas são vinculadas por suas IDs.

**createProof()** sempre criará a **versão 1** da prova. Vamos supor que, para o nosso exemplo, a ID retornada para esta prova &quot;100&quot;.

Ao usar **createProofVersion()** sempre envie a ID da versão anterior. Se queremos criar a **versão 2** na prova &quot;100&quot;, nós **passamos &quot;100&quot; para o parâmetro ParentFileID**. Isso informa ao sistema que essa prova deve ser a versão 2 do conjunto. O método retornará uma ID de prova exclusiva, por exemplo, digamos que seja &quot;101&quot;.

Se uma terceira versão, ou seja, **versão 3**, for necessária, você chamará **createProofVersion()** novamente e, desta vez, **passará em &quot;101&quot; para ParentFileID**, o que garantirá que a lista de versões vinculada seja criada corretamente.

## Preciso obter uma nova ID de sessão antes de cada chamada?

É importante destacar que cada ID de sessão é essencialmente um usuário que executa as ações. 

Não é necessário obter uma nova ID de sessão antes de cada chamada para a API, que permanecerá válida por 24 horas. O tempo de expiração é redefinido sempre que você faz uma chamada para a API.

## O que é uma prova/URL pessoal?

**Equipe/Público**: cada versão de prova tem uma URL de Equipe (Pública) exclusiva. Se ativado, abrirá a prova no modo somente leitura. Você pode obter a URL da Equipe usando o método [getProofURL()](https://api.proofhq.com/home/proofs/getproofurl.html).

**Pessoal**: uma URL pessoal é exclusiva para cada revisor e versão de prova. Se um conjunto de prova tiver 3 versões e um revisor estiver em todas as versões, o revisor terá 3 URLs pessoais exclusivos. Um URL pessoal abre a versão de prova com o revisor já identificado e, portanto, deve ser mantido seguro e não compartilhado. É possível obter URLs pessoais chamando o método [getProofReviewed()](https://api.proofhq.com/home/proofs/getproofreviewers.html) e iterando em cada  [SOAPRecepientObject](https://api.proofhq.com/home/objects/soaprecipientobject.html) e obtendo o parâmetro &quot;proof_url&quot;.

## >Como incluir parâmetros personalizados ao abrir a miniprova?

A miniprova permite incorporar a ferramenta de prova na sua própria página. Um parâmetro &quot;referenciador&quot; pode ser incluído como parte da miniprova para fornecer um URL de redirecionamento quando um usuário clicar no botão Fechar na miniprova. Você pode incluir qualquer número de parâmetros personalizados como parte dessa URL de redirecionamento, anexando-os usando o caractere de escape &#39;&amp;&#39;, por exemplo, %26.

Por exemplo, o URL de miniprova
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com&customparam1=somevalue&customparam2=` deve ser codificado como 
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com%26customparam1=somevalue%26customparam2=` para que os parâmetros personalizados sejam transmitidos.


