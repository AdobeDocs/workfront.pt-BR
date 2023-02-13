---
filename: powerbi-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Power BI
description: O Adobe Workfront Fusion exige uma licença do Adobe Workfront Fusion além de uma licença da Adobe Workfront.
author: Becky
hidefromtoc: true
exl-id: 01405f5f-6821-4c38-b34c-373922f63004
source-git-commit: 3b5f203ead1e7b8ab83bec58adb25dd03c520787
workflow-type: tm+mt
source-wordcount: '2352'
ht-degree: 0%

---

# [!DNL Power BI] Módulos

[!DNL Power BI] é um aplicativo que permite visualizar e apresentar dados às suas partes interessadas. Ele pode obter dados de várias fontes.

>[!NOTE]
>
>[!DNL Workfront Fusion] não é uma fonte de dados. Ao [!DNL Workfront Fusion] O pode criar e usar fontes de dados, ele não armazena seus dados.


## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!DNL Pro] ou superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!DNL Plan], [!DNL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td> 
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

&#42;&#42;Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!DNL Power BI] módulos e seus campos

Ao configurar [!DNL Power BI], [!DNL Workfront Fusion] exibe os campos listados abaixo. Juntamente com esses campos, campos adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Painéis

#### [!UICONTROL Painéis de lista]

Este módulo de pesquisa recupera uma lista de painéis.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do grupo]  </td>
      <td>
        <p>Selecione ou mapeie a ID do Grupo que possui os painéis que deseja listar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]  </td>
      <td>
        <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Listar blocos do painel]

Esse módulo de pesquisa recupera uma lista de blocos de painel.

<table>
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Inserir uma ID de painel]</td>
    <td>
      <p>Selecione ou mapeie a opção para escolher o painel cujos blocos deseja listar.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL ID do painel]</td>
    <td>
      <p>Insira ou mapeie a ID do painel que contém os blocos que você deseja listar.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL ID do grupo]  </td>
    <td>Selecione ou mapeie a ID do Grupo que possui os painéis que contém os blocos que você deseja listar.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Limite]  </td>
    <td>
      <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p>
    </td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Obter um painel]

Esse módulo de ação recupera metadados de um painel especificado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inserir uma ID de painel]</td>
      <td>
        <p>Selecione ou mapeie a opção para escolher o painel para o qual deseja recuperar metadados.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do painel]</td>
      <td>
        <p>Insira ou mapeie a ID do painel para o qual deseja recuperar metadados.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do grupo]  </td>
      <td>Selecione ou mapeie a ID do Grupo que possui os painéis para os quais deseja recuperar metadados.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obter um mosaico de painel]

Esse módulo de ação recupera metadados de um bloco de painel especificado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inserir uma ID de painel]</td>
      <td>
        <p>Selecione ou mapeie a opção para escolher os detalhes do painel que deseja recuperar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do painel]</td>
      <td>
        <p>Insira ou mapeie a ID do painel para a qual deseja recuperar detalhes.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tile ID]</td>
      <td>Insira ou mapeie a ID do [!DNL Power BI] bloco para o qual você deseja recuperar detalhes.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do grupo]  </td>
      <td>Selecione ou mapeie a ID do Grupo que possui o bloco que deseja recuperar.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Criar um painel]

Esse módulo de ação cria um novo painel.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Insira ou mapeie um nome para o Painel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do grupo]  </td>
      <td>Selecione ou mapeie a ID do Grupo que será o proprietário do novo Painel.</td>
    </tr>
  </tbody>
</table>

### Relatórios

#### [!UICONTROL Relatórios de lista]

Este módulo de pesquisa recupera uma lista de relatórios.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do grupo]  </td>
      <td>
        <p>Selecione ou mapeie a ID do Grupo que possui os relatórios que deseja listar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]  </td>
      <td>
        <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obter um relatório]

Esse módulo de ação recupera metadados de um relatório especificado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inserir uma ID de relatório]</td>
      <td>
        <p>Selecione ou mapeie a opção para escolher o relatório para o qual deseja recuperar metadados.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do relatório]</td>
      <td>
        <p>Insira ou mapeie a ID do relatório para o qual deseja recuperar metadados.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do grupo]  </td>
      <td>Selecione ou mapeie a ID do Grupo que possui o relatório para o qual deseja recuperar metadados.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Copiar um relatório]

Esse módulo de ação copia um relatório existente.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inserir uma ID de relatório]</td>
      <td>
        <p>Selecione ou mapeie a opção para escolher o relatório que deseja copiar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do relatório]</td>
      <td>
        <p>Insira ou mapeie a ID do relatório que deseja copiar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do grupo]  </td>
      <td>Selecione ou mapeie a ID do Grupo que possui o relatório que deseja copiar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Novo nome do relatório copiado]</td>
      <td>Insira ou mapeie um nome para o novo relatório.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Excluir um relatório]

Esse módulo de ação exclui um relatório.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inserir uma ID de relatório]</td>
      <td>
        <p>Selecione ou mapeie a opção para escolher o relatório que deseja excluir.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do relatório]</td>
      <td>
        <p>Insira ou mapeie a ID do relatório que deseja excluir.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do grupo]  </td>
      <td>Selecione ou mapeie a ID do Grupo que possui o relatório que deseja excluir.</td>
    </tr>
  </tbody>
</table>

### Conjunto de dados

#### [!UICONTROL Listar conjuntos de dados]

Esse módulo de pesquisa recupera uma lista de conjuntos de dados.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do grupo]  </td>
      <td>Selecione ou mapeie a ID do Grupo que possui o relatório para o qual deseja recuperar metadados.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]</td>
      <td>
        <p>Insira ou mapeie o número máximo de registros para o módulo [action] durante cada ciclo de execução de cenário.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obter um conjunto de dados]

Esse módulo de ação recupera metadados de um conjunto de dados especificado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inserir uma ID de relatório]</td>
      <td>
        <p>Selecione ou mapeie a opção para escolher o relatório para o qual deseja recuperar metadados.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do relatório]</td>
      <td>
        <p>Insira ou mapeie a ID do conjunto de dados para o qual deseja recuperar metadados.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do grupo]  </td>
      <td>Selecione ou mapeie a ID do Grupo que possui o conjunto de dados para o qual deseja recuperar metadados.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Criar um conjunto de dados]

Esse módulo de ação cria um novo conjunto de dados.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Insira ou mapeie um nome para o conjunto de dados.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do grupo]  </td>
      <td>Selecione ou mapeie a ID do Grupo que será o proprietário do novo conjunto de dados.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Modo Padrão]</td>
      <td>
        <p>Selecione ou mapeie o modo padrão do conjunto de dados:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Como Azure]</b>: Um conjunto de dados com uma conexão ativa com o [!DNL Azure Analysis Service]</p>
          </li>
          <li>
            <p><b>[!UICONTROL Como no Prem]</b>: Um conjunto de dados com uma conexão ativa com o [!DNL On-premise Analysis] Serviço</p>
          </li>
          <li>
            <p><b>[!DNL Push]</b>: Um conjunto de dados que permite acesso programático para enviar dados para o [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Push Streaming]</b>: Um conjunto de dados que suporta transmissão de dados e permite acesso programático para enviar dados para o [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Streaming]</b>: Um conjunto de dados compatível com o fluxo de dados</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tabelas]</td>
      <td>Adicionar tabelas ao conjunto de dados. Para campos, consulte <a href="#Table" class="MCXref_0">Campos de tabela</a></td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Data sources]</td>
      <td>Adicione as fontes de dados. Para campos, consulte <a href="#Data" class="MCXref_0">Campos de fontes de dados</a>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Default Retention Policy]  </td>
      <td>
        <p>Selecione ou mapeie a política intencional para o conjunto de dados:</p>
        <ul>
          <li>
            <p>[!UICONTROL Nenhum]</p>
          </li>
          <li>
            <p>[!UICONTROL FIFO básico]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Campos de tabela

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>
        <p>  Insira ou mapeie um nome para a tabela.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Colunas]</td>
      <td>
        <p>Adicione as colunas:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Insira (mapa) um nome de coluna.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Tipo de dados]</b>
            </p>
            <p>Selecione ou mapeie o tipo de dados:</p>
            <ul>
              <li>
                <p>[!UICONTROL String]</p>
              </li>
              <li>
                <p>[!UICONTROL Número inteiro]</p>
              </li>
              <li>
                <p>[!UICONTROL Boolean]</p>
              </li>
              <li>
                <p>[!UICONTROL Data Hora]</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>[!UICONTROL Formatar cadeia de caracteres]</b>
            </p>
            <p>Insira (mapeie) a string de formato.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Linhas]</td>
      <td>Insira ou mapeie os detalhes da linha.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Measures]</td>
      <td>Adicione a medida para as tabelas.</td>
    </tr>
  </tbody>
</table>

##### Campos de fontes de dados

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Banco de dados]  </td>
      <td>
        <p>Insira ou mapeie o banco de dados que deseja usar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Server]  </td>
      <td>
        <p>Insira ou mapeie o nome do servidor que deseja usar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]  </td>
      <td>
        <p>Insira ou mapeie o URL que deseja usar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID da fonte de dados]</td>
      <td>
        <p>  Insira ou mapeie a ID da fonte de dados.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de fonte de dados]  </td>
      <td>
        <p>Selecione ou mapeie o tipo de fonte de dados. Exemplo: SQL.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do gateway]  </td>
      <td>Insira ou mapeie a ID do gateway que deseja usar.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Adicionar ou excluir linhas em uma tabela de conjunto de dados]

Esse módulo de ação adiciona ou exclui linhas de uma tabela de conjunto de dados de push especificada.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inserir uma tabela]</td>
      <td>Selecione ou mapeie a opção para selecionar o conjunto de dados que contém a tabela que você deseja ajustar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do conjunto de dados]</td>
      <td>Insira ou mapeie a ID do conjunto de dados que contém as linhas que deseja adicionar ou excluir.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nome da tabela]  </td>
      <td>
        <p>Insira ou mapeie o nome da tabela que contém as linhas que deseja adicionar ou excluir.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do grupo]  </td>
      <td>Insira ou mapeie a ID do grupo que possui o conjunto de dados.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Selecionar a ação]</td>
      <td>
        <p>Selecione ou mapeie a ação que deseja executar.</p>
        <ul>
          <li>
            <p>[!UICONTROL Adicionar linhas]</p>
          </li>
          <li>
            <p>[!UICONTROL Excluir todas as linhas]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Linhas]</td>
      <td>
        <p>Adicione os campos de linha.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Chave]</b>
            </p>
            <p>Insira ou mapeie o nome da chave.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Tipo de campo]</b>
            </p>
            <p>Selecione ou mapeie o tipo de campo:</p>
            <ul>
              <li>
                <p>Booleano</p>
              </li>
              <li>
                <p>Data</p>
              </li>
              <li>
                <p>Texto</p>
              </li>
              <li>
                <p>Número</p>
              </li>
            </ul>
          </li>
          <li>
            <p>[!UICONTROL Valor]</p>
            <p>Insira ou mapeie o valor da chave.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Atualizar um conjunto de dados]

Este módulo de ação atualiza um conjunto de dados especificado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inserir um conjunto de dados]</td>
      <td>Selecione ou mapeie a opção para selecionar o conjunto de dados que deseja atualizar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do conjunto de dados]</td>
      <td>Insira ou mapeie a ID do conjunto de dados que deseja atualizar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nome da tabela]  </td>
      <td>
        <p>Insira ou mapeie o nome da tabela que contém as linhas que deseja adicionar ou excluir.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do grupo]  </td>
      <td>Insira ou mapeie a ID do grupo que possui o conjunto de dados.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Opção de notificação]  </td>
      <td>
        <p>Selecione ou mapeie a opção para notificar:</p>
        <ul>
          <li>
            <p>[!UICONTROL Email na conclusão]</p>
          </li>
          <li>
            <p>[!UICONTROL Email on Failure]</p>
          </li>
          <li>
            <p>[!UICONTROL Sem notificação]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Excluir um conjunto de dados]

Esse módulo de ação exclui um conjunto de dados.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inserir uma ID de relatório]</td>
      <td>
        <p>Selecione ou mapeie a opção para escolher o conjunto de dados que deseja excluir.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do relatório]</td>
      <td>
        <p>Insira ou mapeie a ID do conjunto de dados que deseja excluir.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do grupo]  </td>
      <td>Selecione ou mapeie a ID do Grupo que possui o conjunto de dados que deseja excluir.</td>
    </tr>
  </tbody>
</table>

### Aplicativos

#### [!UICONTROL Assista aos aplicativos]

Este módulo de acionador inicia um cenário quando um aplicativo é atualizado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]  </td>
      <td>
        <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Listar aplicativos]

Este módulo de pesquisa recupera uma lista de todos os aplicativos instalados.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]  </td>
      <td>
        <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Listar relatórios do aplicativo]

Este módulo de pesquisa recupera uma lista de todos os relatórios do aplicativo especificado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]</td>
      <td>Selecione ou mapeie a ID do aplicativo cujos relatórios você deseja listar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]  </td>
      <td>
        <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Listar painéis do aplicativo]

Este módulo de pesquisa recupera uma lista de painéis de um aplicativo especificado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]</td>
      <td>Selecione ou mapeie a ID do aplicativo cujos painéis você deseja listar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]  </td>
      <td>
        <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obter um aplicativo]

Este módulo de ação recupera metadados de um aplicativo especificado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Selecione ou mapeie a ID do aplicativo que deseja recuperar.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obter o relatório de um aplicativo]

Este módulo de ação recupera os metadados de um relatório de aplicativo especificado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Selecione ou mapeie a ID do aplicativo que contém o relatório que deseja recuperar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do relatório]</td>
      <td>
        <p>  Selecione ou mapeie a ID do relatório que deseja recuperar.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obter o painel de um aplicativo]

Este módulo de ação recupera os metadados do painel de um aplicativo especificado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Selecione ou mapeie a ID do aplicativo que contém o painel que você deseja recuperar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do relatório]</td>
      <td>
        <p>  Selecione ou mapeie a ID do painel que deseja recuperar.</p>
      </td>
    </tr>
  </tbody>
</table>

### Outro

#### [!UICONTROL Faça uma chamada de API]

Este módulo de ação executa uma chamada de API para o [!DNL Power BI] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Power BI] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Caminho]</p>
      </td>
      <td>
        <p>Insira um caminho relativo a <code>https://api.powerbi.com</code>. Exemplo: <code>/v1.0/myorg/datasets</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Método]</p>
      </td>
      <td>
        <p>Selecione o método de solicitação [!UICONTROL HTTP] que você precisa configurar a chamada da API. Para obter mais informações, consulte Métodos de solicitação [!UICONTROL HTTP] .</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cabeçalhos]</td>
      <td>
        <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p>
        <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] adiciona cabeçalhos de autorização e cabeçalhos x-api-key automaticamente.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Sequência de consulta]  </td>
      <td>
        <p>Insira a sequência de consulta da solicitação.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Corpo]</td>
   <td> <p>Adicione o conteúdo do corpo para a chamada da API no formato de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>
