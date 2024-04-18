---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Instalar um pacote de promoção de ambiente
description: O recurso de promoção de ambiente tem como objetivo fornecer a capacidade de mover objetos relacionados à configuração de um ambiente para outro. Saiba como instalar um pacote de promoção de ambiente em um ambiente de destino.
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: 92a7a2df142d7736417b903949a5a667cff53913
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 0%

---

# Instalar um pacote de promoção de ambiente

>[!NOTE]
>
>Para instalar um pacote, você deve estar conectado ao ambiente em que deseja instalar o pacote. Este é o ambiente no qual você está copiando objetos **para**.

1. Vá para o ambiente em que deseja instalar o pacote.
1. Clique em **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível), clique no link **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **[!UICONTROL Configuração]** ![Ícone de Configuração](/help/_includes/assets/gear-icon-setup.png).
1. Selecionar **Sistema** na navegação à esquerda, selecione **Promoção do ambiente**.
1. Selecione o pacote na lista exibida.
1. Para cada objeto que tiver uma colisão, selecione como resolver a colisão.

   Para resolver uma colisão, clique na seta suspensa ao lado do tipo de objeto e selecione a ação que deseja executar.

   Para obter mais informações, consulte [Colisões](#collisions) neste artigo
1. Para implantar o pacote no novo ambiente, clique em **Implantar** no canto superior direito da tela.

## Colisões

As colisões ocorrem quando um objeto que faz parte do pacote de instalação tem o mesmo nome de um objeto que já existe no ambiente de destino. Quando isso ocorrer, você poderá selecionar como resolver a colisão. As colisões são resolvidas no nível do objeto.

Você pode ver as colisões clicando na lista suspensa ao lado de cada tipo de objeto. As colisões são exibidas na coluna Colisão.

Para resolver uma colisão, selecione uma ação na coluna Ação de implantação ou use a ação padrão que já está sendo exibida.

* **Criar com novo nome**: crie um novo objeto no ambiente de destino. Se o objeto existir no ambiente de destino, você poderá criar um novo objeto com um novo nome. Se não existir no ambiente de destino, você poderá criar o objeto com um novo nome ou com o nome que o objeto tem no pacote.
* **Usar existente**: o objeto no pacote não está instalado e o objeto que já existia no ambiente de destino não é alterado.
* **Substituir**: o objeto no pacote substitui o objeto existente no ambiente de destino.

  Você também pode escolher objetos para substituir mesmo se uma colisão não for detectada.

  Para obter detalhes sobre como a substituição afeta objetos pai e filho, consulte
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

Os valores padrão são `Create new` se o objeto não existir no ambiente de destino e `Use existing` se o objeto não existir no ambiente de destino. Você pode reverter para o mapeamento padrão clicando em **Redefinir para mapeamento padrão**.

## Substituição de objetos pai e filho

Alguns objetos no pacote de promoção podem ter objetos filho. Por exemplo, um projeto (principal) tem tarefas (secundárias). Ao substituir um objeto pai, os objetos filho são manipulados da seguinte maneira:

* Os objetos filho que existem no pacote e no target serão atualizados no target para corresponder ao pacote.
* Os objetos filho que existem no pacote, mas não no destino, serão criados.
* Os objetos filho que existem no destino, mas não no pacote, permanecerão inalterados.

Essa funcionalidade afeta os seguintes objetos pai e filho:

| Objeto pai | Objetos filho |
|---|---|
| Projeto | Tarefa<br>QueueDef (Definição de Fila)<br>Regra de Encaminhamento |
| Modelo | TarefaModelo<br>QueueDef (Definição de Fila)<br>Regra de Encaminhamento |
| Parâmetro (campo de formulário personalizado) | ParameterOption (opção de campo de formulário personalizado) |
| CalendarInfo | SeçãoCalendário |
| QueueDef (Definição de Fila) | QueueTopicGroup<br>TópicoFila |

