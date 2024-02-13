---
title: Exemplos do campo Pesquisa externa em um formulário personalizado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Um campo Pesquisa externa em um formulário personalizado chama uma API externa e retorna valores como opções em um campo suspenso. Este artigo fornece exemplos de como usar o campo Pesquisa externa para chamar a mesma instância do Workfront ou uma API pública.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
source-git-commit: a082f010dbd78235aaad41a80d87d772ca77ff89
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 0%

---

# Exemplos do campo Pesquisa externa em um formulário personalizado

Um campo Pesquisa externa em um formulário personalizado chama uma API externa e retorna valores como opções em um campo suspenso. Os usuários que trabalham com o objeto ao qual o formulário personalizado está anexado podem selecionar uma ou mais dessas opções na lista suspensa.

Este artigo fornece exemplos de como usar o campo Pesquisa externa para chamar a mesma instância do Workfront ou uma API pública. Você também pode usar a Pesquisa externa para se comunicar com um sistema externo, como Jira, Salesforce ou ServiceNow.

Para obter mais informações sobre como adicionar um campo Pesquisa externa a um formulário personalizado e definições adicionais dos componentes de pesquisa externa, consulte [Criar um formulário com o designer de formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Configurar um campo Pesquisa externa para a mesma instância do Workfront

Você pode usar a Pesquisa externa para trazer dados da sua instância do Workfront para o formulário personalizado.

Este exemplo mostra como chamar a API do Workfront e trazer dados do campo &quot;Consulta de status&quot; existente para o campo Pesquisa externa.

1. Abra o formulário personalizado.
1. No lado esquerdo da tela, localize **Pesquisa externa** e arraste-a para uma seção na tela.
1. Insira o **Rótulo** e **Nome** para o campo.
1. Selecione o **Formato** para o campo.
1. Insira a chamada do URL da API no **URL base da API** campo.

   * Você pode adicionar $$HOST para fazer referência à mesma instância.
   * Você pode adicionar $$QUERY para filtrar os resultados com base na consulta de um campo diferente.

   **Exemplo**
   `$$HOST/attask/api/v15.0/project/search?status={DE:StatusQuery}&$$QUERY`

1. Revise o **Dependências** para os campos que esse campo de pesquisa referencia na API.

   Um campo de dependência pode ser qualquer campo personalizado ou nativo existente na página de detalhes do objeto.

   Neste exemplo, a variável `{DE:StatusQuery}` serão substituídos pelo valor do campo personalizado StatusQuery.

1. Selecione o **Método HTTP**.

   Isto será provavelmente **Obter**.

1. Insira o **Caminho JSON** para obter os resultados da sua chamada de API.

   **Exemplo**
   `$.data[*].name`

   >[!NOTE]
   >
   >**Cabeçalho** não são necessárias informações para uma chamada para a mesma instância do Workfront.

1. Clique em **Aplicar**.

   ![Configuração da chamada de API para o Workfront no formulário personalizado](assets/external-lookup-to-workfront.png)

   Quando o formulário personalizado é adicionado a um objeto do Workfront (neste exemplo, um projeto), ele é semelhante a este.

   ![Formulário personalizado com campo de pesquisa externo](assets/external-lookup-project-status-example1.png)

   ![Opções de pesquisa externa com base no status](assets/external-lookup-project-status-example2.png)

## Configurar um campo Pesquisa externa para uma API pública

Você pode usar a Pesquisa externa para chamar uma API externa pública e recuperar dados.

Este exemplo mostra como chamar uma API de países (como <https://api.first.org/data/v1/countries>) para que não seja necessário codificar todos os nomes de países nas opções suspensas.

1. Abra o formulário personalizado.
1. No lado esquerdo da tela, localize **Pesquisa externa** e arraste-a para uma seção na tela.
1. Insira o **Rótulo** e **Nome** para o campo.
1. Selecione o **Formato** para o campo.
1. Insira a chamada do URL da API no **URL base da API** campo.

   * Você pode adicionar $$QUERY para implementar a filtragem de consultas para seus usuários finais.

   **Exemplos**
Lista todos os países: <https://api.first.org/data/v1/countries>

   Permite que o usuário pesquise por qualquer país no campo suspenso: <https://api.first.org/data/v1/countries?q=$$QUERY>

   Permite que o usuário pesquise por um país em uma região: <https://api.first.org/data/v1/countries?region={DE:Region}&q=$$QUERY>

   * As regiões disponíveis são definidas em um campo personalizado separado no Workfront.
   * Quando o usuário seleciona uma região no formulário, o campo Pesquisa externa mostra apenas os países dessa região (qual país está em qual região está definida na API). O usuário também pode pesquisar por um país na região selecionada.

1. Revise o **Dependências** para os campos que esse campo de pesquisa referencia na API.

   Um campo de dependência pode ser qualquer campo personalizado ou nativo existente na página de detalhes do objeto.

   Neste exemplo, a variável `{DE:Region}` será substituído pelo valor do campo personalizado Região.

1. Selecione o **Método HTTP**.

   Isto será provavelmente **Obter**.

1. Insira o **Caminho JSON** para obter os resultados da sua chamada de API.

   Essa opção permite extrair dados do JSON retornado pelo URL da API. Ela serve como uma maneira de selecionar quais valores dentro do JSON aparecerão nas opções suspensas.

   **Exemplo**
   `$.data[*].country`

1. (Opcional) Clique em **Adicionar cabeçalho** e digite ou cole o par de valores chave necessário para autenticação com a API.

   >[!NOTE]
   >
   >Os campos de Cabeçalho não são um local seguro para armazenar credenciais, e você deve ter cuidado com o que digitar e salvar.

1. (Opcional) Selecione **Lista suspensa de seleção múltipla** para permitir que o usuário selecione mais de um valor na lista suspensa.

1. Clique em **Aplicar**.

   ![Configuração da chamada da API para a API pública em um formulário personalizado](assets/external-lookup-to-api-for-countries.png)

   Quando o formulário personalizado é adicionado a um objeto do Workfront (neste exemplo, um projeto), ele é semelhante a este.

   ![Formulário personalizado com campo de pesquisa externo](assets/external-lookup-countries-example1.png)

   ![Opções de pesquisa externa para um país com base na região](assets/external-lookup-countries-example2.png)

