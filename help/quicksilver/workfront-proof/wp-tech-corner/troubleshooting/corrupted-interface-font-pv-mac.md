---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Solução de problemas - fonte de interface corrompida no visualizador de prova no Mac
description: Se você observar que o visualizador de prova não exibe a fonte da interface corretamente, isso pode ser devido a alguns problemas com as fontes na sua máquina Mac. Para resolver o problema, tente as seguintes soluções - EDITE-ME.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1e96720a-b967-4447-bd14-26fc6a502b25
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# Solução de problemas - fonte de interface corrompida no visualizador de prova no Mac

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

Se você observar que o visualizador de prova não exibe a fonte da interface corretamente, isso pode ser devido a alguns problemas com as fontes na sua máquina Mac. Para resolver o problema, tente as seguintes soluções:

## Remover duplicatas de fontes

Verifique se há fontes duplicadas no sistema.

1. Feche o navegador que você está usando.
1. Abra o aplicativo Font Book na pasta Aplicativos.
1. Clique em **[!UICONTROL Todas as fontes]** (1)
1. Clique em **[!UICONTROL Editar]** > **[!UICONTROL Procurar duplicatas ativadas]**.

1. Clique em **[!UICONTROL Sim]** para resolver duplicatas.
1. Se você vir um aviso sobre fontes corrompidas, clique em **[!UICONTROL Sim]**.
1. Reinicie o computador.
1. Tente novamente a prova.

## Limpar o cache de fontes

Às vezes, os caches de fonte no Mac OS X ficam corrompidos. Por exemplo, quando uma fonte ou família de fontes é reinstalada várias vezes ou se um aplicativo foi atualizado ou reinstalado. Além dos arquivos de cache de fontes do sistema operacional, alguns aplicativos podem ter seu próprio cache de fontes. A exclusão desses arquivos de cache de fonte pode resolver o problema com texto distorcido.

Primeiro, você precisará iniciar o Font Book, selecionar a fonte ou a família com a qual você está tendo problemas e pressionar o botão Delete no teclado. Além disso, é possível clicar com o botão direito do mouse e selecionar [!UICONTROL Remover Família]. Se não tiver certeza de qual fonte ou família está causando os problemas, tente remover as duplicatas, conforme descrito acima.

A segunda etapa seria limpar o cache de fontes e há várias maneiras de fazer isso.

O primeiro é simplesmente reinicializar no modo de segurança, mantendo a tecla Shift pressionada imediatamente quando ouvir os chimes de inicialização na inicialização. Quando esse modo é carregado, uma barra de progresso deve aparecer, durante a qual o sistema executará várias verificações e rotinas de manutenção, uma das quais é limpar o cache de fontes.

A segunda abordagem é usar o Terminal, o que pode ser feito executando o seguinte comando de uma conta administrativa: *bancos de dados sudo atsutil -remove*

>[!NOTE]
>
>Este comando exigirá que você digite sua senha, que não será mostrada quando digitada. Recomendamos consultar seu departamento de TI, pois isso pode exigir permissões de Administrador em sua máquina.

Outra abordagem seria usar um utilitário de cache de fontes, como FontNuke, e limpar o cache com sua ajuda.

Muitos estúdios de prelo e arte-final/design também usam o software Universal Type Server para gerenciar o licenciamento e a distribuição de fontes. Às vezes, pode ocorrer um problema com o Universal Type Server Font Cache, que pode causar o erro [!DNL Workfront Proof] anotações para desaparecer.

Para corrigir, limpe o Universal Type Server Font Cache e reinicie o Universal Type Server.

## Correção [!DNL Flash] conflito de fontes

Talvez você não tenha acesso a essa funcionalidade porque ela é compatível com o [!DNL Flash], que foi descontinuada na maioria dos ambientes.

O visualizador de prova de legado é baseado em [!DNL Flash Player] e, às vezes, quando o texto está ausente no visualizador de prova, é possível que haja um conflito de fonte entre o OS X e o [!DNL Flash Player]. Tente o seguinte:

1. Abra o Localizador e abra o **[!UICONTROL Ir]** guia .
1. Pressione a tecla Option (⌥ Alt) para abrir o [!UICONTROL Biblioteca] na lista suspensa.
1. Ao manter a tecla Option pressionada, clique no botão [!UICONTROL Biblioteca] pasta.
1. Depois que a variável [!UICONTROL Biblioteca] abre, vá para [!UICONTROL Fontes] localizada em .
1. Mova todas as fontes localizadas na [!UICONTROL Fontes] pasta em outra pasta, talvez na área de trabalho (não crie outra pasta dentro da pasta Fonts ).
1. Essa ação oculta todas as fontes personalizadas; você ainda deve ter as fontes padrão do sistema salvas em seu local separado.
1. Sair e reiniciar [!DNL Safari].
1. Reabra a prova.

Você deve ver suas fontes agora. Se não precisar de nenhuma das fontes removidas do diretório inicial, você poderá excluí-las com segurança. Caso contrário, percorra-os em lotes, copie-os de volta para a pasta Biblioteca/Fontes e veja qual deles está causando o problema.
