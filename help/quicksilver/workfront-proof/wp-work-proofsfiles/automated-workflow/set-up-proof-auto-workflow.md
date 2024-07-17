---
product-previous: workfront-proof
product-area: documents
navigation-topic: automated-workflow-workfront-proof
title: Configurar uma prova com um Fluxo de Trabalho Automatizado no  [!DNL Workfront Proof]
description: Isso repete as informações encontradas em Configuração de provas no Workfront. Consolide aqui ou ali. Talvez melhor aqui.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 605569df-8e63-476d-a0cd-e73802042011
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1637'
ht-degree: 0%

---

# Configurar uma prova com um Fluxo de Trabalho Automatizado no [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

O fluxo de trabalho automatizado facilita o gerenciamento da revisão e aprovação de conteúdo quando você tem processos de revisão complexos ou envia conteúdo para revisão para os mesmos grupos de pessoas regularmente.

Você cria a prova e, em seguida, ela se move de estágio para estágio até a aprovação final. Os usuários relevantes são notificados sempre que precisam fazer uma aprovação.

![diagrama_de_estágios.png](assets/stages-diagram-350x81.png)

Você pode adicionar um fluxo de trabalho automatizado a uma prova ao carregar o documento ou depois que o documento for carregado.

## Criar uma prova com o fluxo de trabalho automatizado

1. Comece a criar a prova.
1. Na seção **[!UICONTROL Compartilhar]**, clique em **[!UICONTROL Usar Fluxo de Trabalho Automatizado]**.

   É possível desmarcar essa opção para alternar de volta para um workflow padrão.

1. (Opcional) Se quiser usar um modelo de Fluxo de Trabalho Automatizado que o administrador do [!DNL Workfront] configurou e compartilhou com você, selecione-o no menu suspenso **[!UICONTROL Selecionar um modelo de Fluxo de Trabalho]**.

   >[!NOTE]
   >
   >Sua capacidade de modificar o modelo depende das configurações do modelo definidas pelo administrador [!DNL Workfront]. Se a capacidade de modificar o modelo estiver desativada, somente o proprietário do modelo poderá modificá-lo.

1. Especifique as seguintes informações para configurar o primeiro estágio do fluxo de trabalho automatizado:

   * **[!UICONTROL Nome]:** O nome do estágio aparece no diagrama de Fluxo de Trabalho e está incluído nas notificações de email enviadas aos revisores.
   * **[!UICONTROL Prazo]:** A funcionalidade deste campo difere dependendo da opção selecionada na lista suspensa **[!UICONTROL Prazo calculado a partir de]**.

   * **[!UICONTROL Da criação da prova]:** selecione a data limite para a prova.
   * **[!UICONTROL Da ativação do estágio]:** Selecione o número de dias úteis que serão adicionados à data de ativação do estágio para definir automaticamente um prazo na prova.
   * **[!UICONTROL Ativar estágio]:** Para cada estágio do fluxo de trabalho, você pode decidir quando ele deve ser ativado. Para o primeiro estágio, as seguintes opções estão disponíveis.

      * Na criação da prova
      * Em uma hora e data específicas
      * Manualmente\

        Opções adicionais estão disponíveis para estágios subsequentes. Essas opções exigem um estágio principal. São eles:
      * Depois que o prazo final anterior é atingido
      * Todas as decisões são aprovadas ou aprovadas com alterações
      * Todas as decisões são aprovadas
      * Todas as decisões são tomadas
   * **[!UICONTROL Prazo calculado de]:** A opção selecionada nesta lista suspensa afeta as opções disponíveis no campo **[!UICONTROL Prazo]**.

   * **[!UICONTROL Criação da prova]:** No campo **[!UICONTROL Prazo]**, selecione a data do prazo final para a prova.

   * **[!UICONTROL Ativação de preparo]:** No campo **[!UICONTROL Prazo]**, selecione o número de dias úteis que serão adicionados à data de ativação do preparo para definir automaticamente um prazo na prova.

   * **[!UICONTROL Estágio de bloqueio]:** Selecione quando o estágio pode ser bloqueado.
   * **[!UICONTROL Tomador de decisão principal]:** Selecione o tomador de decisão principal no estágio. Os tomadores de decisão estão disponíveis na lista suspensa somente após adicionar revisores ao estágio.
   * **[!UICONTROL Somente uma decisão necessária]:** Selecione esta opção para que a revisão seja concluída depois que um dos tomadores de decisão tomar sua decisão.\

     Esta opção não estará disponível se você tiver designado um usuário no menu suspenso **[!UICONTROL Tomador de decisão principal]**.

   * **[!UICONTROL Estágio privado]:** Quando esta opção está selecionada, comentários e decisões não ficam visíveis para pessoas que não foram adicionadas a este estágio ou não são Supervisores, Administradores ou Administradores de Cobrança na conta


1. (Opcional) Adicione revisores ao estágio.
1. Considere o seguinte ao adicionar revisores:

   * Um revisor pode ser adicionado a uma prova apenas uma vez. (Não é possível adicionar a mesma pessoa a mais de um estágio na prova.)
   * Os revisores adicionados a um estágio privado poderão ver somente o estágio ao qual foram adicionados na prova e nos comentários feitos nesse estágio.
   * Por padrão, adicionar um usuário a um estágio concede a ele acesso para visualizar a prova a partir do momento em que a prova é criada.\

     O administrador do sistema pode configurar o sistema de prova para impedir que os usuários acessem a prova até que o fluxo de trabalho entre no estágio em que o usuário foi adicionado. Para obter mais informações, consulte

1. (Opcional) Clique em **[!UICONTROL Novo estágio]** e repita as Etapas 4 e 5 para adicionar vários estágios ao fluxo de trabalho automatizado.
1. Continue criando a prova especificando as informações necessárias nas seções [!UICONTROL Organizar] e [!UICONTROL Mais configurações] na página [!UICONTROL Nova Prova], conforme descrito em

## Diagramas de fluxo de trabalho automatizados

Ao configurar o fluxo de trabalho para sua prova, você observará um diagrama sendo criado. Cada estágio adicionado à prova será exibido no diagrama, indicando claramente as dependências entre os estágios. Os estágios privados são marcados com um ícone de chave.

O diagrama flutua, o que significa que ele permanecerá visível mesmo se você rolar a página para baixo.

Se não precisar ver o diagrama, você pode ocultá-lo (1).

![Diagrama.png](assets/diagram-350x93.png)

## Adicionar um estágio

É possível adicionar outro estágio a um workflow que está criando ou modificando.

1. Se você estiver adicionando um estágio a uma prova existente, vá para a página Detalhes da prova, conforme descrito em [Gerenciar detalhes da prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Na seção **[!UICONTROL Fluxo de trabalho]**, clique em **[!UICONTROL Novo estágio]**.

1. Especifique informações para o estágio como na etapa 4 na seção [!UICONTROL Criação de uma prova com um fluxo de trabalho automatizado] neste artigo.
1. Clique em **[!UICONTROL Adicionar estágio]** e em **[!UICONTROL Concluído]**.

## Excluir um estágio

1. Clique no ícone de lixeira disponível no canto superior direito do estágio (1).\
   O ícone é exibido quando você passa o mouse sobre o palco.\
   ![excluindo_um_estágio.png](assets/deleting-a-stage-350x250.png)

## Configurações de preparo

* **[!UICONTROL Nome do estágio]**: aparece no diagrama de Fluxo de Trabalho e está incluído nas notificações por email enviadas aos revisores.
* **[!UICONTROL Ativar estágio]**: para cada estágio do fluxo de trabalho, você pode decidir quando ele deve ser ativado. Para o primeiro estágio, as seguintes opções estarão disponíveis:

   * Na criação da prova
   * Em uma hora e data específicas
   * Manual
   * Somente essas três opções estão disponíveis para o primeiro estágio. As outras opções ficarão disponíveis quando você adicionar um segundo estágio; elas exigem que você selecione um estágio principal.
   * Depois que o prazo final anterior é atingido (requer a escolha de um estágio principal)
   * Todas as decisões são Aprovadas ou [!UICONTROL Aprovadas com alterações] (é necessário escolher um estágio principal)
   * Todas as decisões são Aprovadas (requer a escolha de um estágio principal)
   * Todas as decisões são tomadas (requer a escolha de um estágio principal)

* **[!UICONTROL Prazo]:** Você pode decidir como o prazo deve ser calculado em cada estágio de um fluxo de trabalho. As opções são:

   * Na criação da prova: no campo [!UICONTROL deadline] (9), é possível selecionar a data do prazo para a prova.
   * Na lista suspensa [!UICONTROL prazo]: selecione o número de dias úteis que serão adicionados à data de ativação do estágio para definir automaticamente um prazo na prova.

* **[!UICONTROL Bloqueio]:** Há várias opções que determinam quando um estágio pode ser bloqueado. As opções incluem:

   * Bloqueio manual
   * Nunca
   * Quando o próximo estágio começar
   * Quando todas as decisões são tomadas

**[!UICONTROL Tomador de decisão principal]**: você define o tomador de decisão principal no estágio. Os tomadores de decisão disponíveis aparecem na lista somente após adicionar os revisores ao estágio.

>[!NOTE]
>
>Se você escolher um Tomador de decisão Principal, apenas uma opção de decisão necessária não estará mais disponível nesse estágio.

* **[!UICONTROL É necessária somente uma decisão]**: você pode habilitar esta opção em um estágio. Isto significa que a revisão será concluída assim que um dos tomadores de decisão tomar a sua decisão.
* **[!UICONTROL Privacidade]:** Cada estágio pode ser privado. Se um estágio for privado, os comentários e as decisões não estarão visíveis para as pessoas que não foram adicionadas a esse estágio ou que não são Supervisores, Administradores ou Administradores de Faturamento na conta. Para obter mais informações, consulte [Visão geral do Fluxo de Trabalho Automatizado](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Adicionar revisores a um estágio

1. Insira um nome de contato ou endereço de email no campo na parte inferior de cada estágio.
1. Clique no ícone de adição verde para adicioná-los.
1. Defina a função na prova.
1. Definir o alerta de email.
1. Ao configurar o primeiro estágio, você também tem a opção de alterar o Proprietário da prova.

   >[!NOTE]
   >
   >* Um revisor pode ser adicionado a uma prova apenas uma vez. Não é possível adicionar a mesma pessoa a mais de um estágio na prova.
   >* Os revisores que não são adicionados a um estágio privado não podem ver o estágio na prova ou nos comentários feitos nesse estágio.


## Converter uma prova em um fluxo de trabalho automatizado

Você pode converter uma prova básica em um Fluxo de trabalho automatizado.

1. Clique em **[!UICONTROL Converter em Fluxo de Trabalho Automatizado]** na página [!UICONTROL Detalhes da prova].
Depois que a prova é retrabalhada para o Fluxo de Trabalho Automatizado, todos os estágios são ativos, públicos e sua opção [!UICONTROL Bloquear estágio] é definida como Manual por padrão. Todos os estágios permanecem com os usuários e suas configurações.

   * Ativar estágio está definido como Na criação de prova em cada estágio.
   * O prazo calculado a partir da opção é definido para a Criação de prova em cada estágio.
   * Se apenas uma opção de decisão foi selecionada na prova básica, todas as etapas a terão selecionada.
   * Se um [!UICONTROL Tomador de decisão principal] da prova básica tiver sido selecionado, os estágios com esse destinatário serão definidos como eles e todos os outros terão o valor definido como Nenhum.
   * O nome do estágio permanece o mesmo.

## Adicionar um modelo adicional a um Fluxo de trabalho automatizado existente

Depois que uma prova básica é convertida em Fluxo de trabalho automatizado, é possível adicionar outro modelo a ela.

1. Na página Detalhes da prova, na seção Fluxo de trabalho, clique em **[!UICONTROL Adicionar modelo].**

   * As configurações do modelo determinam o que pode ser feito com uma prova à qual esse modelo foi adicionado. Por exemplo, se o modelo tiver as opções [!UICONTROL Adicionar um estágio e Adicionar pessoas a estágios] desabilitadas, os botões para [!UICONTROL adicionar estágio] e [!UICONTROL compartilhar prova] não estarão visíveis.
   * Se a opção [!UICONTROL Adicionar um estágio] estiver desabilitada no modelo fornecido, o botão [!UICONTROL Adicionar modelo] não ficará visível após adicioná-la.
   * Quando uma pessoa é adicionada a um estágio em um modelo de Fluxo de trabalho automatizado, mas também já está presente na prova, se esse modelo for aplicado, o sistema removerá automaticamente essa pessoa do estágio. Se não houver mais ninguém adicionado a esse estágio específico, o erro a seguir será exibido, pois o sistema não permitirá a adição de um estágio vazio ao workflow.

     ![erro_ao_adicionar_modelo.png](assets/error-when-adding-template-350x66.png)
