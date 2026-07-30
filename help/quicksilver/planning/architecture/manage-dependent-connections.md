---
title: Gerenciar Conexões Dependentes
description: Como um gerenciador de espaço de trabalho, você pode definir conexões dependentes ao criar campos de conexão entre tipos de registro no Adobe Workfront Planning. Ao adicionar campos conectados, você pode ativar uma configuração que indica que os valores do tipo de registro conectado dependem dos valores do tipo de registro de origem (aquele em que você está adicionando a conexão), sempre que ambos os campos aparecerem juntos em um terceiro tipo de registro.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 0a4b902b2ac586b2a893dea29abb90299bee1ec3
workflow-type: tm+mt
source-wordcount: '1332'
ht-degree: 1%

---


# Gerenciar conexões dependentes

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Após o lançamento para Pré-visualização, os mesmos recursos também estarão disponíveis mensalmente no ambiente de Produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Como um gerenciador de espaço de trabalho, você pode definir conexões dependentes ao criar campos de conexão entre tipos de registro no Adobe Workfront Planning.

Ao adicionar campos conectados, você pode ativar uma configuração que indica que os valores do tipo de registro conectado dependem dos valores do tipo de registro de origem (aquele em que você está adicionando a conexão), sempre que ambos os campos aparecerem juntos em um terceiro tipo de registro.

Por exemplo, você pode querer garantir que um campo Região mostre apenas valores vinculados à Geografia selecionada. Isso é configurado diretamente na configuração do campo de conexão: ao adicionar uma conexão de um tipo de registro Geográfico a um tipo de registro dependente (como Região), uma nova configuração permite que os gerentes de espaço de trabalho marquem-na como dependente do tipo de registro Geográfico, usando os relacionamentos já estabelecidos entre esses tipos de registro.

Uma vez configurado, qualquer tipo de registro que referencie ambos os campos (como uma Campanha) verá o efeito imediatamente: selecionar um valor Geográfico restringe o seletor de Região somente às Regiões realmente vinculadas a essa Geografia. Isso reforça a estrutura de registros automaticamente, eliminando combinações incompatíveis e reduzindo a limpeza manual.

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr> 
<tr> 
   <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<p>Para conectar tipos de registro do mesmo espaço de trabalho: </p>
<ul> 
<li><p>Qualquer pacote do Workfront ou Workflow com qualquer pacote do Planning</p></li>
<p>Ou</p>
<li><p>Qualquer pacote do Planning quando adquirido como um produto independente</p></li>
</ul>

<p>Para conectar tipos de registro de espaços de trabalho diferentes:</p>

<ul>

<li><p>Qualquer fluxo de trabalho e um pacote do Planning Prime ou Ultimate</p></li>
<p>Ou</p>
<li><p>Qualquer pacote do Planning Prime ou Ultimate quando adquirido como um produto independente</p></li>
</ul>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront. </p> 
   </td> 
<tr> 
<td> 
   <p> Produtos adicionais</p> </td> 
   <td> 
   <p> Além do Adobe Workfront, você deve ter o seguinte, se quiser conectar tipos de registro a objetos dos seguintes aplicativos:</p>
   <ul><li><p>Uma licença do Adobe Experience Manager Assets e uma integração entre o AEM Assets e o Workfront para conectar o AEM Assets aos tipos de registro do Planning.</p>
   <p>Para obter informações, consulte <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront para Experience Manager Assets e Assets Essentials: índice do artigo</a>. </p></li>
   <li><p> Uma licença da Adobe GenStudio for Performance Marketing para conectar tipos de registro a objetos e marcas da GenStudio</p>
   <p>Para obter informações, consulte <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started">Introdução ao Adobe GenStudio for Performance Marketing</a>.</p></li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Padrão</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões em um espaço de trabalho</p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Sent a slack message to Norayr, Predator, Snowstorm, Armine for info for this section: 
-->

## Considerações para campos conectados dependentes


* Os campos conectados dependentes só podem ser configurados entre tipos de registro que tenham uma relação de campo de conexão estabelecida. Não é possível definir a lógica de dependência entre tipos de registro não relacionados.

* Você pode ter um campo conectado dependente entre tipos de registro em espaços de trabalho separados.

* Você não pode ter um campo conectado dependente entre os tipos de registro do Planning e os tipos de objeto do Workfront ou do AEM.

* A configuração de dependência é definida uma conexão de cada vez, dentro da própria configuração do campo de conexão, em vez de como uma regra global.

* O comportamento de filtragem entre os dois registros conectados só é ativado quando os campos de origem e dependente estão presentes juntos em um terceiro tipo de registro. A dependência não tem efeito se apenas um dos dois campos for exibido em um tipo de registro.

* O seletor de campos dependentes está limitado a valores já vinculados ao valor de origem selecionado no nível de registro; ele não pode mostrar ou sugerir valores desvinculados.

* Se o valor do campo de origem for alterado, o campo dependente será automaticamente limpo, em vez de ser deixado em um estado inválido, evitando que combinações incompatíveis persistam.

  Você recebe uma mensagem em linha ou em caixa de informações explicando por que o campo dependente foi limpo.

* Cada campo dependente pode ter até 3 campos de controle direto.

* Os níveis de dependência são limitados a 6 conexões. Isso significa que até 7 tipos de registro podem ser conectados.

* Para que a cadeia de dependências funcione, todos os campos dependentes devem existir no mesmo tipo de registro ao mesmo tempo.

## Criar uma conexão dependente

1. Como um gerenciador de espaço de trabalho, vá para um tipo de registro no Workfront Planning e abra-o na exibição de tabela.
1. Clique no ícone **+** no canto superior direito da exibição de tabela para adicionar um novo campo.
1. Clique em **Nova conexão** e comece a adicionar uma nova conexão para um segundo tipo de registro.

   >[!TIP]
   >
   >Você pode criar uma conexão dependente somente entre dois tipos de registro do Planning. Não é possível criar conexões dependentes entre tipos de registro e objetos do Workfront ou AEM.
1. Na seção **Configurações de conexão**, ative **Tornar esta conexão dependente**.

   >[!TIP]
   >
   >Ativar a configuração **Tornar esta conexão dependente** ativa automaticamente o **Criar um campo correspondente no tipo de registro vinculado**. Há um limite de 500 campos por tipo de registro.

   ![Nova guia de conexão com conexão dependente habilitada](assets/dependent-connection-enabled-setting.png)

1. Continue configurando a conexão, conforme descrito no artigo [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md).
1. Clique em **Salvar**.

   As seguintes situações ocorrem:

   * A conexão entre os dois tipos de registro é criada e seus valores dependerão uns dos outros quando exibidos juntos no mesmo tipo de registro.
   * Um campo correspondente que exibe o primeiro tipo de registro é criado para o segundo tipo de registro.
   * Quando ambos os tipos de registro estão conectados a um terceiro tipo de registro, os valores exibidos como opções para o segundo campo de registro conectado são aqueles que estão conectados ao primeiro registro. Os valores exibidos como opções para o primeiro tipo de registro são aqueles conectados ao segundo tipo de registro.

     Para obter informações, consulte a seção [Exemplo de tipos de registros conectados dependentes](#example-of-dependent-connected-record-types) neste artigo.
   * Há uma indicação no cabeçalho da coluna dos campos de registro conectados que explica que o campo está em um relacionamento de conexão dependente.

     ![Dica de ferramenta do ícone dependente no cabeçalho da coluna](assets/dependent-icon-tooltip-in-column-header.png)

1. (Opcional e recomendado) Vá para um terceiro tipo de registro e adicione o primeiro e o segundo tipo de registro como campos de registro conectados.

   ![Indicador de campo conectado dependente em um terceiro tipo de registro](assets/dependent-connected-field-indicator-on-a-third-record-type.png)

## Exemplo de tipos de registros conectados dependentes

Esta seção fornece um exemplo simples de como você pode configurar tipos de registros dependentes e como eles funcionam para um terceiro tipo de registro.

1. Em um espaço de trabalho que você pode gerenciar, crie os seguintes tipos de registro:

   * Campaign
   * Países
   * Continentes

1. No tipo de registro **Países**, adicione os seguintes registros:

   * França
   * Estados Unidos
   * Japão
1. No tipo de registro **Continentes**, adicione os seguintes registros:

   * Europa
   * América
   * Ásia

1. No tipo de registro **Países**, crie um campo dependente conectado para **Continentes**.

   Isso adiciona os seguintes campos de registro conectados:

   * O campo de registro conectado **Países** para o tipo de registro **Continentes**.
   * O campo de registro conectado **Continentes** para o tipo de registro **Países**.

1. Siga um destes procedimentos:

   * Na exibição de tabela do tipo de registro **Países**, adicione os seguintes valores para o campo de registro conectado Continentes:

     * Europa para a França
     * América para os Estados Unidos
     * Ásia para o Japão
   * Na exibição de tabela do tipo de registro **Continentes**, adicione os seguintes valores para o campo de registro conectado **Países**:

     * França para a Europa
     * Estados Unidos da América
     * Japão para Ásia
1. Adicione os campos conectados **Países** e **Continentes** à exibição de tabela do tipo de registro **Campanha**.
1. Selecione **Japão** para o campo **Países** no tipo de registro **Campanha**. Observe que o único valor disponível para o campo conectado **Continentes** na campanha é **Ásia**.

   Ou

   Selecione **Europa** para o campo **Continentes** no tipo de registro de Campanha.

   Observe que o único valor disponível para o campo conectado **Países** na campanha é **França**.



