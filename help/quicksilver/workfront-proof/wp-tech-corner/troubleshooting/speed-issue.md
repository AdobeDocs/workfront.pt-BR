---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Problemas de velocidade no [!DNL Workfront Proof]
description: Esta página de ajuda pode ajudá-lo a determinar se há problemas de velocidade que você esteja enfrentando ao usar o [!DNL Workfront Proof] estão relacionados ao seu ISP ou [!DNL Workfront Proof]rede de entrega de conteúdo do.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 42e999a6-5b27-482d-a7cf-b8030272da32
source-git-commit: 20fcf4dd07c1058559533501f7e297d78c43a70b
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# Problemas de velocidade no [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro do [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

Esta página de ajuda pode ajudá-lo a determinar se há problemas de velocidade que você esteja enfrentando ao usar o [!DNL Workfront Proof] estão relacionados ao seu ISP ou [!DNL Workfront Proof]rede de entrega de conteúdo do.

Problemas de velocidade geralmente ocorrem devido à conexão ISP local ou à configuração de acesso à Internet local (por exemplo, onde um servidor proxy é usado) e, portanto, estão fora do controle do [!DNL Workfront Proof].

Dito isso, há algumas etapas que você pode seguir para verificar a velocidade da conexão, o que permitirá determinar a causa raiz dos problemas que você está enfrentando. Todas essas etapas são igualmente importantes para o processo de solução de problemas, e recomendamos que você reserve um tempo para coletar informações sobre todas as etapas listadas para garantir o diagnóstico mais preciso do problema.

Depois de reunir todos os detalhes, recomendamos consultar o departamento de TI local para identificar problemas locais.

## Estabeleça qual parte do sistema está lenta

Quando você usa [!DNL Workfront Proof], você pode estar trabalhando com o Painel, por exemplo, gerenciando o conteúdo e os usuários da pasta ou com o [!DNL Workfront Proof] Visualizador: realização de uma revisão de prova, verificação dos comentários já feitos e assim por diante.

Determinar qual parte exata do sistema está lenta é o primeiro passo para solucionar problemas de velocidade. Ao relatar [!DNL Workfront Proof] sendo lento, descreva o seguinte:

* Você está enfrentando lentidão em alguma outra página da Web?
* O problema ocorre no painel ou [!DNL Workfront Proof] Visualizador?
* Qual parte exata do sistema é lenta? (por exemplo, processar uma nova prova ou abrir um comentário no [!DNL Workfront Proof] Visualizador)

## Executar testes de ping e traceroute

Quando houver problemas de desempenho, é importante executar o comando traceroute para verificar a conexão. Para fazer isso, abra o Prompt de comando em seu sistema (Terminal no Mac/Linux) e execute as seguintes etapas:

1. Digite um dos seguintes itens e aguarde a conclusão do tracerout:

   * Windows: **tracert app.proofhq.com**
   * Mac/Linux: **traceroute app.proofhq.com**

1. (Somente para Windows) Digite **ping app.proofhq.com**.
1. Quando o ping for concluído, clique com o botão direito do mouse no prompt de comando e selecione tudo.
1. Copie e cole os resultados na resposta ao seu email.
Certifique-se de permitir a conclusão do traceroute e do ping antes de enviar os resultados para a Equipe de suporte.

## Testar a velocidade da conexão usando Speedtest.net

1. Abra um navegador e acesse Speedtest.net.
1. Siga as instruções na base de conhecimento Speedtest (Teste rápido) para testar a velocidade de sua conexão com a Internet.
1. Copie e cole os resultados em um e-mail para nossa Equipe de suporte.

## Verifique a guia de rede no console do navegador

O console da Web disponível nos navegadores modernos reúne informações úteis sobre qualquer latência de rede, o que será útil para determinar a causa raiz dos problemas de velocidade que você está enfrentando.

Para verificar os tempos de carregamento de uma página da Web:

1. Abra o console do navegador e a guia Rede.
1. Recarregue a página.
1. Faça capturas de tela ou grave uma captura de tela dos resultados.
1. Compartilhe os resultados com a Equipe de suporte.

Certifique-se de que a captura de tela mostre todos os dados. Você pode expandir a janela do console ao fazer uma captura de tela ou rolar para baixo em uma captura de tela.

Você também pode verificar a documentação do navegador para obter instruções mais detalhadas.

## Verifique sua conexão em uma rede e computador diferentes

Verificar se você enfrenta o mesmo problema com a velocidade da conexão usando um dispositivo ou rede diferente é uma etapa crucial no processo de solução de problemas. Tente alternar para outro computador ou dispositivo móvel, bem como tente usar uma rede alternativa (por exemplo, dados móveis).

Comparar a conexão em combinações diferentes: usando uma máquina diferente na mesma rede, usando a mesma máquina em uma rede diferente e usando uma máquina e uma rede alternativas. Em seguida, compartilhe os resultados com a Equipe de suporte.
