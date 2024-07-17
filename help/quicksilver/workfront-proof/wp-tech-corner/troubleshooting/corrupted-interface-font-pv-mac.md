---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Solução de problemas - fonte de interface corrompida no visualizador de provas no Mac
description: Solução de problemas de fonte de interface corrompida no revisor de provas no Mac
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1e96720a-b967-4447-bd14-26fc6a502b25
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# Solução de problemas - fonte de interface corrompida no visualizador de provas no Mac

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

Se você observar que o revisor de provas não exibe a fonte da interface corretamente, isso pode ocorrer devido a alguns problemas com as fontes no computador Mac. Para resolver o problema, tente as seguintes soluções:

## Remover duplicatas de fontes

Verifique se há fontes duplicadas no sistema.

1. Feche o navegador que você está usando.
1. Abra o aplicativo Font Book na pasta Aplicativos.
1. Clique em **[!UICONTROL Todas as fontes]** (1).
1. Clique em **[!UICONTROL Editar]** > **[!UICONTROL Procurar Duplicatas Habilitadas]**.

1. Clique em **[!UICONTROL Sim]** para resolver duplicatas.
1. Se você vir um aviso sobre fontes corrompidas, clique em **[!UICONTROL Sim]**.
1. Reinicie o computador.
1. Tente a prova novamente.

## Limpar o cache de fontes

Às vezes, os caches de fonte no Mac OS X ficam corrompidos. Por exemplo, quando uma fonte ou uma família de fontes é reinstalada várias vezes ou se um aplicativo foi atualizado ou reinstalado. Além dos arquivos de cache de fontes do sistema operacional, alguns aplicativos podem ter seu próprio cache de fontes. A exclusão desses arquivos de cache de fontes pode resolver o problema de texto distorcido.

Em primeiro lugar, você terá que iniciar o Font Book, selecionar a fonte ou família que você está tendo problemas com e pressionar o botão Excluir no seu teclado. Você também pode clicar com o botão direito do mouse e selecionar [!UICONTROL Remover Família]. Se não tiver certeza de qual fonte ou família está causando os problemas, tente primeiro remover as duplicatas, conforme descrito acima.

A segunda etapa seria limpar o cache de fontes e há várias maneiras de fazer isso.

A primeira é simplesmente reinicializar no Modo de segurança, mantendo a tecla Shift pressionada imediatamente quando você ouvir os sinalizadores de inicialização na inicialização. Quando esse modo é carregado, uma barra de progresso deve aparecer, durante a qual o sistema executará várias verificações e rotinas de manutenção, uma das quais é limpar o cache de fontes.

A segunda abordagem é usar o Terminal, que pode ser feito executando o seguinte comando de uma conta administrativa: *sudo atsutil databases -remove*

>[!NOTE]
>
>Este comando exigirá que você digite sua senha, que não será mostrada ao digitar. Recomendamos consultar seu departamento de TI, pois isso pode exigir permissões de administrador no computador.

Outra abordagem seria usar um utilitário de cache de fontes, como o FontNuke, e limpar o cache com sua ajuda.

Muitos estúdios de prova de prelo e arte/design também usam o software Universal Type Server para gerenciar o licenciamento e a distribuição de fontes. Às vezes, pode ocorrer um problema com o Cache de Fontes do Universal Type Server, o que pode fazer com que as anotações [!DNL Workfront Proof] desapareçam.

Para corrigir, limpe o Universal Type Server Font Cache e reinicie o Universal Type Server.

## Corrigir conflito de fonte [!DNL Flash]

Talvez você não tenha acesso a essa funcionalidade porque ela tem suporte no [!DNL Flash], que foi descontinuado na maioria dos ambientes.

O visualizador de provas herdado é baseado em [!DNL Flash Player] e, às vezes, quando o texto está ausente no visualizador de provas, é possível que haja um conflito de fontes entre o OS X e [!DNL Flash Player]. Tente o seguinte:

1. Abra o Localizador e abra a guia **[!UICONTROL Ir]**.
1. Pressione a tecla Option (⌥ Alt) para abrir a pasta [!UICONTROL Biblioteca] na lista suspensa.
1. Ao manter pressionada a tecla Option, clique na pasta [!UICONTROL Biblioteca].
1. Depois que a pasta [!UICONTROL Biblioteca] for aberta, vá para a pasta [!UICONTROL Fontes] localizada em.
1. Mova todas as fontes localizadas na pasta [!UICONTROL Fontes] para outra pasta, talvez na sua área de trabalho (não crie outra pasta dentro da pasta Fontes).
1. Esta ação oculta todas as suas fontes personalizadas; você ainda deve ter as fontes padrão do sistema salvas em seus locais separados.
1. Sair e reiniciar [!DNL Safari].
1. Reabra a prova.

Você deve ver suas fontes agora. Se você não precisa de nenhuma das fontes que você removeu de seu diretório inicial, você pode excluí-las com segurança. Caso contrário, verifique-as em lotes, copie-as de volta para a pasta Biblioteca/Fontes e veja qual delas está causando o problema.
