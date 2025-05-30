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
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: 8fe93796b2bc89352ac2c924d6a5e3bf25551ff0
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 0%

---

# Instalar um pacote de promoção de ambiente

Depois de criar um pacote, você pode instalá-lo em um ambiente diferente.

Você deve instalar um pacote no ambiente para o qual deseja copiar os objetos **para**. Por exemplo, se você estiver configurando um projeto no ambiente Personalizado de atualização da sandbox e promovendo-o no ambiente de produção, será necessário instalar o pacote no ambiente de produção.

>[!IMPORTANT]
>
>* Se sua sandbox de atualização personalizada for atualizada enquanto você estiver configurando o objeto para promoção de ambiente, essa configuração será perdida na atualização. Recomendamos que você não atualize sua sandbox de atualização personalizada a menos que todos os objetos e pacotes de promoção de ambiente pendentes tenham sido promovidos com êxito.
>* Os objetos criados no ambiente de destino como parte da instalação do pacote **não** têm a mesma ID que o objeto no ambiente original. Isso se deve ao fato de que as IDs são atribuídas pelo sistema quando os objetos são criados.

## Requisitos de acesso

Você deve ter o seguinte:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plano</strong>
   </td>
   <td> Prime ou Ultimate (somente novos planos)
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenças</strong>
   </td>
   <td> [!UICONTROL Padrão]
   </td>
  </tr>
   <tr>
   <td>Configurações de nível de acesso
   </td>
   <td>Você deve ser um administrador [!DNL Workfront].
   </td>
  </tr>
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Pré-requisitos

Um pacote de promoção de ambiente deve ser criado antes de ser instalado.

Para obter instruções, consulte [Criar ou editar um pacote de promoção de ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md).

## Status do pacote para instalação

Um pacote deve estar com o status ATIVO para ser instalado em seu ambiente de produção.

Recomendamos mover o pacote para o status TESTANDO e instalar em outra sandbox para testar o pacote.  Se esse teste for bem-sucedido, sem erros, mova o pacote para ATIVE para instalá-lo no ambiente de produção.

Para editar o status de um pacote:

1. Selecione o pacote conforme descrito em [Editar ou montar um pacote existente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-or-edit-an-environment-promotion-package) no artigo Criar e editar pacotes de promoção de ambiente.
1. Clique em **Editar Pacote**.
1. Clique em **Status**.
1. Selecione o status desejado no menu suspenso.

Para obter mais informações sobre status, consulte [Status de promoção do ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) no artigo Visão geral da movimentação de objetos entre ambientes do Workfront.

## Instalar um pacote

>[!NOTE]
>
>* Para instalar um pacote, você deve estar conectado ao ambiente em que deseja instalar o pacote. Este é o ambiente no qual você está copiando os objetos **para**.

1. Vá para o ambiente em que deseja instalar o pacote.
1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique no ícone **[!UICONTROL Instalação]** ![Instalação](/help/_includes/assets/gear-icon-setup.png).
1. Selecione **Sistema** na navegação à esquerda e **Promoção do ambiente**.
1. Selecione o pacote na lista exibida.
1. Para cada objeto que tiver uma colisão, selecione como resolver a colisão.

   Para resolver uma colisão, clique na seta suspensa ao lado do tipo de objeto e selecione a ação que deseja executar.

   Para obter mais informações, consulte [Conflitos](#collisions) neste artigo
1. Para implantar o pacote no novo ambiente, clique em **Implantar** no canto superior direito da tela.

## Colisões

Uma colisão é um objeto encontrado no ambiente de destino de uma instalação que corresponde a um dos objetos que estão sendo instalados do ambiente de origem. As colisões são detectadas comparando os nomes e as IDs dos objetos de origem com os objetos no ambiente de destino. As colisões também são detectadas comparando os objetos de origem com os registros de objetos instalados anteriormente.

Quando ocorre uma colisão, você pode selecionar como resolver a colisão. As colisões são resolvidas no nível do objeto.

Você pode exibir colisões clicando na lista suspensa ao lado de cada tipo de objeto. As colisões são exibidas na coluna Colisão.

>[!NOTE]
>
>As colisões detectadas podem não ser os objetos que você deseja substituir ou usar na instalação. Recomendamos validar as colisões detectadas para garantir que os destinos de instalação estejam corretos.

Para resolver uma colisão, selecione uma ação na coluna Ação de implantação ou use a ação padrão que já está sendo exibida.

* **Criar com novo nome**: criar um novo objeto no ambiente de destino. Se o objeto existir no ambiente de destino, você poderá criar um novo objeto com um novo nome. Se não existir no ambiente de destino, você poderá criar o objeto com um novo nome ou com o nome que o objeto tem no pacote.
* **Usar existente**: o objeto no pacote não está instalado e o objeto que já existia no ambiente de destino não foi alterado.
* **Substituir**: o objeto no pacote substitui o objeto existente no ambiente de destino.

  Você também pode escolher objetos para substituir mesmo se uma colisão não for detectada.

  Para obter detalhes sobre como a substituição afeta objetos pai e filho, consulte [Substituição de objetos pai e filho](#overwriting-parent-and-child-objects) neste artigo.
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

Os valores padrão são `Create new` se o objeto não existir no ambiente de destino e `Use existing` se o objeto não existir no ambiente de destino. Você pode reverter para o mapeamento padrão clicando em **Redefinir para o mapeamento padrão**.

## Substituição de objetos pai e filho

Alguns objetos no pacote de promoção podem ter objetos filho. Por exemplo, um projeto (principal) tem tarefas (secundárias). Ao substituir um objeto pai, os objetos filho são manipulados da seguinte maneira:

* Os objetos filho que existem no pacote e no target serão atualizados no target para corresponder ao pacote.
* Os objetos filho que existem no pacote, mas não no destino, serão criados.
* Os objetos filho que existem no destino, mas não no pacote, permanecerão inalterados.

Essa funcionalidade afeta os seguintes objetos pai e filho:

| Objeto pai | Objetos filho |
|---|---|
| Projeto | Tarefa<br>QueueDef (Definição de Fila)<br>RoutingRule |
| Modelo | TemplateTask<br>QueueDef (Definição de Fila)<br>RoutingRule |
| Parâmetro (campo de formulário personalizado) | ParameterOption (opção de campo de formulário personalizado) |
| CalendarInfo | SeçãoCalendário |
| QueueDef (Definição de Fila) | QueueTopicGroup<br>QueueTopic |

