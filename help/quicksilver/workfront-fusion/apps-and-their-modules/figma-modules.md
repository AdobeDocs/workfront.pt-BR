---
filename: figma-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos do Figma
description: Com os  [!DNL Adobe Workfront Fusion] módulos Figma, você pode recuperar listas de comentários, arquivos, versões de arquivos ou projetos. Você também pode postar um comentário ou fazer uma chamada para a API do Figma.
author: Becky
feature: Workfront Fusion
exl-id: d88db592-32d4-4765-952f-9ffb58cf1720
source-git-commit: 2e91e9a4c691430f3c98e3cbddb30706ea57f84a
workflow-type: tm+mt
source-wordcount: '2331'
ht-degree: 0%

---

# [!DNL Figma] Módulos

Com os módulos [!DNL Adobe Workfront Fusion] [!DNL Figma], você pode recuperar listas de comentários, arquivos, versões de arquivos ou projetos. Você também pode postar um comentário ou chamar a API [!DNL Figma].

Se você precisar de instruções sobre como criar um cenário, consulte [Criar um cenário](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obter informações sobre módulos, consulte [Módulos em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plano*</td>
      <td>
        <p>[!UICONTROL Pro] ou superior</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licença*</td>
      <td>
        <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td>
      <td>
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Produto</td>
      <td>
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td>
    </tr>
  </tbody>
</table>


Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Para usar módulos [!DNL Figma], você deve ter uma conta [!DNL Figma].

## Informações da API do Figma

O conector Figma usa o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL base</td> 
   <td> https://api.figma.com/v1</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Versão da API</td> 
   <td> v1 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tag da API</td> 
   <td>v1.8.25</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Figma] módulos e seus campos

Ao configurar módulos do [!DNL Figma], o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL Figma] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Comentários](#comments)

* [Projetos e arquivos](#projects-and-files)

* [Componentes e estilos](#components-and-styles)

* [Outro](#other)


### Comentários

* [Excluir um comentário](#delete-a-comment)

* [Listar comentários](#list-comments)

* [Postar um comentário](#post-a-comment)


#### [!UICONTROL Excluir um comentário]

Este módulo de ação exclui um único comentário de um arquivo.

<table style="table-layout:auto"> 
  <col/>
  <col />
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Figma] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas.</a></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Arquivo]</td>
      <td>Insira ou mapeie a ID do arquivo do qual você deseja adicionar um comentário para exclusão. </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Comentário]</td>
      <td>Insira o texto do comentário que deseja excluir.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Listar comentários]

Este módulo de pesquisa lista todos os comentários anexados a um único arquivo no [!DNL Figma].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Figma] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Arquivo]</td>
      <td>
        <p>Insira ou mapeie a ID do arquivo para o qual deseja recuperar comentários. </p>
        <ul>
          <li>
            <p>Se você não souber a identificação, clique em <b>[!UICONTROL Localizar Arquivos]</b>, insira ou mapeie a identificação do projeto ao qual o arquivo está associado e selecione o arquivo.</p>
          </li>
          <li>
            <p>Se você não souber a ID do projeto, clique em <b>[!UICONTROL Localizar Projetos]</b>, insira ou mapeie a ID da equipe que possui o projeto ao qual o arquivo está associado, selecione o projeto e selecione o arquivo.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]</td>
      <td>Insira ou mapeie o número máximo de comentários que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL Postar um comentário]

Este módulo de ação publica um comentário em um arquivo Figma.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Figma] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas.</a></p>
    </tr>
    <tr>
      <td  role="rowheader">[!UICONTROL ID de Arquivo]</td>
      <td>
        <p>Insira ou mapeie a ID do arquivo no qual você deseja postar um comentário. </p>
        <ul>
          <li>
            <p>Se você não souber a identificação do arquivo, clique em <b>[!UICONTROL Localizar Arquivos]</b>, insira ou mapeie a identificação do projeto ao qual o arquivo está associado e selecione o arquivo.</p>
          </li>
          <li>
            <p>Se você estiver tentando encontrar a ID do arquivo e não souber a ID do projeto, clique em <b>[!UICONTROL Localizar Projetos]</b> e insira ou mapeie a ID da equipe proprietária do projeto ao qual o arquivo está associado. Selecione o projeto e, em seguida, o arquivo.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Comentário]</td>
      <td>Insira o texto do comentário.</td>
    </tr>
  </tbody>
</table>


### Projetos e arquivos

* [Obter um arquivo ou uma imagem](#get-a-file-or-image)

* [Listar histórico de versão do arquivo](#list-file-version-history)

* [Listar arquivos de projeto](#list-project-files)

* [Listar projetos](#list-projects)


#### [!UICONTROL Obter um arquivo ou uma imagem]

Este módulo de ação recupera um único arquivo ou imagem de uma biblioteca Figma

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Figma] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de objeto]</td>
      <td>
        <p>Selecione o tipo de objeto que deseja recuperar.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Arquivo]</b>
            </p>
            <p>O módulo retorna o documento referenciado pela [!UICONTROL Chave] como um objeto JSON. A chave do arquivo pode ser analisada de qualquer URL do arquivo Figma.</p>
            <p>Para campos, consulte <a href="#Get2" class="MCXref xref" >[!UICONTROL Obter um arquivo ou imagem: Arquivo]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL nós de Arquivo]</b>
            </p>
            <p>Retorna os nós aos quais as IDs fazem referência como um objeto JSON. Os nós são recuperados do arquivo [!DNL Figma] ao qual a [!UICONTROL Key] faz referência.</p>
            <p>Para campos, consulte <a href="#Get3" class="MCXref xref" >[!UICONTROL Obter um arquivo ou imagem: nós de arquivo]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Imagem]</b>
            </p>
            <p>O módulo renderiza imagens de um arquivo.</p>
            <p>Para campos, consulte <a href="#Get4" class="MCXref xref" >[!UICONTROL Obter um arquivo ou imagem: Imagem]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Preenchimentos de imagem]</b>
            </p>
            <p>O módulo retorna links de download para todas as imagens presentes em preenchimentos de imagem em um documento. Os preenchimentos de imagem são como [!DNL Figma] representa quaisquer imagens fornecidas pelo usuário. Quando você arrasta uma imagem para [!DNL Figma], [!DNL Figma] cria um retângulo com um único preenchimento que representa a imagem, e o usuário pode transformar o retângulo (e as propriedades no preenchimento).</p>
            <p>Para campos, consulte <a href="#Get5" class="MCXref xref" >[!UICONTROL Obter um arquivo ou imagem: Preenchimentos de imagem]</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL Obter um arquivo ou uma imagem: Arquivo]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Chave do arquivo]</td>
      <td>Selecione o arquivo do qual deseja retornar JSON.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Versão]</td>
      <td>Insira ou mapeie a versão do arquivo que o módulo deve retornar. Para o módulo atual, deixe este campo em branco.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL IDs de Nó]</td>
      <td>
        <p>Para retornar apenas um subconjunto do documento, insira os nós que você deseja que o módulo retorne. O módulo retorna os nós listados, seus filhos e qualquer item entre o nó raiz e os nós listados.</p>
        <p>Para cada nó que você deseja retornar, clique em <b>[!UICONTROL Add]</b> e insira o texto do nó.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Profundidade]</td>
      <td>
        <p>Insira ou mapeie um número inteiro que represente a profundidade máxima na árvore de documentos para a qual você deseja retornar resultados. </p>
        <div class="example"><span class="autonumber"><span><b>Exemplo: </b></span></span>
          <ul>
            <li>
              <p>Para retornar somente páginas, digite <code>1</code>.</p>
            </li>
            <li>
              <p>Para retornar páginas e objetos de nível superior, digite <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>Para retornar todos os nós, deixe este campo em branco.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Geometria]</td>
      <td>Para retornar dados vetoriais, digite <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dados do plug-in]</td>
      <td>Uma lista separada por vírgulas de IDs de plug-in e/ou a sequência "[!UICONTROL shared]". Quaisquer dados presentes no documento escrito por esses plug-ins serão incluídos no resultado nas propriedades <code>pluginData</code> e <code>sharedPluginData</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dados de ramificação]</td>
      <td>Habilite esta opção para retornar os metadados da ramificação para o arquivo solicitado. Se o arquivo for uma ramificação, a chave do arquivo principal será incluída na resposta retornada. Se o arquivo tiver ramificações, os metadados serão incluídos na resposta retornada. Padrão: <code>false</code>.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Obter um arquivo ou uma imagem: nós de arquivo]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Chave do arquivo]</td>
      <td>Selecione o arquivo do qual deseja retornar JSON.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL IDs de Nó]</td>
      <td>
        <p>Insira os nós que você deseja que o módulo retorne e converta</p>
        <p>Para cada nó que você deseja retornar, clique em <b>[!UICONTROL Add]</b> e insira o texto do nó.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Versão]</td>
      <td>Insira ou mapeie a versão do arquivo que o módulo deve retornar. Para o módulo atual, deixe este campo em branco.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Profundidade]</td>
      <td>
        <p>Insira ou mapeie um número inteiro que represente a profundidade máxima na árvore de documentos para a qual você deseja retornar resultados. </p>
        <div class="example"><span class="autonumber"><span><b>Exemplo: </b></span></span>
          <ul>
            <li>
              <p>Para retornar somente páginas, digite <code>1</code>.</p>
            </li>
            <li>
              <p>Para retornar páginas e objetos de nível superior, digite <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>Para retornar todos os nós, deixe este campo em branco.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Geometria]</td>
      <td>Para retornar dados vetoriais, digite <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dados do plug-in]</td>
      <td>Uma lista separada por vírgulas de IDs de plug-in e/ou a sequência "compartilhada". Quaisquer dados presentes no documento escrito por esses plug-ins serão incluídos no resultado nas propriedades pluginData e sharedPluginData.</td>
    </tr>
  </tbody>
</table>


##### Obter um arquivo ou imagem: Imagem

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Chave do arquivo]</td>
      <td>Selecione o arquivo do qual deseja retornar JSON.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL IDs de Nó]</td>
      <td>
        <p>Insira os nós que você deseja que o módulo renderize.</p>
        <p>Para cada nó que você deseja renderizar, clique em <b>[!UICONTROL Add]</b> e insira o texto do nó.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Escala]</td>
      <td>Para dimensionar a imagem, insira ou mapeie o fator de dimensionamento. Este número deve estar entre 0,01 e 4.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Formatar]</td>
      <td>
        <p>Selecione o formato para a saída da imagem.</p>
        <ul>
          <li>
            <p>JPG</p>
          </li>
          <li>
            <p>Imagem PNG</p>
          </li>
          <li>
            <p>SVG</p>
          </li>
          <li>
            <p>PDF</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SVG - Incluir ID]</td>
      <td>Habilite esta opção para incluir atributos de ID para todos os elementos de SVG. Padrão: [!UICONTROL false].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SVG - Simplificar Traço]</td>
      <td>Ative essa opção para simplificar traçados internos/externos e, se possível, use o atributo de traçado em vez de &lt;mask&gt;. Padrão: [!UICONTROL true].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Usar limites absolutos]</td>
      <td>Habilite essa opção para usar as dimensões completas do nó, independentemente de ele estar ou não cortado ou do espaço ao redor estar vazio. Use isso para exportar nós de texto sem cortar. Padrão: [!UICONTROL false].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Versão]</td>
      <td>Insira ou mapeie a versão do arquivo que o módulo deve retornar. Para o módulo atual, deixe este campo em branco.</td>
    </tr>
  </tbody>
</table>

##### Obter um arquivo ou imagem: preenchimentos de imagem

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Chave do arquivo]</td>
      <td>Selecione o arquivo do qual deseja retornar JSON.</td>
    </tr>
  </tbody>
</table>

### [!UICONTROL Listar histórico de versões de arquivos]

Este módulo de pesquisa retorna o histórico de versões de um único arquivo no [!UICONTROL Figura].
<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Figma] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas.</a></p>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Arquivo]</td>
      <td>
        <p>Insira ou mapeie a ID do arquivo para o qual você deseja recuperar o histórico de versões. </p>
        <ul>
          <li>
            <p>Se você não souber a identificação do arquivo, clique em <b>[!UICONTROL Localizar Arquivos]</b>, insira ou mapeie a identificação do projeto ao qual o arquivo está associado e selecione o arquivo.</p>
          </li>
          <li>
            <p>Se você estiver tentando encontrar a ID do arquivo e não souber a ID do projeto, clique em <b>[!UICONTROL Localizar Projetos]</b> e insira ou mapeie a ID da equipe proprietária do projeto ao qual o arquivo está associado. Selecione o projeto e, em seguida, o arquivo.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]</td>
      <td>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Listar arquivos de projeto]

Este módulo de pesquisa retorna uma lista de todos os arquivos no projeto especificado.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Figma] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Arquivo]</td>
      <td>
        <p>Insira ou mapeie a ID do projeto para o qual você deseja recuperar os arquivos. </p>
        <ul>
          <li>
            <p>Se você não souber a identificação dos projetos, clique em <b>[!UICONTROL Localizar Projetos]</b>, insira ou mapeie a identificação da equipe à qual o projeto está associado e selecione o projeto.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]</td>
      <td>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Listar projetos]

Este módulo de pesquisa retorna uma lista de todos os projetos dentro da equipe especificada.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Figma] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID da Equipe]</td>
      <td>Insira ou mapeie a ID do projeto do qual você deseja recuperar os arquivos. A ID da equipe pode ser encontrada no URL da página da equipe no Figma</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]</td>
      <td>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</td>
    </tr>
  </tbody>
</table>


### Componentes e estilos

#### [!UICONTROL Obter um estilo ou componente]

Este módulo de ação recupera um único estilo ou componente, ou um conjunto de estilos ou componentes.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Figma] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas.</a></p>
    </tr>
    <tr>
      <td role="rowheader">&lt;[!UICONTROL Objeto&gt; chave]</td>
      <td>Informe a chave (identificador exclusivo) do objeto que deseja recuperar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID da Equipe]</td>
      <td>Insira ou mapeie a ID da equipe à qual o registro ou os registros estão associados.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tamanho da Página]</td>
      <td>Insira ou mapeie o número ou os resultados a serem retornados por página. Padrão: 30.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Depois]</td>
      <td>
        <p>Insira ou mapeie o número do resultado após o qual começar a recuperar os resultados. Isso pode ser combinado com o campo [!UICONTROL Tamanho da página] para paginar resultados.</p>
        <p>Esse valor não corresponde às IDs de objeto.</p>
        <p>Este campo não pode ser usado em combinação com o campo [!UICONTROL Antes].</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Antes]</td>
      <td>
        <p>Insira ou mapeie o número do resultado antes do qual começar a recuperar os resultados. Isso pode ser combinado com o campo [!UICONTROL Tamanho da página] para paginar resultados.</p>
        <p>Esse valor não corresponde às IDs de objeto.</p>
        <p>Este campo não pode ser usado em combinação com o campo [!UICONTROL After].</p>
      </td>
    </tr>
  </tbody>
</table>


### Outro

* [Fazer uma chamada de API](#make-an-api-call)

* [Assistir a eventos](#watch-events)


#### [!UICONTROL Fazer uma chamada de API]

Esse módulo de ação permite fazer uma chamada autenticada personalizada para a API Figma sem precisar pensar na autenticação. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pelos outros módulos do Figma.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Figma] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Insira um caminho relativo para <code>https://api.figma.com/v1/</code>.</p>
        <p>Por exemplo: <code>[!DNL files/7179110/comments]</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Método]</td>
      <td> <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cabeçalhos]</td>
      <td>
        <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão.</p>
        <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] O adiciona os cabeçalhos de autorização para você.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cadeia de Consulta]</td>
      <td>
        <p>Adicione a consulta da chamada à API na forma de um objeto JSON padrão.</p>
        <p>Por exemplo: <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Corpo]</td>
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar instruções condicionais como <code>if</code> em seu JSON, coloque as aspas fora da instrução condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Assistir a eventos]

Este módulo de acionamento inicia um cenário quando um dos seguintes eventos ocorre para uma equipe específica no seu espaço de equipe [!DNL Figma]

* Atualização de arquivo

* Atualização da versão do arquivo

* Arquivo excluir

* Publicação da biblioteca

* Comentário do arquivo

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>
        <p>Selecione o webhook que o módulo observa.</p>
        <p>Para adicionar um novo webhook:</p>
        <ol>
          <li value="1">
            <p>Clique em <b>[!UICONTROL Adicionar]</b> ao lado do campo [!UICONTROL Webhook].</p>
          </li>
          <li value="2">
            <p>Selecione a conexão que deseja usar com este webhook. Para obter instruções sobre como conectar sua conta do [!DNL Figma] ao [!UICONTROL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!UICONTROL Adobe Workfront Fusion] - Instruções básicas.</a></p>
          </li>
          <li value="3">
            <p>Selecione o tipo de evento que você deseja que o módulo veja.</p>
          </li>
          <li value="4">
            <p>Digite a ID da equipe cujos eventos você deseja que o webhook assista.</p>
          </li>
          <li value="5">
            <p>Insira o [!UICONTROL Status] ou a [!UICONTROL Descrição] dos eventos que você deseja que o webhook assista.</p>
          </li>
          <li value="6">
            <p>Clique em <b>[!UICONTROL Salvar]</b> para salvar o webhook e retornar ao módulo.</p>
          </li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>
