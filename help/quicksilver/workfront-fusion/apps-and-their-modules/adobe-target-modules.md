---
filename: adobe-target-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos Adobe Target
description: Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Adobe Target], as well as connect it to multiple third-party applications and services. [!DNL Adobe Target] os módulos permitem criar, ler, atualizar ou excluir registros, listar todos os registros de um determinado tipo, pesquisar registros com base nos critérios especificados ou executar uma chamada de API personalizada para a [!DNL Adobe Target] API.
author: Becky
exl-id: 9597806b-d4bf-4627-b27d-30e24a1e6776
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2598'
ht-degree: 0%

---

# [!DNL Adobe Target] Módulos

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Adobe Target], bem como conectá-lo a vários aplicativos e serviços de terceiros. [!DNL Adobe Target] os módulos permitem criar, ler, atualizar ou excluir registros, listar todos os registros de um determinado tipo, pesquisar registros com base nos critérios especificados ou executar uma chamada de API personalizada para a [!DNL Adobe Target] API.


Se precisar de instruções para criar um cenário, consulte [Criar um cenário](../../workfront-fusion/scenarios/create-a-scenario.md).

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
      <td >
        <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Produto</td>
      <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td>
    </tr>
    </tr>
  </tbody>
</table>


Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Antes de usar a variável [!DNL Adobe Target] , você deve garantir que os seguintes pré-requisitos sejam atendidos:

* Você deve ter um [!DNL Adobe Target] conta.

## Criar uma conexão com [!DNL Adobe Target]

Para criar uma conexão para [!DNL Adobe Target] módulos:

1. Clique em **[!UICONTROL Adicionar]** ao lado da caixa Conexão.

1. Preencha os seguintes campos:

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Nome da conexão]</td>
        <td>
          <p>Digite um nome para esta conexão.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Insira seu [!DNL Adobe] ID do cliente. Isso pode ser encontrado na seção [!UICONTROL Credentials] da seção [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Segredo do cliente]</td>
        <td>Insira seu [!DNL Adobe] Segredo do cliente. Isso pode ser encontrado na seção [!UICONTROL Credentials] da seção [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Organization ID]</td>
        <td>Insira seu [!DNL Adobe] ID da organização. Isso pode ser encontrado na seção [!UICONTROL Credentials] da seção [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID da conta técnica]</td>
        <td>Insira seu [!DNL Adobe] ID da conta técnica. Isso pode ser encontrado na seção [!UICONTROL Credentials] da seção [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Tenant]</td>
        <td>
          <p> Para localizar seu locatário, faça logon no [!DNL Adobe Experience Cloud], abrir [!DNL Target]e clique no botão [!DNL Target] cartão. Use o valor da ID do locatário, conforme observado no subdomínio do URL.</p>
          <p>Por exemplo, se o URL estiver conectado a [!DNL Adobe Target] é <code>&lt;https://mycompany.experiencecloud.adobe.com/...></code> então sua ID do locatário é "minha empresa".</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Metscópios]</td>
        <td>Enter <code>ent_marketing_sdk</code>       </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Chave privada]</td>
        <td>
          <p>Insira a chave privada que foi gerada quando suas credenciais foram criadas no [!DNL Adobe Developer Console]. </p>
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

Ao configurar [!DNL Adobe Target] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Adobe Target] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Ações](#actions)

* [Pesquisas](#searches)


### Ações

* [[!UICONTROL Criar um registro]](#create-a-record)

* [[!UICONTROL Efetuar uma chamada de API personalizada]](#make-a-custom-api-call)

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
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Target], consulte <a href="#Create" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Target]</a> neste artigo.</td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Tipo de registro]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>Selecione o tipo de registro que deseja criar.</p>
      <ul>
        <li>
          <p>[!UICONTROL AB Activity]</p>
          <p>Continue para <a href="#AB%C2%A0Activ" class="MCXref xref" >Campos de atividade AB</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Atividade XT]</p>
          <p>Continue para <a href="#XT" class="MCXref xref" >Campos de atividade XT</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Offer]</p>
          <p>Continue para <a href="#Offer" class="MCXref xref" >Campos de oferta</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Público-alvo]</p>
          <p>Continue para <a href="#Audience" class="MCXref xref" >Campos de público-alvo</a>.</p>
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
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Insira ou mapeie um nome para esta atividade. O nome não pode ter mais de 250 caracteres.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Opções]</td>
      <td>
        <p>Para cada opção que deseja adicionar à atividade, clique em <b>[!UICONTROL Adicionar item]</b> e preencha os seguintes campos:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Opção ID local]</b>
            </p>
            <p>Insira ou mapeie uma string a ser usada para rastrear a opção nas solicitações de API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Insira ou mapeie um nome para a opção. O nome não deve ter mais de 250 caracteres.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Offer ID]</b>
            </p>
          </li>
          <li>
            <p>Selecione ou mapeie a Oferta associada à opção .</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Localizações]</td>
      <td>
        <p>Para cada Mbox que você deseja adicionar à atividade, clique em <b>[!UICONTROL Adicionar item]</b> e preencha os seguintes campos:</p>
        <ul>
          <li>
            <p>[!UICONTROL IDs de público-alvo]</p>
            <p>Para cada público-alvo que você deseja adicionar à Mbox, clique em <b>[!UICONTROL Adicionar item]</b> e selecione a ID de público-alvo.</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID local]</b>
            </p>
            <p>Insira ou mapeie uma string a ser usada para rastrear o local nas solicitações de API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Insira ou mapeie um nome para a Localização. O nome não deve ter mais de 250 caracteres.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Experiências]</td>
      <td>
        <p>Uma lista de locais na página onde a oferta de conteúdo é disponibilizada. Um local contém o seguinte:
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience ID local]</b>
            </p>
            <p>Insira ou mapeie a ID da experiência</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
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
            <p><b>[!UICONTROL Porcentagem do visitante]</b>
            </p>
            <p>Inserir ou mapear a porcentagem de visitantes alocada para a experiência</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Métricas]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de terceiros]</td>
      <td>Insira ou mapeie uma ID para identificar essa atividade. Você pode escolher essa ID. Essa ID não deve ser igual a outra atividade e não pode ter mais de 250 caracteres.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL inicia em]</td>
      <td>Insira ou mapeie a data e a hora para iniciar a atividade no formato <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL termina em]</td>
      <td>Insira ou mapeie a data e a hora para terminar a atividade no formato <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
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
            <p>[!UICONTROL desativado]</p>
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
      <td role="rowheader">[!UICONTROL Autoalocar tráfego]</td>
      <td>
        <p>Ative essa opção para alocar o tráfego automaticamente. A alocação automática envia mais tráfego para a experiência mais bem-sucedida.</p>
        <p>Selecione ou mapeie os critérios de avaliação pelos quais avaliar qual experiência é mais bem sucedida.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Inserir ou mapear o espaço de trabalho ao qual a atividade está associada</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL IDs de propriedades] </td>
      <td>Para cada propriedade que deseja adicionar à atividade, clique em <b>[!UICONTROL Adicionar item]</b> e selecione ou mapeie a ID da propriedade.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Reporting audiences]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>Para cada público-alvo de relatório que deseja adicionar à atividade, clique em [!UICONTROL Adicionar item] e insira as seguintes informações:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL ID local do público-alvo dos relatórios]</b>
            </p>
            <p>Insira ou mapeie uma string a ser usada para rastrear o Público de relatórios nas solicitações da API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Audience ID]</b>
            </p>
            <p>Inserir ou mapear o Segmento a ser usado no relatório</p>
          </li>
          <li>
            <p><b>[!UICONTROL Métrica ID local]</b>
            </p>
            <p>Insira ou mapeie uma string a ser usada para rastrear a métrica nas solicitações da API.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Campos de atividade XT

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Insira ou mapeie um nome para esta atividade. O nome não pode ter mais de 250 caracteres.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Opções]</td>
      <td>
        <p>Para cada opção que deseja adicionar à atividade, clique em <b>[!UICONTROL Adicionar item]</b> e preencha os seguintes campos:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Opção ID local]</b>
            </p>
            <p>Insira ou mapeie uma string a ser usada para rastrear a opção nas solicitações de API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Insira ou mapeie um nome para a opção. O nome não deve ter mais de 250 caracteres.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Offer ID]</b>
            </p>
          </li>
          <li>
            <p>Selecione ou mapeie a Oferta associada à opção .</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Localizações]</td>
      <td>
        <p>Para cada Mbox que você deseja adicionar à atividade, clique em <b>[!UICONTROL Adicionar item]</b> e preencha os seguintes campos:</p>
        <ul>
          <li>
            <p>[!UICONTROL IDs de público-alvo]</p>
            <p>Para cada público-alvo que você deseja adicionar à Mbox, clique em <b>[!UICONTROL Adicionar item]</b> e selecione a ID de público-alvo.</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID local]</b>
            </p>
            <p>Insira ou mapeie uma string a ser usada para rastrear o local nas solicitações de API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Insira ou mapeie um nome para a Localização. O nome não deve ter mais de 250 caracteres.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Experiências]</td>
      <td>
        <p>Uma lista de locais na página onde a oferta de conteúdo é disponibilizada. Um local contém o seguinte:
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience ID local]</b>
            </p>
            <p>Insira ou mapeie a ID da experiência</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
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
            <p><b>[!UICONTROL Porcentagem do visitante]</b>
            </p>
            <p>Inserir ou mapear a porcentagem de visitantes alocada para a experiência</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Métricas]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de terceiros]</td>
      <td>Insira ou mapeie uma ID para identificar essa atividade. Você pode escolher essa ID. Essa ID não deve ser igual a outra atividade e não pode ter mais de 250 caracteres.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL inicia em]</td>
      <td>Insira ou mapeie a data e a hora para iniciar a atividade no formato <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL termina em]</td>
      <td>Insira ou mapeie a data e a hora para terminar a atividade no formato <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
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
            <p>[!UICONTROL desativado]</p>
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
      <td role="rowheader">[!UICONTROL Autoalocar tráfego]</td>
      <td>
        <p>Ative essa opção para alocar o tráfego automaticamente. A alocação automática envia mais tráfego para a experiência mais bem-sucedida.</p>
        <p>Selecione ou mapeie os critérios de avaliação pelos quais avaliar qual experiência é mais bem sucedida.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Inserir ou mapear o espaço de trabalho ao qual a atividade está associada</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL IDs de propriedades] </td>
      <td>Para cada propriedade que deseja adicionar à atividade, clique em <b>[!UICONTROL Adicionar item]</b> e selecione ou mapeie a ID da propriedade.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Reporting audiences]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>Para cada público-alvo de relatório que deseja adicionar à atividade, clique em [!UICONTROL Adicionar item] e insira as seguintes informações:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL ID local do público-alvo dos relatórios]</b>
            </p>
            <p>Insira ou mapeie uma string a ser usada para rastrear o Público de relatórios nas solicitações da API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Audience ID]</b>
            </p>
            <p>Inserir ou mapear o Segmento a ser usado no relatório</p>
          </li>
          <li>
            <p><b>[!UICONTROL Métrica ID local]</b>
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
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Insira ou mapeie um nome para esta atividade. O nome não pode ter mais de 250 caracteres.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Conteúdo]</td>
      <td>
        <p>Insira ou mapeie o conteúdo da Oferta que será exibida para o usuário.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>Insira ou mapeie a ID do espaço de trabalho associado à oferta. Caso deixado em branco, a oferta será associada ao espaço de trabalho padrão da conta. Essa funcionalidade se aplica somente a [!DNL Target] Contas Premium.</p>
      </td>
    </tr>
  </tbody>
</table>

##### Campos de público-alvo

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Insira ou mapeie um nome para esse público-alvo. O nome não pode ter mais de 250 caracteres.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Conteúdo]</td>
      <td>
        <p>Insira ou mapeie uma descrição desse público-alvo.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Regra do Target]</td>
      <td>
        <p>Ative o botão para criar regras E, ou seja, todas as regras devem ser aplicadas.</p>
        <p>Para cada regra que deseja aplicar ao público-alvo, clique em <b>[!UICONTROL Adicionar item]</b> e insira o JSON da regra que deseja aplicar. </p>
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
        <p>Insira ou mapeie a ID do espaço de trabalho associada ao público-alvo. Caso deixado em branco, a oferta será associada ao espaço de trabalho padrão da conta. Essa funcionalidade se aplica somente a [!DNL Target Premium] contas.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Efetuar uma chamada de API personalizada]

Esse módulo faz uma chamada de API personalizada para o [!DNL Adobe Target] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Target], consulte <a href="#Create" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Target]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL [!DNL Target] URL base]</td>
      <td>Insira ou mapeie a [!DNL Target] URL base.</td>
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
   <td> <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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

#### [!UICONTROL Excluir um registro]

Esse módulo de ação exclui uma única atividade AB, atividade XT, Oferta ou Público-alvo.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Target], consulte <a href="#Create" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Target]</a> neste artigo.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Tipo de registro]</td>
    <td>Selecione o tipo de registro que deseja excluir.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL ID do registro]</td>
    <td>Insira ou mapeie a ID do registro que deseja excluir.</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Ler um registro]

Esse módulo de ação recupera dados de uma única Atividade, Oferta, Público-alvo, Propriedade ou Relatório.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Target], consulte <a href="#Create" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Target]</a> neste artigo.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Tipo de registro]</td>
    <td>Selecione o tipo de registro que deseja ler.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL ID do registro]</td>
    <td>Insira ou mapeie a ID do registro que deseja ler.</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Atualizar um registro]

Este módulo de ação atualiza uma Atividade, Oferta ou Público-alvo.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Target], consulte <a href="#Create" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Target]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de registro]</td>
      <td>
        <p>Selecione o tipo de registro que deseja atualizar.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL AB Activity]</b>
            </p>
            <p>Consulte descrições de campo em <a href="#AB%C2%A0Activ" class="MCXref xref" >Campos de atividade AB</a> under <a href="#Create2" class="MCXref xref" >Criar um registro</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Atividade XT]</b>
            </p>
            <p>Consulte descrições de campo em <a href="#XT" class="MCXref xref" >Campos de atividade XT</a> under <a href="#Create2" class="MCXref xref" >Criar um registro</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Outra Atividade]</b>
            </p>
            <p>Selecione o campo para o qual deseja atualizar um valor e insira o novo valor para o campo.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Offer]</b>
            </p>
            <p>Consulte descrições de campo em <a href="#Offer" class="MCXref xref" >Campos de oferta</a> under <a href="#Create2" class="MCXref xref" >Criar um registro</a>.</p>
          </li>
          <li>
            <p><b>[!DNL Audience]</b>
            </p>
            <p>Consulte descrições de campo em <a href="#Audience" class="MCXref xref" >Campos de público-alvo</a> under <a href="#Create2" class="MCXref xref" >Criar um registro</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID do registro]</td>
      <td>Insira ou mapeie a ID do registro que deseja atualizar.</td>
    </tr>
  </tbody>
</table>

### Pesquisas

* [[!UICONTROL Obter registros]](#get-records)

* [[!UICONTROL Pesquisar]](#search)


#### [!UICONTROL Obter registros]

Esse módulo de pesquisa recupera uma lista de registros do tipo selecionado.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Target], consulte <a href="#Create" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Target]</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tipo de registro]</td>
      <td>Selecione o tipo de registro que deseja atualizar.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Classificar por]</td>
      <td>Para cada campo que deseja classificar, clique em <b>[!UICONTROL Adicionar item]</b> e selecione o campo e se os resultados retornados devem ser crescentes ou decrescentes.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Inicia Em]</td>
      <td>
        <p>Insira a data mais antiga para a qual deseja recuperar registros. </p>
        <p>Para obter uma lista de formatos de data e hora compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coação de tipo em [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Termina Em]</td>
      <td>
        <p>Insira a data mais recente para a qual você deseja recuperar registros. </p>
        <p>Para obter uma lista de formatos de data e hora compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coação de tipo em [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Pesquisar]

Este módulo de pesquisa pesquisa pesquisa por Atividades, Ofertas ou Públicos-alvo com base nos critérios que você especificar.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Para obter instruções sobre como criar uma conexão com o [!DNL Adobe Target], consulte <a href="#Create" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Target]</a> neste artigo.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Tipo de registro]</td>
    <td>Selecione o tipo de registro que deseja atualizar.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Classificar por]</td>
    <td>Para cada campo que deseja classificar, clique em <b>[!UICONTROL Adicionar item]</b> e selecione o campo e se os resultados retornados devem ser crescentes ou decrescentes.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Critérios de pesquisa]</td>
    <td>Para cada regra que deseja configurar, selecione o campo , o operador e o valor. Clique em <b>[!UICONTROL Adicionar regra E]</b> para criar regras adicionais.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Deslocamento]</td>
    <td>
      <p>Insira o número da primeira resposta que você deseja que o módulo retorne. A primeira resposta retornada tem um deslocamento de <code>0</code>. Use esse campo em combinação com o campo [!UICONTROL Número máximo de resultados retornados] para paginar as respostas.</p>
      <p>Por exemplo, para ver a terceira página de respostas, quando cada página tiver dez respostas, defina [!UICONTROL Offset] como 20 e [!UICONTROL Número máximo de respostas] como 10.</p>
    </td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Número máximo de resultados retornados]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário. Use esse campo em combinação com o campo [!UICONTROL Offset] para paginar as respostas.</p>
      <p>Por exemplo, para ver a terceira página de respostas, quando cada página tiver dez respostas, defina [!UICONTROL Offset] como 20 e [!UICONTROL Número máximo de respostas] como 10.</p>
    </td>
  </tr>
</tbody>
</table>
