---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Problemas de velocidade em [!DNL Workfront Proof]
description: Esta página de ajuda pode ajudar a determinar se há algum problema de velocidade que você esteja enfrentando ao usar [!DNL Workfront Proof] estão relacionadas ao seu ISP ou [!DNL Workfront Proof]Rede de entrega de conteúdo da .
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 42e999a6-5b27-482d-a7cf-b8030272da32
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 0%

---

# Problemas de velocidade em [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

Esta página de ajuda pode ajudar a determinar se há algum problema de velocidade que você esteja enfrentando ao usar [!DNL Workfront Proof] estão relacionadas ao seu ISP ou [!DNL Workfront Proof]Rede de entrega de conteúdo da .

Problemas de velocidade geralmente são causados pela conexão ISP local ou pela configuração de acesso à Internet local (por exemplo, onde um servidor proxy é usado) e, portanto, infelizmente, estão fora do controle de [!DNL Workfront Proof].

Dito isso, há algumas etapas que você pode tomar para verificar a velocidade da conexão, o que permitirá que a causa raiz dos problemas que você está enfrentando seja determinada. Todas essas etapas são igualmente importantes para o processo de solução de problemas e recomendamos que você se dedique ao tempo para coletar informações sobre todas as etapas listadas para garantir o diagnóstico mais preciso do problema.

Depois de coletar todos os detalhes, recomendamos que você consulte o departamento de TI local para identificar problemas locais. Se precisar de mais ajuda, entre em contato com nossa [Equipe de suporte](https://support.workfront.com/hc/en-us/requests/new).

## Determine qual parte do sistema está lenta

Ao utilizar [!DNL Workfront Proof], você pode estar trabalhando com o Painel , por exemplo, gerenciando o conteúdo da pasta e os usuários ou com o [!DNL Workfront Proof] Visualizador: Proceder a uma revisão das provas, verificar as observações já feitas e assim por diante.

Determinar qual parte exata do sistema está lenta é o primeiro passo para solucionar problemas de velocidade. Ao relatar [!DNL Workfront Proof] sendo lento, descreva o seguinte:

* Você está passando por lentidão em alguma outra página da Web?
* O problema ocorre no Painel ou [!DNL Workfront Proof] Visualizador?
* Qual é exatamente a parte lenta do sistema? (por exemplo, processar uma nova prova ou abrir um comentário em [!DNL Workfront Proof] Visualizador)

## Executar testes de trackeroute e ping

Quando estiver com problemas de desempenho, é importante executar o comando traceroute para verificar a conexão. Para fazer isso, abra o Prompt de comando no sistema (Terminal no Mac/Linux) e execute as seguintes etapas:

1. Digite um dos seguintes itens e aguarde até que o rastreamento seja concluído:

   * Windows: **tracert app.proofhq.com**
   * Mac/Linux: **traceroute app.proofhq.com**

1. (Somente Windows) Tipo **ping app.proofhq.com**.
1. Quando o ping for concluído, clique com o botão direito do mouse no prompt de comando e selecione tudo.
1. Copie e cole os resultados na resposta do seu email.
Certifique-se de permitir que o traceroute e o ping sejam concluídos antes de enviar os resultados para a Equipe de suporte.

## Testar a velocidade de conexão usando Speedtest.net

1. Clique em [here](http://www.speedtest.net/) para acessar Speedtest.net.
1. Siga as instruções na base de conhecimento Speedtest para testar a velocidade da sua conexão com a Internet.
1. Copie e cole os resultados em um e-mail para nossa equipe de suporte.

## Verifique a guia Rede no console do navegador

O console da Web disponível nos navegadores modernos reúne informações úteis sobre qualquer latência de rede, o que nos ajudará a determinar a causa raiz dos problemas de velocidade que você está enfrentando.

Para verificar os tempos de carregamento de uma página da Web:

1. Abra o console do navegador e a guia Rede.
1. Recarregue a página.
1. Tire capturas de tela ou registre uma projeção de tela dos resultados.
1. Compartilhe os resultados com a equipe de suporte.

Certifique-se de que a captura de tela mostra todos os dados. Você pode expandir a janela do console ao capturar a tela ou rolar para baixo em uma transmissão de tela.

Se não souber como abrir o console no navegador, consulte estas etapas gravadas:

* [Cromo](http://screencast.com/t/AgQU6JQQ)
* [Safari](http://screencast.com/t/f31GqQYm0w)
* [Firefox](http://screencast.com/t/Xg7SscmAi)
* [Edge](http://www.screencast.com/t/epSwBiaD)
* [Internet Explorer](http://screencast.com/t/x5Q3eHczbc)

Você também pode verificar a documentação do navegador para obter instruções mais detalhadas.

## Verifique a conexão em outra rede e máquina

Verificar se você tem o mesmo problema com a velocidade da conexão usando um dispositivo ou rede diferente é uma etapa crucial no processo de solução de problemas. Tente mudar para uma máquina diferente ou um dispositivo móvel, bem como tentar utilizar uma rede alternativa (por exemplo, dados móveis).

Compare a conexão em combinações diferentes: usando uma máquina diferente na mesma rede, usando a mesma máquina em uma rede diferente e usando a máquina e a rede alternativas, em seguida, compartilhe os resultados com a equipe de suporte.
