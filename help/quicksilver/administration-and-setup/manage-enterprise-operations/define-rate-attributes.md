---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Definir atributos de taxa
description: Os atributos de taxa ampliam a funcionalidade do cartão de taxa e das taxas do Adobe Workfront, permitindo a adição de dimensões adicionais às taxas, além da função de trabalho. Em seguida, o Workfront pode selecionar automaticamente a taxa correta para as atribuições, garantindo a precisão financeira e a consistência entre projetos.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d570ef6a-935f-4dd0-9c54-a480163ec9d8
source-git-commit: 3a194bc2b2707c7b7e1cd5edffc3dd5ab43e91b3
workflow-type: tm+mt
source-wordcount: '1378'
ht-degree: 2%

---

# Definir atributos de taxa

{{highlighted-preview-article-level}}

Os atributos de taxa ampliam a funcionalidade do cartão de taxa e das taxas do Adobe Workfront, permitindo a adição de dimensões adicionais às taxas, além da função de trabalho. Isso é essencial para agências e empresas em que as taxas variam não apenas por função de trabalho, mas também por fatores como agência, local, marca, centro de custo ou outros.
Ao combinar esses atributos, o Workfront pode selecionar automaticamente a taxa correta para as atribuições, garantindo a precisão financeira e a consistência entre os projetos.

>[!IMPORTANT]
>
>Os atributos de taxa são uma configuração básica única.

Depois que os atributos forem ativados e aplicados aos cartões de taxa e às taxas, alterá-los posteriormente poderá comprometer a integridade dos dados em toda a configuração financeira.

## Visão geral dos atributos de taxa

Os atributos de taxa são considerados uma configuração única porque:

* Os atributos se tornam parte do modelo de dados financeiros quando são ativados.
* Taxas, atribuições, valores planejados e valores reais dependem dos valores de atributo escolhidos.
* Alterar os atributos posteriormente (renomear, remover ou reordenar) pode causar:

   * Perda de vínculo entre taxas e atributos
   * Taxas inválidas ou &quot;órfãs&quot;
   * Alinhamento incorreto no faturamento e nos relatórios

Por esses motivos, os atributos devem ser projetados com cuidado durante a implementação inicial do Workfront e deixados inalterados posteriormente.

### Objetos usados como atributos de taxa

Atualmente, o Workfront oferece suporte a três objetos do sistema que podem ser usados como atributos de taxa:

* **Grupo**: Geralmente renomeado como _Agência_ ou _Unidade de Negócios_.
* **Empresa**: pode representar a _Marca_, _Cliente_ ou _Cliente_.
* **Local**: Geralmente usado como _Mercado_, _Região_ ou _Escritório_.

  A localização é definida hierarquicamente em até 3 níveis. (Exemplo: se você definir &quot;Localização&quot; como Los Angeles, Califórnia e EUA também serão usados em correspondências de taxa.)

Cada objeto pode ser renomeado para corresponder à terminologia da sua organização ao configurar seus atributos.
Por exemplo:

* Rótulo &quot;Agency&quot; = referência do objeto de grupo
* Rótulo &quot;Centro de custos&quot; = Referência do objeto de subgrupo
* Rótulo &quot;Location&quot; = Referência do objeto Location

Isso permite que a configuração espelhe sua estrutura comercial, mantendo a integridade do modelo de dados da Workfront.

### Observações sobre atributos de taxa no Workfront

* O Workfront oferece suporte a até 5 níveis de atributos. O sistema sempre segue a hierarquia de atributo, selecionando a correspondência mais específica disponível.

   * 0 = taxa de base genérica
   * 1 - 5 = taxas progressivamente mais específicas

* É possível renomear atributos para refletir sua empresa (Agência, Marca, Mercado, Centro de custos etc.).
* A configuração é feita apenas uma vez: alterar os atributos posteriormente corre o risco de quebrar a integridade dos dados financeiros.
* Os atributos que não são referenciados em nenhum lugar do sistema podem ser excluídos com segurança.

  No entanto, se um atributo já estiver em uso (referenciado em cartões de taxa, perfis de usuário, recursos ou atribuições), a exclusão será bloqueada para proteger a integridade dos dados. Nesses casos, tentar remover o atributo, especialmente por meio de uma chamada de API, resultará em um erro.

* Testar antes da ativação: crie um cartão de taxa piloto e valide se as taxas corretas foram resolvidas nas atribuições.
* Documente sua configuração: compartilhe a configuração de atributos de taxa com suas equipes para que elas entendam como as taxas funcionam.

### Onde os atributos de taxa podem ser aplicados

Os atributos de taxa são suportados em todas as áreas em que existem taxas no Workfront:

* Cartões de taxa: Defina taxas por função de cargo mais atributos.
* Sobreposições no nível do projeto: aplique atributos ao substituir taxas no nível do projeto.
* Funções de trabalho (em Configuração): Defina as taxas de funções de trabalho padrão com atributos.
* Usuários (perfis de usuários): Designa atributos nativos a usuários individuais, de modo que as designações sejam resolvidas automaticamente com as taxas corretas.

<!--
BULLET POINT Staffing plan resources
BULLET POINT Non-labor resources: Attributes can also be defined on resources such as equipment or services.-->

<!--Non-labor resource categories and -->As funções de trabalho não oferecem suporte a atributos de taxa diretamente no nível do objeto. Eles são conectados a atributos de taxa por meio das taxas definidas neles.

Quando você puder criar atribuições de espaço reservado vinculadas aos valores de atributo corretos, suas taxas serão preenchidas adequadamente.

* Para funções de trabalho, quando você substitui o espaço reservado posteriormente por um usuário real, o sistema redefine automaticamente os atributos da atribuição para aqueles definidos no perfil desse usuário. Nesse ponto, os atributos não podem mais ser editados no nível de atribuição. Eles são herdados do usuário para preservar a consistência e evitar o desalinhamento entre os atributos do usuário e as taxas aplicadas.

<!-- BULLET POINT For non-labor resource categories, placeholder assignments can be used similarly: You assign the category through a placeholder that carries the required attributes. Once the actual non-labor resource is substituted, the attributes are automatically pulled from the resource's profile. Just like with users, these attributes cannot be overridden manually at the assignment level, ensuring financial data integrity and preventing accidental mismatches between resources and their designated attributes.-->

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacote</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licença</td> 
   <td><p>[!UICONTROL Padrão]</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar atributos de taxa

Cada atributo tem um conjunto de opções configuráveis, incluindo propriedades e filtros gerais.
Os filtros controlam como os valores de atributo são sugeridos e validados ao definir as taxas. Elas são essenciais para manter as seleções de atributos consistentes, orientar os usuários em relação às opções válidas e evitar combinações inválidas.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Atributos de taxa**.
1. Clique em um ícone de sinal de mais no diagrama para adicionar um atributo.

   >[!NOTE]
   >
   >É possível ter até cinco atributos no diagrama. A ordem de cima para baixo define a hierarquia de como os atributos são aplicados. Clique no ícone **Girar** ![Ícone Girar](assets/rotate-attribute-view-icon.png) para exibir o diagrama da esquerda para a direita. Você também pode ampliar ou reduzir e ajustar o diagrama à tela.

1. Selecione um atributo para abrir o painel de configuração à direita da tela.

   ![Configurar atributos de taxa](assets/configure-rate-attributes.png)

1. Renomeie os objetos (Grupo, Empresa, Local) nos termos necessários para sua empresa (como Agência, Local, Centro de custos).
1. Clique em **Salvar** em cada atributo para salvar sua convenção de nomenclatura.

   Os nomes desses atributos serão exibidos em todos os cartões de taxa e taxas no sistema.

1. Defina as propriedades de cada atributo no painel de configuração:

   * **Obrigatório**: Selecione se o atributo é um campo obrigatório em taxas.
   * **A ser usado no cálculo de receita**: inclui este atributo nos cálculos de taxa de cobrança.
   * **A ser usado no cálculo de custo**: inclui este atributo nos cálculos de taxa de custo.

     >[!NOTE]
     >
     >Pelo menos uma das opções de cálculo deve ser selecionada para que o atributo funcione em cálculos financeiros.

   * (Opcional) **Hierárquico**: permite que o atributo respeite relações pai-filho, como Cidade > Estado > País.

     Essa propriedade está disponível somente para o objeto Location.

### Definir filtros para os atributos

Dois tipos de filtros estão disponíveis para os atributos:

* Os Filtros de sugestão restringem a lista de opções disponíveis com base na lógica do sistema ou em seleções de atributos anteriores. Eles tornam os menus suspensos sensíveis ao contexto e fáceis de usar.

  Exemplo: Agência > Local > Centro de Custo

  Nesta configuração, o atributo Centro de Custo deve ter um Filtro de Sugestão que faça referência à Agência e ao Local.

  Ao adicionar uma taxa, se você selecionar Agência = &quot;Estrela&quot; pela primeira vez, a lista suspensa Localização sugerirá apenas as Localizações que pertencem a &quot;Estrela&quot;.

  Se você selecionar Local = Chicago na taxa, a lista suspensa Centro de custo sugerirá apenas Centros de custo vinculados a &quot;Estrela&quot; e Chicago.

* Os Filtros de relacionamento estabelecem a cadeia de dependência entre atributos. Eles garantem que o sistema entenda como os atributos se relacionam entre si e impõem dependências válidas.

  Exemplo: Agência > Local > Centro de Custo

  Nesta configuração, o atributo Agência deve ter um Filtro de Relacionamento que o vincule a Locais e Centros de Custo válidos.

Os filtros devem ser sempre configurados em ambas as direções. Se o Atributo A tiver um Filtro de relacionamento com o Atributo B, o Atributo B deverá ter um Filtro de sugestão de volta para o Atributo A. Isso garante a integridade dos dados e uma experiência limpa para o usuário.

1. Selecione opções para definir os Filtros de Sugestão e os Filtros de Relacionamento para o atributo no painel de configuração:

   * **Tipo de filtro**:

      * Um filtro **Standard** aplica uma condição universal ao objeto de atributo. Por exemplo, Local > Está ativo = Verdadeiro (somente os Locais ativos serão exibidos).

        O filtro Padrão é sempre aplicado, independentemente de outros atributos serem selecionados.

      * Um filtro **Atributo** vincula um atributo a outro na cadeia. Por exemplo, Local > Referência = Agência (somente os Locais vinculados à Agência selecionada serão mostrados).

        O filtro Atributo só é aplicado se o atributo referenciado tiver um valor. Por exemplo, se a opção Agência for selecionada, somente os Locais válidos serão sugeridos. Se Agência estiver em branco, todas as Localizações serão exibidas (mas ainda podem ser limitadas pelos filtros Padrão aplicados à Localização).

   * **Campo**: o campo direto do objeto de atributo, como ID de Local ou Sinalizador Ativo.
   * **Operador**: essas opções dependem do tipo de Campo selecionado. Os exemplos incluem Igual a, Diferente de, Está em branco, Verdadeiro/Falso.
   * (Somente tipo de filtro padrão) **Value**: por exemplo, Is Ative = True.
   * (Somente tipo de filtro de atributo) **Reference**: o atributo do qual esse filtro depende, como Agency.
   * (Somente tipo de filtro de atributo) **Campo de Referência**: o campo no atributo referenciado que deve corresponder, como ID da Agência.

1. Clique em **Salvar** em cada atributo para salvar as propriedades e os filtros.
