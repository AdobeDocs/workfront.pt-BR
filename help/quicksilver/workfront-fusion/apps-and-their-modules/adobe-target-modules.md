---
filename: adobe-target-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos do Adobe Target
description: Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!DNL Adobe Target], as well as connect it to multiple third-party applications and services. [!DNL Adobe Target] Os módulos do permitem criar, ler, atualizar ou excluir registros, listar todos os registros de um determinado tipo, pesquisar registros com base nos critérios especificados ou executar uma chamada de API personalizada para o [!DNL Adobe Target] API.
author: Becky
feature: Workfront Fusion
exl-id: 9597806b-d4bf-4627-b27d-30e24a1e6776
source-git-commit: c0be0a1f21d5db3a480485a39e019a129d248574
workflow-type: tm+mt
source-wordcount: '2665'
ht-degree: 0%

---

# [!DNL Adobe Target] Módulos

Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!DNL Adobe Target], bem como conectá-lo a vários aplicativos e serviços de terceiros. [!DNL Adobe Target] Os módulos do permitem criar, ler, atualizar ou excluir registros, listar todos os registros de um determinado tipo, pesquisar registros com base nos critérios especificados ou executar uma chamada de API personalizada para o [!DNL Adobe Target] API.


Se precisar de instruções sobre como criar um cenário, consulte [Criar um cenário](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obter informações sobre módulos, consulte [Módulos no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e integração do trabalho] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Produto</td>
      <td>
   <p>Requisito atual do produto: se você tiver o [!UICONTROL Select] ou o [!UICONTROL Prime] [!DNL Adobe Workfront] Planejar, sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no [!UICONTROL Ultimate] [!DNL Workfront] plano.</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td>
    </tr>
    </tr>
  </tbody>
</table>


Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Antes de poder usar o [!DNL Adobe Target] deve garantir que os seguintes pré-requisitos sejam atendidos:

* Você deve ter um ativo [!DNL Adobe Target] conta.

## Criar uma conexão com o [!DNL Adobe Target]

Para criar uma conexão para o seu [!DNL Adobe Target] módulos:

1. Clique em **[!UICONTROL Adicionar]** ao lado da caixa Conexão.

1. Preencha os seguintes campos:

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Nome da Conexão]</td>
        <td>
          <p>Insira um nome para esta conexão.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID do Cliente]</td>
        <td>Insira seu [!DNL Adobe] ID do cliente. Isso pode ser encontrado na seção [!UICONTROL Credenciais detalhes] do [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Segredo do Cliente]</td>
        <td>Insira seu [!DNL Adobe] Segredo do cliente. Isso pode ser encontrado na seção [!UICONTROL Credenciais detalhes] do [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID da Organização]</td>
        <td>Insira seu [!DNL Adobe] ID da organização. Isso pode ser encontrado na seção [!UICONTROL Credenciais detalhes] do [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID da conta técnica]</td>
        <td>Insira seu [!DNL Adobe] ID da conta técnica. Isso pode ser encontrado na seção [!UICONTROL Credenciais detalhes] do [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Locatário]</td>
        <td>
          <p> Para localizar seu locatário, faça logon na [!DNL Adobe Experience Cloud], abrir [!DNL Target]e clique no botão [!DNL Target] cartão. Use o valor da ID do locatário conforme observado no subdomínio do URL.</p>
          <p>Por exemplo, se o URL ao fazer logon no [!DNL Adobe Target] é <code>&lt;https://mycompany.experiencecloud.adobe.com/...></code> em seguida, a ID do locatário é "mycompany".</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Metaescopos]</td>
        <td>Enter <code>ent_marketing_sdk</code>       </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Chave privada]</td>
        <td>
          <p>Insira a chave privada que foi gerada quando suas credenciais foram criadas na [!DNL Adobe Developer Console]. </p>
          <p>Para extrair sua chave privada ou certificado:</p>
          <ol>
            <li value="1">
              <p>Clique em <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>Selecione o tipo de arquivo que você está extraindo.</p>
            </li>
            <li value="3">
              <p>Selecione o arquivo que contém a chave privada ou o certificado.</p>
            </li>
            <li value="4">
              <p>Digite a senha do arquivo.</p>
            </li>
            <li value="5">
              <p>Clique em <b>[!UICONTROL Salvar]</b> para extrair o arquivo e retornar à configuração da conexão.</p>
            </li>
          </ol>
        </td>
      </tr>
    </tbody>
    </table>

1. Clique em **[!UICONTROL Continuar]** para salvar a conexão e retornar ao módulo.

## [!DNL Adobe Target] módulos e seus campos

Ao configurar [!DNL Adobe Target] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Adobe Target] Os campos podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Ações](#actions)

* [Pesquisas](#searches)


### Ações

* [[!UICONTROL Criar um registro]](#create-a-record)

* [[!UICONTROL Fazer uma chamada de API personalizada]](#make-a-custom-api-call)

* [[!UICONTROL Excluir um registro]](#delete-a-record)

* [[!UICONTROL Ler um registro]](#read-a-record)

* [[!UICONTROL Atualizar um registro]](#update-a-record)


#### [!UICONTROL Criar um registro]

Esse módulo de ação cria uma atividade AB ou XT, uma oferta ou um público-alvo.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Conexão]</td>
    <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Target], consulte <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Target]</a> neste artigo.</td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Tipo de registro]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>Selecione o tipo de registro que deseja criar.</p>
      <ul>
        <li>
          <p>[!UICONTROL Atividade AB]</p>
          <p>Continue para <a href="#ab-activity-fields" class="MCXref xref" >Campos de atividade AB</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Atividade XT]</p>
          <p>Continue para <a href="#xt-activity-fields" class="MCXref xref" >Campos de atividade de XT</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Oferta]</p>
          <p>Continue para <a href="#offer-fields" class="MCXref xref" >Campos de oferta</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Público-alvo]</p>
          <p>Continue para <a href="#audience-fields" class="MCXref xref" >Campos de público</a>.</p>
        </li>
      </ul>
    </td>
  </tr>
</tbody>
</table>

##### Campos de atividade AB

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Nome]</td>
      <td>Insira ou mapeie um nome para esta atividade. O nome não pode ter mais de 250 caracteres.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Opções]</td>
      <td>
        <p>Para cada opção que deseja adicionar à atividade, clique em <b>[!UICONTROL Adicionar item]</b> e preencha os seguintes campos:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL ID local da Opção]</b>
            </p>
            <p>Insira ou mapeie uma string a ser usada para rastrear a opção nas solicitações da API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Nome]</b>
            </p>
            <p>Insira ou mapeie um nome para a opção. O nome não deve ter mais de 250 caracteres.</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID da oferta]</b>
            </p>
          </li>
          <li>
            <p>Selecione ou mapeie a Oferta associada à opção.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Locais]</td>
      <td>
        <p>Para cada Mbox que você deseja adicionar à atividade, clique em <b>[!UICONTROL Adicionar item]</b> e preencha os seguintes campos:</p>
        <ul>
          <li>
            <p>[!UICONTROL IDs de público-alvo]</p>
            <p>Para cada público-alvo que você deseja adicionar à mbox, clique em <b>[!UICONTROL Adicionar item]</b> e selecione a ID de público-alvo.</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID Local do Local]</b>
            </p>
            <p>Insira ou mapeie uma string a ser usada para rastrear o local nas solicitações da API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Nome]</b>
            </p>
            <p>Insira ou mapeie um nome para o Local. O nome não deve ter mais de 250 caracteres.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Experiências]</td>
      <td>
        <p>Uma lista de locais na página onde a oferta de conteúdo é apresentada. Um local contém o seguinte:
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL ID de Experiência local]</b>
            </p>
            <p>Insira ou mapeie a ID da experiência</p>
          </li>
          <li>
            <p><b>[!UICONTROL Nome]</b>
            </p>
            <p>Insira ou mapeie o nome da experiência

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>Para cada público-alvo que você deseja ver a experiência, clique em <b>[!UICONTROL Adicionar item]</b> e insira a ID de público-alvo.

</p>
          </li>
          <li>
            <p><b>[!UICONTROL Porcentagem de Visitantes]</b>
            </p>
            <p>Insira ou mapeie a porcentagem de visitantes alocada para a experiência</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Métricas]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Terceiros]</td>
      <td>Insira ou mapeie uma ID para identificar esta atividade. Você pode escolher essa ID. Essa ID não deve ser igual a outra atividade e não pode ter mais de 250 caracteres.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inicia às]</td>
      <td>Insira ou mapeie a data e a hora para iniciar a atividade no formato <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Termina em]</td>
      <td>Insira ou mapeie a data e a hora para encerrar a atividade no formato <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Estado]</td>
      <td>
        <p>Insira ou mapeie o estado da atividade.</p>
        <ul>
          <li>
            <p>[!UICONTROL Aprovado]</p>
          </li>
          <li>
            <p>[!UICONTROL Desativado]</p>
          </li>
          <li>
            <p>[!UICONTROL Pausado]</p>
          </li>
          <li>
            <p>[!UICONTROL Salvo] </p>
          </li>
          <li>
            <p>[!UICONTROL Excluído]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Prioridade]</td>
      <td>Insira um número que defina a prioridade da atividade. Números mais altos têm prioridade mais alta. Esse valor deve estar entre 0 e 999. O valor padrão é 5.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Alocar tráfego automaticamente]</td>
      <td>
        <p>Ative essa opção para alocar o tráfego automaticamente. A alocação automática envia mais tráfego para a experiência mais bem-sucedida.</p>
        <p>Selecione ou mapeie os critérios de avaliação pelos quais julgar qual experiência é mais bem-sucedida.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Insira ou mapeie o espaço de trabalho ao qual a atividade está associada</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL IDs de Propriedades] </td>
      <td>Para cada propriedade que você deseja adicionar à atividade, clique em <b>[!UICONTROL Adicionar item]</b> e selecione ou mapeie a ID da propriedade.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Relatórios de públicos-alvo]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>Para cada público-alvo de relatório que você deseja adicionar à atividade, clique em [!UICONTROL Adicionar item] e insira as seguintes informações:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL ID Local do Público-alvo de Relatório]</b>
            </p>
            <p>Insira ou mapeie uma cadeia de caracteres a ser usada para rastrear o Público-alvo do relatório nas solicitações da API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID de público-alvo]</b>
            </p>
            <p>Inserir ou mapear o segmento a ser usado no relatório</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID local da métrica]</b>
            </p>
            <p>Insira ou mapeie uma string a ser usada para rastrear a métrica nas solicitações da API.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Campos de atividade de XT

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Nome]</td>
      <td>Insira ou mapeie um nome para esta atividade. O nome não pode ter mais de 250 caracteres.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Opções]</td>
      <td>
        <p>Para cada opção que deseja adicionar à atividade, clique em <b>[!UICONTROL Adicionar item]</b> e preencha os seguintes campos:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL ID local da Opção]</b>
            </p>
            <p>Insira ou mapeie uma string a ser usada para rastrear a opção nas solicitações da API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Nome]</b>
            </p>
            <p>Insira ou mapeie um nome para a opção. O nome não deve ter mais de 250 caracteres.</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID da oferta]</b>
            </p>
          </li>
          <li>
            <p>Selecione ou mapeie a Oferta associada à opção.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Locais]</td>
      <td>
        <p>Para cada Mbox que você deseja adicionar à atividade, clique em <b>[!UICONTROL Adicionar item]</b> e preencha os seguintes campos:</p>
        <ul>
          <li>
            <p>[!UICONTROL IDs de público-alvo]</p>
            <p>Para cada público-alvo que você deseja adicionar à mbox, clique em <b>[!UICONTROL Adicionar item]</b> e selecione a ID de público-alvo.</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID Local do Local]</b>
            </p>
            <p>Insira ou mapeie uma string a ser usada para rastrear o local nas solicitações da API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Nome]</b>
            </p>
            <p>Insira ou mapeie um nome para o Local. O nome não deve ter mais de 250 caracteres.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Experiências]</td>
      <td>
        <p>Uma lista de locais na página onde a oferta de conteúdo é apresentada. Um local contém o seguinte:
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL ID de Experiência local]</b>
            </p>
            <p>Insira ou mapeie a ID da experiência</p>
          </li>
          <li>
            <p><b>[!UICONTROL Nome]</b>
            </p>
            <p>Insira ou mapeie o nome da experiência

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>Para cada público-alvo que você deseja ver a experiência, clique em <b>[!UICONTROL Adicionar item]</b> e insira a ID de público-alvo.

</p>
          </li>
          <li>
            <p><b>[!UICONTROL Porcentagem de Visitantes]</b>
            </p>
            <p>Insira ou mapeie a porcentagem de visitantes alocada para a experiência</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Métricas]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Terceiros]</td>
      <td>Insira ou mapeie uma ID para identificar esta atividade. Você pode escolher essa ID. Essa ID não deve ser igual a outra atividade e não pode ter mais de 250 caracteres.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inicia às]</td>
      <td>Insira ou mapeie a data e a hora para iniciar a atividade no formato <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Termina em]</td>
      <td>Insira ou mapeie a data e a hora para encerrar a atividade no formato <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Estado]</td>
      <td>
        <p>Insira ou mapeie o estado da atividade.</p>
        <ul>
          <li>
            <p>[!UICONTROL Aprovado]</p>
          </li>
          <li>
            <p>[!UICONTROL Desativado]</p>
          </li>
          <li>
            <p>[!UICONTROL Pausado]</p>
          </li>
          <li>
            <p>[!UICONTROL Salvo] </p>
          </li>
          <li>
            <p>[!UICONTROL Excluído]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Prioridade]</td>
      <td>Insira um número que defina a prioridade da atividade. Números mais altos têm prioridade mais alta. Esse valor deve estar entre 0 e 999. O valor padrão é 5.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Alocar tráfego automaticamente]</td>
      <td>
        <p>Ative essa opção para alocar o tráfego automaticamente. A alocação automática envia mais tráfego para a experiência mais bem-sucedida.</p>
        <p>Selecione ou mapeie os critérios de avaliação pelos quais julgar qual experiência é mais bem-sucedida.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Insira ou mapeie o espaço de trabalho ao qual a atividade está associada</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL IDs de Propriedades] </td>
      <td>Para cada propriedade que você deseja adicionar à atividade, clique em <b>[!UICONTROL Adicionar item]</b> e selecione ou mapeie a ID da propriedade.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Relatórios de públicos-alvo]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>Para cada público-alvo de relatório que você deseja adicionar à atividade, clique em [!UICONTROL Adicionar item] e insira as seguintes informações:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL ID Local do Público-alvo de Relatório]</b>
            </p>
            <p>Insira ou mapeie uma cadeia de caracteres a ser usada para rastrear o Público-alvo do relatório nas solicitações da API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID de público-alvo]</b>
            </p>
            <p>Inserir ou mapear o segmento a ser usado no relatório</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID local da métrica]</b>
            </p>
            <p>Insira ou mapeie uma string a ser usada para rastrear a métrica nas solicitações da API.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Campos de oferta

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Nome]</td>
      <td>Insira ou mapeie um nome para esta atividade. O nome não pode ter mais de 250 caracteres.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Conteúdo]</td>
      <td>
        <p>Insira ou mapeie o conteúdo da oferta que será exibido para o usuário.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>Insira ou mapeie a ID do espaço de trabalho associado à oferta. Se deixado em branco, a oferta é associada ao espaço de trabalho padrão da conta. Essa funcionalidade se aplica somente ao [!DNL Target] Contas Premium.</p>
      </td>
    </tr>
  </tbody>
</table>

##### Campos de público

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Nome]</td>
      <td>Insira ou mapeie um nome para este público. O nome não pode ter mais de 250 caracteres.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Conteúdo]</td>
      <td>
        <p>Insira ou mapeie uma descrição deste público-alvo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Regra de Destino]</td>
      <td>
        <p>Ative a opção para criar regras AND, ou seja, todas as regras devem ser aplicadas.</p>
        <p>Para cada regra que você deseja aplicar ao público-alvo, clique em <b>[!UICONTROL Adicionar item]</b> e insira o JSON da regra que deseja aplicar. </p>
        <div class="example"><span class="autonumber"><span><b>Exemplo: </b></span></span>
          <p>Exemplos:</p>
          <p ><code>&lbrace;</code></p>
                    <p ><code>                "page": "url",</code>
                    </p>
                    <p><code>                "equals":&lbrack;</code>
                    </p>
                    <p ><code>                    "http://www.myhomepage.com/"</code>
                    </p>
                    <p><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;,</code>
                    </p>
                    <p ><code>            &lbrace;</code>
                    </p>
                    <p><code>                "geo": "region",</code>
                    </p>
                    <p><code>                "matches": &lbrack;</code>
                    </p>
                    <p ><code>                    "california"</code>
                    </p>
                    <p ><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;</code>
                    </p>
      </td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Workspace]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>Insira ou mapeie a ID do espaço de trabalho associado ao público. Se deixado em branco, a oferta é associada ao espaço de trabalho padrão da conta. Essa funcionalidade se aplica somente ao [!DNL Target Premium] contas.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Fazer uma chamada de API personalizada]

Esse módulo faz uma chamada de API personalizada para o [!DNL Adobe Target] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Target], consulte <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Target]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL [!DNL Target] URL base]</td>
      <td>Insira ou mapeie seu [!DNL Target] URL base.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Caminho]</p>
      </td>
      <td>
        <p>Insira um caminho relativo a {baseURL}/</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Método]</p>
      </td>
   <td> <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cabeçalhos]</td>
      <td>
        <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão.</p>
        <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] O adiciona cabeçalhos de autorização e cabeçalhos x-api-key automaticamente.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cadeia de Consulta]  </td>
      <td>
        <p>Insira a string de consulta da solicitação.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Corpo]</td>
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Excluir um registro]

Esse módulo de ação exclui uma única atividade AB, atividade XT, Oferta ou Público-alvo.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Conexão]</td>
    <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Target], consulte <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Target]</a> neste artigo.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Tipo de registro]</td>
    <td>Selecione o tipo de registro que deseja excluir.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL ID de Registro]</td>
    <td>Informe ou mapeie a ID do registro que deseja deletar.</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Ler um registro]

Este módulo de ação recupera dados para uma única Atividade, Oferta, Público-alvo, Propriedade ou Relatório.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Conexão]</td>
    <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Target], consulte <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Target]</a> neste artigo.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Tipo de registro]</td>
    <td>Selecione o tipo de registro que deseja ler.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL ID de Registro]</td>
    <td>Insira ou mapeie a ID do registro que deseja ler.</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Atualizar um registro]

Esse módulo de ação atualiza uma Atividade, Oferta ou Público-alvo.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Target], consulte <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Target]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de registro]</td>
      <td>
        <p>Selecione o tipo de registro que deseja atualizar.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Atividade AB]</b>
            </p>
            <p>Consulte descrições de campo em <a href="#ab-activity-fields" class="MCXref xref" >Campos de atividade AB</a> em <a href="#create-a-record" class="MCXref xref" >Criar um registro</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Atividade XT]</b>
            </p>
            <p>Consulte descrições de campo em <a href="#xt-activity-fields" class="MCXref xref" >Campos de atividade de XT</a> em <a href="#create-a-record" class="MCXref xref" >Criar um registro</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Outra Atividade]</b>
            </p>
            <p>Selecione o campo para o qual deseja atualizar um valor e insira o novo valor do campo.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Oferta]</b>
            </p>
            <p>Consulte descrições de campo em <a href="#offer-fields" class="MCXref xref" >Campos de oferta</a> em <a href="#create-a-record" class="MCXref xref" >Criar um registro</a>.</p>
          </li>
          <li>
            <p><b>[!DNL Audience]</b>
            </p>
            <p>Consulte descrições de campo em <a href="#audience-fields" class="MCXref xref" >Campos de público</a> em <a href="#create-a-record" class="MCXref xref" >Criar um registro</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de Registro]</td>
      <td>Insira ou mapeie a ID do registro que deseja atualizar.</td>
    </tr>
  </tbody>
</table>

### Pesquisas

* [[!UICONTROL Obter registros]](#get-records)

* [[!UICONTROL Pesquisa]](#search)


#### [!UICONTROL Obter registros]

Este módulo de pesquisa recupera uma lista de registros do tipo selecionado.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Target], consulte <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Target]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de registro]</td>
      <td>Selecione o tipo de registro que deseja atualizar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Classificar por]</td>
      <td>Para cada campo pelo qual deseja classificar, clique em <b>[!UICONTROL Adicionar item]</b> e selecione o campo e se os resultados retornados devem ser crescentes ou decrescentes.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inicia Em]</td>
      <td>
        <p>Insira a data mais antiga para a qual você deseja recuperar registros. </p>
        <p>Para obter uma lista de formatos de data e hora compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerção de tipo em [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Termina Em]</td>
      <td>
        <p>Insira a última data para a qual deseja recuperar registros. </p>
        <p>Para obter uma lista de formatos de data e hora compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerção de tipo em [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Pesquisa]

Este módulo de pesquisa pesquisa por Atividades, Ofertas ou Públicos-alvo com base nos critérios especificados.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Conexão]</td>
    <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Target], consulte <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Criar uma conexão com o [!DNL Adobe Target]</a> neste artigo.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Tipo de registro]</td>
    <td>Selecione o tipo de registro que deseja atualizar.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Classificar por]</td>
    <td>Para cada campo pelo qual deseja classificar, clique em <b>[!UICONTROL Adicionar item]</b> e selecione o campo e se os resultados retornados devem ser crescentes ou decrescentes.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Pesquisar critérios]</td>
    <td>Para cada regra que você deseja configurar, selecione o campo, o operador e o valor. Clique em <b>[!UICONTROL Adicionar regra AND]</b> para criar regras adicionais.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Deslocamento]</td>
    <td>
      <p>Insira o número da primeira resposta que você deseja que o módulo retorne. A primeira resposta retornada tem um deslocamento de <code>0</code>. Use este campo em combinação com o campo [!UICONTROL Número máximo de resultados retornados] para paginar as respostas.</p>
      <p>Por exemplo, para ver a terceira página de respostas, quando cada página tiver dez respostas, defina [!UICONTROL Deslocamento] como 20 e [!UICONTROL Número máximo de resultados retornados] como 10.</p>
    </td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Número máximo de resultados retornados]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário. Use este campo em combinação com o campo [!UICONTROL Deslocamento] para paginar as respostas.</p>
      <p>Por exemplo, para ver a terceira página de respostas, quando cada página tiver dez respostas, defina [!UICONTROL Deslocamento] como 20 e [!UICONTROL Número máximo de resultados retornados] como 10.</p>
    </td>
  </tr>
</tbody>
</table>
