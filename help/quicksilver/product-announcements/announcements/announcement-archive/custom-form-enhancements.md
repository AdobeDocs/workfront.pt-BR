---
title: Aprimoramentos de formulários personalizados
description: Os seguintes aprimoramentos significativos foram feitos no gerenciamento de formulários personalizados na versão 22.2.
author: Luke
feature: Product Announcements, Custom Forms
exl-id: 81568eab-8a65-4767-b8ab-fb9353a90bb6
source-git-commit: 8dac7959919014d7bfbbbd39d193d026ca31c4b2
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 0%

---

# Aprimoramentos de formulários personalizados

Os seguintes aprimoramentos significativos foram feitos no gerenciamento de formulários personalizados na versão 22.2.

## Adicionar widgets de ativos

Você pode incorporar imagens em seus formulários personalizados. Isso permite que você se comunique com os usuários do formulário personalizado de uma maneira mais interativa e visual. Tipos de widget adicionais serão disponibilizados em breve.

![](assets/image-in-custom-form.png)

Quando um formulário personalizado contendo um widget é anexado a um objeto, os usuários que trabalham com o objeto podem vê-lo nas seguintes áreas:

* A área Detalhes do objeto (por exemplo, para um projeto, a área Detalhes do projeto)&#x200B;

  ![](assets/see-image-details-page.png)

* A caixa Editar do objeto, se ele tiver a nova aparência da experiência do Adobe Workfront (por exemplo, as caixas Editar projeto e Editar tarefa)&#x200B;

  ![](assets/image-see-in-edit.png)

Atualmente, os usuários não podem ver o widget nas seguintes áreas:&#x200B;

* Listas e relatórios
* Início e resumo
* A caixa Editar do objeto, se ele não tiver a nova aparência e comportamento da experiência do Adobe Workfront (por exemplo, a caixa Editar Despesa)
* &#x200B;O aplicativo móvel do Workfront

## Associar um formulário personalizado a vários tipos de objeto

Você pode associar vários tipos de objetos a qualquer novo formulário personalizado:

![](assets/new-custom-form-object-types.png)

Ou qualquer formulário personalizado existente:

![](assets/add-object-type-existing-form.png)

Isso permite criar um único formulário personalizado para usar em projetos, tarefas, problemas e qualquer outro tipo de objeto que seja compatível com formulários personalizados.

Isso é especialmente útil quando você converte um problema ou tarefa, pois é possível transportar um formulário personalizado e seus dados para o objeto convertido. Não é mais necessário criar e manter cópias exatas do mesmo formulário personalizado para vários tipos de objetos. Adicione o formulário personalizado ao projeto manualmente.

>[!INFO]
>
>**Exemplo:**
>
>Alguém envia uma solicitação de TI interna (problema) e fornece detalhes sobre o que é necessário em um formulário personalizado anexado.
>
>Converta o problema em um projeto para os usuários que trabalharão nele.
>
>Como o formulário personalizado que contém os detalhes do remetente está associado aos tipos de objeto Problema e Projeto, o formulário personalizado e todos esses detalhes são transferidos para o projeto durante a conversão.

>[!NOTE]
>
>Quando a conversão ocorrer, o formulário personalizado já deverá estar associado ao tipo de objeto para o qual você está convertendo.

Considere o seguinte ao criar ou editar um formulário personalizado de vários objetos:

* [Opções de permissão para quebras de seção](#permission-options-for-section-breaks)
* [Compatibilidade de campo personalizado calculada](#calculated-custom-field-compatibility)
* [Cuidado ao excluir um tipo de objeto de um formulário personalizado](#caution-about-deleting-an-object-type-from-a-custom-form)

### Opções de permissão para quebras de seção

O conjunto de opções de permissão de quebra de seção disponíveis para os tipos de objeto Problema, Tarefa, Projeto e Usuário tem uma opção de permissão a mais do que o conjunto de opções de permissão para todos os outros tipos de objeto: Edição limitada.

![](assets/section-break-permissions-limited-edit.png)

O conjunto de permissões de quebra de seção disponível para todos os outros tipos de objeto (Portfolio, Documento, Programa, Despesa, Empresa, Iteração, Registro de faturamento e Grupo) não inclui Edição limitada:

![](assets/section-break-permissions-no-limited-edit.png)

Em um formulário personalizado associado a tipos de objeto de ambos os grupos, o sistema usa um conjunto comum de permissões de quebra de seção que funcionam para todos os tipos de objeto. Especificamente, em vez de usar a opção de permissão Edição limitada, esse conjunto comum substitui a opção de permissão Editar pela opção de permissão Edição limitada. A opção Editar é compatível com todos os tipos de objeto.

Ao associar um tipo de objeto que usa opções de permissão diferentes dos outros tipos de objeto que já estão em um formulário personalizado, uma mensagem é exibida e permite que você alterne para o conjunto comum de opções de permissão que será usado para o formulário. Essa alteração se aplicará a todos os campos, mesmo que eles não estejam em uma quebra de seção.

### Compatibilidade de campo personalizado calculada

Em um formulário personalizado de vários objetos, se um campo calculado referenciar campos que estejam disponíveis para uso com todos os tipos de objeto associados do formulário (como {name}, {description} e {entryDate}, que estão disponíveis para vários tipos de objeto), os dados serão calculados corretamente, independentemente do objeto ao qual você os anexa.

Por exemplo, se você tiver um formulário de vários objetos para projetos e problemas e adicionar um campo calculado contendo a expressão {name}, o campo exibirá o nome do projeto quando você adicionar o formulário a um projeto, e o nome da tarefa de você adicionará o formulário a uma tarefa.

Campos não compatíveis com o objeto exibirão N/D no formulário.

>[!INFO]
>
>**Exemplo:** em um formulário personalizado associado ao tipo de objeto Tarefa, você cria um campo personalizado calculado que faz referência ao campo interno Atribuído a: Nome para que ele possa mostrar o nome do responsável principal sempre que o formulário for anexado a uma tarefa:
>
>```
>Assigned To: Name{assignedTo}.{name}
>```
>
>Posteriormente, você adiciona o tipo de objeto Projeto ao formulário personalizado. Uma mensagem de aviso informa que o tipo de objeto Project é incompatível com o campo personalizado calculado. Isso ocorre porque o campo Atribuído a não está disponível para projetos.

Quando isso ocorrer, você poderá executar um dos seguintes procedimentos:

* Remova um dos dois itens incompatíveis do formulário personalizado, seja o tipo de objeto ou o campo de referência.
* Mantenha ambos os itens e use a variável de filtro curinga `$$OBJCODE` como uma condição em uma expressão IF para criar duas versões diferentes do campo Encargo. Isso permite que o campo funcione com êxito, independentemente do tipo de objeto ao qual o formulário está anexado.

  Usando o exemplo acima, embora não exista um campo interno Atribuído a: Nome para projetos, há um campo Proprietário integrado (que é preenchido automaticamente com o nome da pessoa que criou o projeto, a menos que alguém altere isso manualmente). Portanto, em seu campo personalizado Encargo, você pode usar `$$OBJCODE` como mostrado abaixo para fazer referência ao campo Proprietário quando o formulário personalizado estiver anexado a um projeto, e o campo Atribuído a: Nome quando o formulário estiver anexado a uma tarefa:

  ```
  IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})
  ```

>[!NOTE]
>
>  Se você adicionar um tipo de objeto na frente de um nome de campo, ele fará referência ao objeto pai do objeto, de modo que você não pode usar `{project}.{name}` com um projeto, mas pode usá-lo com uma tarefa.


Para obter mais informações sobre variáveis como `$$OBJCODE`, consulte [Visão geral das variáveis de filtro curinga](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

### Cuidado ao excluir um tipo de objeto de um formulário personalizado

É possível excluir um tipo de objeto em um formulário personalizado a qualquer momento, mas isso deve ser feito com cuidado. Se os usuários já tiverem anexado o formulário personalizado a objetos do tipo que você deseja excluir e adicionado dados a ele, esses dados serão excluídos permanentemente quando você excluir esse tipo de objeto no formulário.

Além disso, não há um sistema de notificação para alertar as pessoas que usam o formulário personalizado de que ele foi excluído.

Para obter mais informações, consulte [Excluir um campo ou widget personalizado do sistema](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
