---
product-previous: workfront-proof
product-area: documents
navigation-topic: automated-workflow-workfront-proof
title: Configure uma prova com um Fluxo de trabalho automatizado no [!DNL Workfront Proof]
description: Isso repete as informações encontradas em Configuração de provas no Workfront. Consolide aqui ou ali. Talvez melhor aqui.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 605569df-8e63-476d-a0cd-e73802042011
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1637'
ht-degree: 0%

---

# Configure uma prova com um Fluxo de trabalho automatizado no [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

O fluxo de trabalho automatizado facilita o gerenciamento da revisão e aprovação de conteúdo quando você tem processos de revisão complexos ou envia conteúdo para análise aos mesmos grupos de pessoas regularmente.

Você cria a prova e então ela se move de estágio para estágio até aprovação final. Os usuários relevantes são notificados sempre que forem solicitados a fazer uma aprovação.

![stage_diagrama.png](assets/stages-diagram-350x81.png)

Você pode adicionar um fluxo de trabalho automatizado a uma prova ao fazer upload do documento ou após o upload do documento.

## Criar uma prova com o Fluxo de trabalho automatizado

1. Comece a criar a prova.
1. No **[!UICONTROL Compartilhar]** seção , clique em **[!UICONTROL Usar fluxo de trabalho automatizado]**.

   É possível desmarcar essa opção para voltar para um fluxo de trabalho padrão.

1. (Opcional) Se você quiser usar um modelo de Fluxo de trabalho automatizado que [!DNL Workfront] administrador configurado e compartilhado com você, selecione-o no **[!UICONTROL Selecionar um modelo de Fluxo de trabalho]** menu suspenso.

   >[!NOTE]
   >
   >Sua capacidade de modificar o modelo depende das configurações do modelo definidas pelo [!DNL Workfront] administrador. Se a capacidade de modificar o modelo estiver desativada, somente o proprietário do modelo poderá modificá-lo.

1. Especifique as seguintes informações para configurar o primeiro estágio do Fluxo de trabalho automatizado:

   * **[!UICONTROL Nome]:** O nome do palco aparece no diagrama de Fluxo de trabalho e é incluído nas notificações por email enviadas aos revisores.
   * **[!UICONTROL Prazo]:** A funcionalidade desse campo varia dependendo da opção selecionada na variável **[!UICONTROL Prazo calculado a partir de]** lista suspensa.

   * **[!UICONTROL Da criação de prova]:** Selecione a data final para a prova.
   * **[!UICONTROL A partir da ativação de estágio]:** Selecione o número de dias úteis que serão adicionados à data de ativação do estágio para definir automaticamente um prazo na prova.
   * **[!UICONTROL Ativar estágio]:** Para cada estágio do fluxo de trabalho, você pode decidir quando ele deve ser ativado. Para o seu primeiro estágio, as opções a seguir estão disponíveis.

      * Na criação da prova
      * Em uma data e hora específicas
      * Manualmente\

         Opções adicionais estão disponíveis para estágios subsequentes. Essas opções exigem um estágio principal. Eles são:
      * Depois de atingido o prazo anterior
      * Todas as decisões são Aprovadas ou Aprovadas com alterações
      * Todas as decisões são aprovadas
      * Todas as decisões são tomadas
   * **[!UICONTROL Prazo calculado a partir de]:** A opção selecionada nessa lista suspensa afeta as opções disponíveis na variável **[!UICONTROL Prazo]** campo.

   * **[!UICONTROL Criação de prova]:** No **[!UICONTROL Prazo]** selecione a data final para a prova.

   * **[!UICONTROL Ativação de estágio]:** No **[!UICONTROL Prazo]** , selecione o número de dias úteis que serão adicionados à data de ativação do estágio para definir automaticamente um prazo na prova.

   * **[!UICONTROL Bloquear palco]:** Selecione quando o palco pode ser bloqueado.
   * **[!UICONTROL Tomador de decisão principal]:** Selecione o principal decisor no palco. Os tomadores de decisão estão disponíveis na lista suspensa somente depois que você adiciona revisores ao palco.
   * **[!UICONTROL Apenas uma decisão é necessária]:** Selecione esta opção para que a revisão seja concluída depois que um dos tomadores de decisão tomar sua decisão.\

      Essa opção não estará disponível se você tiver designado um usuário na **[!UICONTROL Tomador de decisão principal]** menu suspenso.

   * **[!UICONTROL Fase privada]:** Quando essa opção é selecionada, comentários e decisões não ficam visíveis para pessoas que não estão adicionadas a esse estágio ou que não são Supervisores, Administradores ou Administradores de Faturamento na conta


1. (Opcional) Adicione revisores ao palco.
1. Considere o seguinte ao adicionar revisores:

   * Um revisor pode ser adicionado a uma prova apenas uma vez. (Não é possível adicionar a mesma pessoa a mais de um estágio na prova.)
   * Os revisores adicionados a uma fase privada podem ver apenas a etapa em que são adicionados na prova e os comentários feitos nessa etapa.
   * Por padrão, adicionar um usuário a um palco concede a esse usuário acesso para visualizar a prova a partir do momento em que a prova é criada.\

      O administrador do sistema pode configurar o sistema de prova para impedir que os usuários acessem a prova até que o workflow entre no estágio em que o usuário foi adicionado. Para obter mais informações, consulte

1. (Opcional) Clique em **[!UICONTROL Nova etapa]**, repita a Etapa 4 e a Etapa 5 para adicionar vários estágios ao fluxo de trabalho automatizado.
1. Continue criando a prova especificando as informações necessárias na variável [!UICONTROL Organizar] e [!UICONTROL Mais configurações] seções sobre [!UICONTROL Nova prova] conforme descrito em

## Diagramas de fluxo de trabalho automatizados

Ao configurar o workflow para sua prova, você observará um diagrama sendo criado. Cada estágio adicionado à prova será exibido no diagrama, indicando claramente as dependências entre os estágios. Os estágios privados são marcados com um ícone de chave.

O diagrama flutua, o que significa que ele permanecerá visível mesmo se você rolar a página para baixo.

Se não precisar ver o diagrama, poderá ocultá-lo (1).

![Diagrama.png](assets/diagram-350x93.png)

## Adicionar um estágio

Você pode adicionar uma etapa adicional a um fluxo de trabalho que esteja criando ou modificando.

1. Se você estiver adicionando um estágio a uma prova existente, vá para a página Detalhes da prova , conforme descrito em [Gerenciar detalhes de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. No **[!UICONTROL Fluxo de trabalho]** seção , clique em **[!UICONTROL Nova etapa]**.

1. Especifique as informações para o estágio como na etapa 4 em [!UICONTROL Criação de uma prova com um fluxo de trabalho automatizado] neste artigo.
1. Clique em **[!UICONTROL Adicionar estágio]**, depois clique em **[!UICONTROL Concluído]**.

## Excluir um estágio

1. Clique no ícone de lixeira disponível no canto superior direito do palco (1).\
   O ícone é exibido quando você passa o mouse sobre o palco.\
   ![deleting_a_stage.png](assets/deleting-a-stage-350x250.png)

## Configurações de preparo

* **[!UICONTROL Nome da fase]**: Aparece no diagrama de Fluxo de trabalho e é incluído nas notificações por email enviadas aos revisores.
* **[!UICONTROL Ativar estágio]**: Para cada estágio do fluxo de trabalho, você pode decidir quando ele deve ser ativado. Para o seu primeiro estágio, as seguintes opções estarão disponíveis:

   * Na criação da prova
   * Em uma data e hora específicas
   * Manualmente
   * Somente essas três opções estão disponíveis para o primeiro estágio. As outras opções ficarão disponíveis ao adicionar uma segunda etapa; eles exigem que você selecione um estágio principal.
   * Após o cumprimento do prazo anterior (requer a separação de um estágio principal)
   * Todas as decisões são Aprovadas ou [!UICONTROL Aprovado com alterações] (requer escolher um estágio principal)
   * Todas as decisões são Aprovadas (requer a escolha de um estágio pai)
   * Todas as decisões são tomadas (requer a escolha de um estágio principal)

* **[!UICONTROL Prazo]:** Você pode decidir como o prazo deve ser calculado em cada estágio de um workflow. As opções são:

   * A partir da criação da prova: No [!UICONTROL prazo] (9) é possível selecionar a data limite para a prova.
   * Da ativação do estágio: No [!UICONTROL prazo] selecione o número de dias úteis que serão adicionados à data de ativação do estágio para definir automaticamente um prazo na prova.

* **[!UICONTROL Bloquear]:** Há várias opções que determinam quando um estágio pode ser bloqueado. As opções incluem:

   * Bloqueio manual
   * Nunca
   * Quando a próxima etapa começar
   * Quando todas as decisões forem tomadas

**[!UICONTROL Tomador de decisão principal]**: Você define o principal decisor no palco. Os tomadores de decisão disponíveis aparecem na lista somente após ter adicionado os revisores ao palco.

>[!NOTE]
>
>Se você escolher um Principal decisor, apenas uma opção obrigatória não estará mais disponível neste estágio.

* **[!UICONTROL Apenas uma decisão é necessária]**: Você pode ativar essa opção em um estágio. Isto significa que a revisão estará concluída quando um dos decisores tomar a sua decisão.
* **[!UICONTROL Privacidade]:** Cada estágio pode ser privado. Se um estágio for privado, os comentários e as decisões não estarão visíveis para pessoas que não estão adicionadas a esse estágio ou que não são Supervisores, Administradores ou Administradores de faturamento na conta. Para obter mais informações, consulte [Visão geral do fluxo de trabalho automatizado](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md) .

## Adicionar revisores a um estágio

1. Insira um nome de contato ou endereço de email no campo , na parte inferior de cada estágio.
1. Clique no ícone de mais verde para adicioná-los.
1. Defina a função na prova.
1. Defina o alerta do email.
1. Ao configurar o primeiro estágio, você também tem a opção de alterar o Proprietário da prova.

   >[!NOTE]
   >
   >* Um revisor pode ser adicionado a uma prova apenas uma vez. Não é possível adicionar a mesma pessoa a mais de um estágio na prova.
   >* Os revisores que não são adicionados a uma fase privada não podem ver o estágio na prova ou nos comentários feitos nessa fase.



## Converter uma prova em um fluxo de trabalho automatizado

Você pode converter uma prova básica em Fluxo de trabalho automatizado.

1. Clique em **[!UICONTROL Converter em fluxo de trabalho automatizado]** no [!UICONTROL Detalhes da prova] página.
Depois que a prova é retrabalhada para o Fluxo de trabalho automatizado, todos os estágios são ativos, públicos e seus [!UICONTROL Bloquear palco] está definida como Manual por padrão. Todos os estágios permanecem com os usuários e suas configurações.

   * Ativate stage é definido como On proof creation em cada estágio.
   * O prazo calculado da opção é definido como Criação de prova em cada estágio.
   * Se apenas uma opção de decisão foi selecionada na prova básica, todas as etapas a selecionaram.
   * Em caso de prova de base [!UICONTROL Tomador de decisão principal] foi selecionado, então os estágios com esse recipient são definidos para ele e todos os outros têm definido como Nenhum.
   * O nome do palco permanece o mesmo.

## Adicionar um modelo adicional a um Fluxo de trabalho automatizado existente

Depois que uma prova básica é convertida em Fluxo de trabalho automatizado, você pode adicionar outro modelo a ela.

1. Na página Detalhes da prova , na seção Fluxo de trabalho , clique em **[!UICONTROL Adicionar modelo].**

   * As configurações do modelo determinam o que pode ser feito com uma prova à qual esse modelo foi adicionado. Por exemplo, se o modelo tiver o [!UICONTROL Adicionar um palco e Adicionar pessoas aos palcos] opções desativadas, botões para [!UICONTROL adicionar estágio] e [!UICONTROL compartilhar prova] não estará visível.
   * If [!UICONTROL Adicionar uma opção de estágio] está desativado no modelo em questão, depois de adicioná-lo ao [!UICONTROL Adicionar modelo] não estão visíveis.
   * Quando uma pessoa é adicionada a um estágio em um modelo de Fluxo de trabalho automatizado, mas também já está presente na prova, se esse modelo for aplicado, o sistema removerá essa pessoa do estágio automaticamente. Se não houver mais ninguém adicionado a esse estágio específico, o seguinte erro será mostrado, pois o sistema não permitirá adicionar um estágio vazio ao fluxo de trabalho.

      ![error_when_adding_template.png](assets/error-when-adding-template-350x66.png)
