---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Criar e Gerenciar Exibições Personalizadas em [!DNL Workfront Proof]
description: É possível criar exibições personalizadas de seus arquivos e provas para listar os itens desejados da maneira que você desejar que eles sejam exibidos. Você também pode exportar as informações na visualização personalizada como um relatório (em CSV, valor separado por vírgulas, formato de arquivo).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 7c6f3fdd-f767-4e8d-937a-1c7645aba55b
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '2458'
ht-degree: 0%

---

# Criar e Gerenciar Modos de Exibição Personalizados no [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

É possível criar exibições personalizadas de seus arquivos e provas para listar os itens desejados da maneira que você desejar que eles sejam exibidos. Você também pode exportar as informações na visualização personalizada como um relatório (em CSV, valor separado por vírgulas, formato de arquivo).

>[!NOTE]
>
>As exibições personalizadas estão disponíveis apenas nos planos Select e Premium. Entre em contato com nossa equipe de vendas para obter uma cotação.

## Criar uma visualização personalizada

Ao criar uma visualização personalizada, você pode escolher:

* Se incluir provas, arquivos ou ambos
* Quais colunas são exibidas
* Por qual coluna classificar
* A ordem de classificação da coluna (crescente ou decrescente)
* Quais tipos de filtros usar para determinar quais informações são incluídas na exibição

Depois que a exibição personalizada é criada, ela fica disponível para uso imediatamente. O nome da nova exibição também está incluído no menu suspenso no cabeçalho Minhas exibições personalizadas (abaixo das exibições padrão).

Para criar uma exibição personalizada:

1. Vá para a página **[!UICONTROL Exibições]**.
1. Para obter mais informações sobre exibições, consulte [Gerenciar Itens na Página Exibições em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).
1. Desempenhe uma das ações a seguir, dependendo se deseja criar uma nova exibição personalizada do zero ou criar uma nova exibição personalizada com base em uma exibição padrão existente:

   * Para criar uma nova view personalizada com base em uma view padrão existente: no menu suspenso, selecione a view padrão existente que deseja usar como base para a nova view personalizada. Clique no ícone **[!UICONTROL Exibir configurações]** e em **[!UICONTROL Copiar]** para novo modo de exibição personalizado.

   * ![](assets/proof-custom-view-icon.png)

   * Para criar um novo modo de exibição personalizado do zero: clique no ícone **[!UICONTROL Novo Modo de Exibição]**.
   * ![](assets/proof-newview.png)

1. Na seção **[!UICONTROL Detalhes]**, especifique as seguintes informações:

   * **[!UICONTROL Nome]** (obrigatório): o nome da nova exibição. Use um nome exclusivo para que os usuários possam encontrar facilmente a exibição personalizada no menu suspenso nas Exibições.
   * **[!UICONTROL Itens]**: selecione se deseja que provas e arquivos, provas apenas ou arquivos apenas sejam incluídos no modo de exibição. Por padrão, provas e arquivos são incluídos.

1. Na seção **[!UICONTROL Colunas]**, determine quais colunas você deseja incluir no modo de exibição personalizado.

   1. Clique no ícone de seta para a direita.
   1. ![](assets/proof-view-rightarrow.png)

   1. Clique duas vezes no nome da coluna selecionada.
   1. Você deve selecionar pelo menos uma coluna, e uma coluna pode ser adicionada apenas uma vez.
   1. Selecione uma coluna na área **[!UICONTROL Colunas disponíveis]** que você deseja incluir no novo modo de exibição.
   1. As colunas foram movidas da lista **[!UICONTROL Colunas disponíveis]** para a lista **[!UICONTROL Colunas selecionadas]**.

   1. Você pode selecionar entre as colunas padrão ou escolher Campos personalizados e Motivos de decisão para serem colunas em sua exibição personalizada. (Se você tiver essas colunas configuradas em sua conta, elas aparecerão abaixo da área Lista padrão de colunas Disponíveis .)
   1. Colunas padrão que você pode incluir

      <table style="table-layout:auto">
      <thead>

      </thead>
      <tbody>  
      <tr>   
      <td><strong>Nome do estágio ativo</strong></td>   
      <td>Nome do estágio ativo no fluxo de trabalho automatizado.</td>  
      </tr>  
      <tr>   
      <td><strong>Comentários</strong></td>   
      <td>O número de comentários recebidos.</td>
      </tr>  
      <tr>   
      <td><strong>Contador</strong></td>
      <td>Mostra um número de provas que foram carregadas na sua conta (você precisa ter uma opção de contador de provas ativada nas Configurações da conta).</td>
      </tr>
      <tr>
      <td><strong>Criado</strong></td>
      <td>A data e a hora em que o item foi criado.</td>
      </tr>
      <tr>
      <td><strong>Criador</strong></td>
      <td>O usuário que criou o item.</td>
      </tr>
      <tr>
      <td><strong>[!UICONTROL Data de adição à prova]</strong></td>
      <td>A data em que você foi adicionado à prova. </td>
      </tr>
      <tr>
      <td><strong>Prazo</strong></td>
      <td>O prazo para toda a prova.</td>
      </tr>
      <tr>
      <td><strong>Decisões</strong></td>
      <td>O número de decisões fornecidas do número esperado (por exemplo, 0 de 1, 1 de 1, etc.)</td>
      </tr>
      <tr>
      <td><strong>[!UICONTROL Downloads]</strong></td>
      <td>O número de vezes que o arquivo original foi baixado.</td>
      </tr>
      <tr>
      <td><strong>Nome do arquivo</strong></td>
      <td>O nome do arquivo ou da prova.</td>
      </tr>
      <tr>
      <td><strong>Pasta</strong></td>
      <td>A pasta que contém o item.</td>
      </tr>
      <tr>
      <td><strong>Última atividade</strong></td>
      <td>A data e hora da última atividade no item.</td>
      </tr>
      <tr>
      <td><strong>Última decisão em</strong></td>
      <td>A data e a hora da última decisão tomada.</td>
      </tr>
      <tr>
      <td><strong>Meu prazo final</strong></td>
      <td>Seu próprio prazo nas provas em que você é explicitamente adicionado como Revisor/Aprovador (se aplicado).</td>
      </tr>
      <tr>
      <td><strong>Proprietário</strong></td>
      <td>O proprietário do item.</td>
      </tr>
      <tr>
      <td><strong>País do proprietário</strong></td>
      <td>O país registrado no sistema para o proprietário da prova. </td>
      </tr>
      <tr>
      <td><strong>Prova principal</strong></td>
      <td>O nome da prova principal.</td>
      </tr>
      <tr>
      <td><strong>Progresso</strong></td>
      <td><p>Barra de progresso. Exibe provas que ainda não foram iniciadas, abertas, comentadas ou decididas.</p><p>Essas informações não estão classificadas em.</p></td>
      </tr>
      <tr>
      <td><strong>Nome da prova</strong></td>
      <td>O nome da prova.</td>
      </tr>
      <tr>
      <td><strong>Tipo de prova</strong></td>
      <td><p>O tipo de prova: Arquivo estático, Página da Web estática, Web interativa (.zip upload), Página da Web interativa (https), Vídeo, Áudio e Outros. </p><p>As provas combinadas são identificadas como "Tipo de prova combinado". Tipo de arquivo da prova.</p></td>
      </tr>
      <tr>
      <td><strong>Tamanho do arquivo (MB)</strong></td>
      <td><p>Tamanho do arquivo da prova em relação à cota de uso do disco.</p><p>Essas informações são fornecidas para a versão atual da prova. Se não houver uma versão atual, ela será para a versão mais recente.</p></td>
      </tr>
      <tr>
      <td><p> </p><p><strong>Prazo da fase ativa</strong></p></td>
      <td>Prazo dos estágios no fluxo de trabalho automatizado.</td>
      </tr>
      <tr>
      <td><strong>Nome do estágio</strong></td>
      <td>Nome de cada estágio no fluxo de trabalho automatizado. Isso inclui estágios anteriores, ativos e futuros.</td>
      </tr>
      <tr>
      <td><strong>Estado</strong></td>
      <td>Ativo, bloqueado, rascunho ou enviado.</td>
      </tr>
      <tr>
      <td><strong>Status</strong></td>
      <td>Pendente, Alterações necessárias, Aprovado com alterações, Aprovado ou Não relevante.</td>
      </tr>
      <tr>
      <td><strong>Tags</strong></td>
      <td>Quaisquer tags anexadas ao item.</td>
      </tr>
      <tr>
      <td><strong>Nomes dos próximos estágios</strong></td>
      <td> Nome de cada estágio que ainda não foi iniciado no fluxo de trabalho automatizado. </td>
      </tr>
      <tr>
      <td><strong>Contador de versão</strong></td>
      <td> O número de versões do item. </td>
      </tr>
      <tr>
      <td><strong>Número da versão da prova</strong></td>
      <td><i>O número da versão da prova.</i></td>
      </tr> 
      </tbody>
      </table>

   1. (Opcional) Siga um destes procedimentos para mover a coluna para a área **[!UICONTROL Colunas selecionadas]** de modo que ela seja incluída na nova exibição:

      * Reordene quaisquer colunas na lista **[!UICONTROL Colunas selecionadas]**.
      * A ordem em que as colunas são mostradas na lista **[!UICONTROL Colunas selecionadas]** determina a ordem em que as colunas são exibidas no modo de exibição personalizado.
      * As colunas estão visíveis na lista **[!UICONTROL Colunas selecionadas]** na ordem em que foram adicionadas na lista **[!UICONTROL Colunas disponíveis]**.

      * Para reordenar uma coluna na lista **[!UICONTROL Colunas selecionadas]**, selecione o nome da coluna e arraste-o para cima ou para baixo na lista.

      * Remova uma coluna da lista **[!UICONTROL Colunas selecionadas]**, clicando no nome da coluna selecionada e clicando na seta **[!UICONTROL Esquerda]**. Como alternativa, você pode clicar duas vezes no nome da coluna selecionada (a coluna é movida de volta para a lista **[!UICONTROL Colunas disponíveis]**).

      * Uma coluna só pode ser adicionada uma vez. Por exemplo, se você mover a coluna Comentários da lista [!UICONTROL Disponível] para [!UICONTROL Colunas selecionadas], o nome dessa coluna desaparecerá da lista [!UICONTROL Colunas disponíveis].

1. Na seção **[!UICONTROL Sorting]**, especifique as seguintes informações:

   * **Classificar por:** use a guia [!UICONTROL Classificação] se desejar definir uma ordem específica na qual os itens são listados no modo de exibição personalizado. Se você não selecionar uma coluna para classificação, o padrão será Nenhuma coluna, ou seja, nenhuma coluna ou ordem de classificação especial.
   * Somente as colunas selecionadas na guia [!UICONTROL Colunas] estão incluídas na lista suspensa [!UICONTROL Classificar por coluna].
   * **Crescente ou Decrescente:** selecione se deseja classificar a coluna em ordem crescente ou decrescente por padrão.

1. Use a seção **[!UICONTROL Filtros]** para definir um ou mais critérios para selecionar itens a serem incluídos no modo de exibição Personalizado. Os filtros são especialmente úteis se você quiser usar sua visualização personalizada como um relatório.
1. Para incluir todos os itens no modo de exibição personalizado, ignore a seção **[!UICONTROL Filtros]**.
1. Filtros disponíveis:

   * **Campo:** Selecione o Campo para este filtro (Comentários é o campo padrão.) A lista Campo contém todos os campos Padrão (como na guia [!UICONTROL Colunas]). A lista não está limitada às colunas selecionadas para exibição.
   * **Operador:** os Operadores disponíveis para o filtro dependem do tipo de Campo selecionado. Selecione um Operador que mostre a relação entre o Campo e o campo de valor. Você preencherá essas informações posteriormente.
   * **Valor:** Selecione ou insira o valor escolhido neste Campo, de acordo com o campo e o Operador selecionados. Dependendo do Operador escolhido, pode haver um campo Valor, dois ou nenhum. Veja os exemplos abaixo.
   * **Os filtros são aplicados usando a seguinte lógica:** Os critérios de filtro entre campos diferentes usarão o operador AND. Vários critérios de filtro que usam o mesmo campo usarão o operador OR para o mesmo campo.

     Se quiser ver apenas provas com comentários zero, selecione os seguintes valores:

      * Campo: Comentários
      * Operador: Igual a
      * Campo de valor: 0

     Se quiser ver apenas provas com dois ou mais comentários, selecione os seguintes valores:

      * Campo: Comentários
      * Operador: maior ou igual a
      * Campo de valor: 2

     Se quiser ver apenas provas com comentários entre 1 e 4, selecione os seguintes valores:

      * Campo: Comentários
      * Operador: Entre
      * Campo de valor (primeiro campo): 1
      * Campo de valor (segundo campo): 4

        Você pode alterar um filtro adicionado ao modo de exibição Personalizado sem problemas ou removê-lo clicando no ícone cruzado ao lado do filtro [!UICONTROL instalação], se necessário.

        Como a lista Campo não está limitada às colunas selecionadas na guia [!UICONTROL Colunas], tenha cuidado ao criar um filtro que inclua uma coluna que você não selecionou para exibição no modo de exibição personalizado. Por exemplo, o filtro a seguir para a exibição selecionará todas as provas com um valor de contador de Versão de 2 ou mais:

         * Campo = Contador de versão
         * Operador = Maior ou igual a
         * Campo de valor = 2

           >[!NOTE]
           >
           >Você pode alterar um filtro adicionado ao modo de exibição Personalizado sem problemas ou removê-lo clicando no ícone cruzado ao lado do filtro [!UICONTROL instalação], se necessário.



1. Na seção **[!UICONTROL Compartilhamento]**, selecione quais usuários da sua conta poderão ver sua exibição Personalizada.
1. As exibições personalizadas são específicas do usuário que as cria. Por padrão, a nova Exibição personalizada fica visível somente para seu criador; no entanto, você pode optar por compartilhar a exibição personalizada escolhendo uma das seguintes opções:

   * **Somente você pode ver este modo de exibição personalizado** (padrão): selecione esta opção se desejar que o modo de exibição personalizado fique disponível somente para você.
   * **Todos os usuários podem ver este modo de exibição personalizado**: selecione esta opção para disponibilizar o modo de exibição personalizado a todos os usuários da sua conta.
   * **Selecione os usuários que podem ver este modo de exibição personalizado**: selecione esta opção para disponibilizar o modo de exibição personalizado somente para usuários específicos.
   * Comece digitando o nome ou o endereço de email do usuário que deseja que tenha acesso à visualização personalizada e clique no nome quando ele aparecer na lista suspensa.
   * Se você optar por não compartilhar sua visualização com outros usuários neste momento, poderá fazê-lo posteriormente editando a visualização personalizada.

1. Clique em **[!UICONTROL Criar]**.
1. A Exibição personalizada é exibida e está disponível na página [!DNL Views]. Para obter mais informações sobre exibições, consulte [Gerenciar Itens na [!DNL Views] Página em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

## Editar Exibições Personalizadas

É possível editar uma visualização personalizada facilmente. Para editar uma exibição personalizada:

1. Vá para a página **[!UICONTROL Exibições]**.\
   Para obter mais informações sobre exibições, consulte [Gerenciar Itens na Página Exibições em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Clique no botão [!UICONTROL Exibições] (1)
1. Selecione a exibição que deseja editar no menu suspenso.\
   ![](assets/proof-view-edit.png)

1. Clique no botão **[!UICONTROL Opções de Exibição]** e em **[!UICONTROL Editar exibição]**.\
   ![](assets/proof-view-options.png)\
   A página Editar Exibição Personalizada é exibida.

1. Clique no menu [!UICONTROL Ações]. (3)\
   Esse botão só estará disponível se você incluir a coluna Nome da prova na visualização.
1. Selecione [!UICONTROL Editar exibição] no menu. (4) \
   ![editing_custom_view_2.png](assets/editing-custom-view-2-350x258.png)

1. A página Editar exibição personalizada é exibida.

![Editar_exibição_personalizada.png](assets/edit-custom-view-page-350x543.png)

>[!NOTE]
>
>Se você editar a visualização Personalizada, as colunas na lista Colunas selecionadas serão organizadas em ordem alfabética automaticamente. Você precisará reorganizá-los, se necessário, antes de atualizar a visualização.


## Copiando Exibições Personalizadas

A função Copiar exibição permite fazer facilmente uma cópia de uma exibição personalizada existente. Isso é muito útil, por exemplo, se você quiser configurar exibições separadas para todos os designers, sendo que cada exibição é a mesma, exceto para o proprietário da prova (designer).

Para copiar uma exibição personalizada:

1. Vá para a página **[!UICONTROL Exibições]**.\
   Para obter mais informações sobre exibições, consulte [Gerenciar Itens na Página Exibições em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Clique no botão **[!UICONTROL Exibições]**. (1)
1. Selecione a Exibição personalizada na lista. (2)
1. Clique no menu **[!UICONTROL Ações]**. (3)\
   Esse botão só estará disponível se você incluir a coluna Nome da prova na visualização.

1. Selecione [!UICONTROL Copiar] no menu. (4)\
   ![copying_custom_view.png](assets/copying-custom-view-350x258.png)

1. Na página Copiar modo de exibição personalizado, todas as configurações originais são preenchidas. Modifique o modo de exibição Personalizado conforme sua escolha e clique no botão **[!UICONTROL Copiar modo de exibição]**. Você será direcionado imediatamente à sua nova visualização.\
   ![](assets/copy-custom-view-page-350x542.png)

## Compartilhamento de exibições personalizadas

A função Compartilhar visualização permite compartilhar uma visualização com outros usuários em sua conta se você ainda não os selecionou na seção Compartilhamento da visualização. Quando você compartilha um modo de exibição personalizado com outros usuários, ele aparece na seção [!UICONTROL Meus modos de exibição personalizados] do menu suspenso Modos de Exibição.

Para compartilhar uma visualização personalizada com outros usuários:

1. Vá para a página **[!UICONTROL Exibições]**.\
   Para obter mais informações sobre exibições, consulte [Gerenciar Itens na Página Exibições em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Clique no botão **[!UICONTROL Exibições]** (1)
1. Selecione a Exibição personalizada na lista (2)
1. Clique no menu **[!UICONTROL Ações]**. (3)\
   Esse botão só estará disponível se você incluir a coluna Nome da prova na visualização.

1. Selecione [!UICONTROL Compartilhar exibição] no menu (4)
1. A página Editar exibição personalizada será exibida.
1. Na seção [!UICONTROL Compartilhamento], selecione os usuários com os quais deseja compartilhar o modo de exibição e clique em **[!UICONTROL Atualizar modo de exibição]**.

   ![Editar_exibição_personalizada_página__1_.png](assets/edit-custom-view-page--1--350x543.png)

## Exportando exibições personalizadas para arquivos CSV

Para exportar os dados de uma exibição personalizada para um arquivo CSV:

1. Vá para a página **[!UICONTROL Exibições]**.\
   Para obter mais informações sobre exibições, consulte [Gerenciar Itens na Página Exibições em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Clique no botão **[!UICONTROL Exibições]**. (1)
1. Selecione a Exibição personalizada na lista. (2)
1. Clique no menu **[!UICONTROL Ações]**. (3)\
   Esse botão só estará disponível se você incluir a coluna Nome da prova na visualização.

1. Selecione [!UICONTROL Exportar para CSV] no menu. (4)\
   ![export_custom_view.png](assets/exporting-custom-view-350x258.png)\
   Em uma janela separada do navegador, &quot;Gerando relatório: 100%&quot; é exibido mais o número de registros (o número de itens incluídos no relatório da exibição personalizada)

1. (Condicional) Se uma mensagem de segurança for exibida indicando que o download do relatório está bloqueado no momento, clique em para permitir que o download continue.
1. Clique em **[!UICONTROL Salvar]** quando a janela Download de Arquivo aparecer perguntando se você deseja abrir ou salvar o arquivo.
1. Selecione um local no computador e salve o arquivo.

## Exclusão de Exibições Personalizadas

É possível excluir uma Exibição personalizada facilmente. Para fazer isso:

1. Vá para a página **[!UICONTROL Exibições]**.\
   Para obter mais informações sobre exibições, consulte [Gerenciar Itens na Página Exibições em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Clique no botão **[!UICONTROL Exibições]**.
1. Selecione a visualização Personalizada na lista
1. Clique no menu **[!UICONTROL Ações]**. (3)\
   Esse botão só estará disponível se você incluir a coluna Nome da prova na visualização.

1. Selecione [!UICONTROL Excluir] no menu. (4)\
   ![excluindo_modo_de_exibição_personalizado.png](assets/deleting-custom-view-350x258.png)

1. Clique em **[!UICONTROL Excluir]** (5) para confirmar que deseja excluir o modo de exibição Personalizado atual\
   ![excluir__1_.png](assets/delete--1--350x187.png)

1. A exibição padrão Todos os itens é exibida e a exibição personalizada excluída não aparece mais no menu suspenso **[!UICONTROL Exibições]**.
