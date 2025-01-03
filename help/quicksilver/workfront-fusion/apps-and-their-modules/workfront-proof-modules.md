---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Workfront Proof
description: Em um cenário  [!DNL Adobe Workfront Fusion] , é possível automatizar fluxos de trabalho que usam  [!DNL Workfront Proof], bem como conectá-los a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion, Workfront Proof, Digital Content and Documents
exl-id: f5c6fb08-880d-4432-aef1-57db13b3ecdb
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '3176'
ht-degree: 0%

---

# [!DNL Workfront Proof] módulos

Em um cenário [!DNL Adobe Workfront Fusion], você pode automatizar fluxos de trabalho que usam [!DNL Workfront Proof], bem como conectá-los a vários aplicativos e serviços de terceiros.

Isso é útil se você precisar executar tarefas que atualmente não têm suporte na prova no [!DNL Workfront] ou no [!DNL Workfront Proof], como atualizar provas com base em determinados eventos e procurar os destinatários de uma prova.

O conector [!DNL Workfront Proof] não conta com o número de aplicativos ativos disponíveis para a sua organização. Todos os cenários, mesmo que usem apenas o aplicativo [!DNL Workfront Proof], contam com a contagem total de cenários de sua organização.

Se você precisar de instruções sobre como criar um cenário, consulte [Criar um cenário [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obter informações sobre módulos, consulte [Módulos em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td>
  <td> <p>[!UICONTROL Pro] ou superior</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td>
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td> 
   <td>
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para Automação do Trabalho]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o plano [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], sua organização deve comprar [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Informações do Workfront Proof

O conector do Workfront Proof usa o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Versão da API</td> 
   <td> v21.3.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tag da API</td> 
   <td>v1.8.92</td> 
  </tr>
 </tbody> 
 </table>

## Conectar [!DNL Workfront Proof] a [!DNL Workfront Fusion]

Você pode criar uma conexão com sua conta do [!DNL Workfront Proof] diretamente de dentro de um módulo do [!DNL Workfront Fusion].

1. Em qualquer módulo [!DNL Workfront Fusion], clique em [!UICONTROL **Adicionar**] ao lado do campo [!UICONTROL Conexão]

2. Preencha os seguintes campos:

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL Nome da Conexão]</p>
                </td>
                <td>Insira um nome para a conexão</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL.connections.environmentType]</td>
                <td>Selecione se é um ambiente de Produção ou um ambiente de não produção, como Pré-visualização ou Sandbox.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL.connections.authenticationType]</td>
                <td>Selecione se é uma Conta de serviço ou uma Conta pessoal.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Email / Nome de Usuário]</td>
                <td>Digite o nome de usuário para sua conta [!DNL Workfront Proof].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Senha]</td>
                <td>Digite a senha da sua conta [!DNL Workfront Proof].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL ID de Locatário]</td>
                <td><strong>Observação</strong>: os clientes que não usam BYOK devem deixar este campo em branco. <p>Insira a ID do locatário para esta conta. Se precisar de ajuda para encontrar sua ID de locatário, entre em contato com o Suporte ao cliente da Workfront.</p></td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Extensão de Domínio]</td>
                <td>Insira a extensão do URL que você usa para acessar sua conta. <p>Exemplo: <code>com</code> ou <code>eu</code></p></td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Produção, Visualização ou Ambiente Personalizado]</td>
                <td>Selecione uma conexão com um ambiente de produção, de visualização ou personalizado.</td>
            </tr>
        </tbody>
    </table>


3. Clique em [!UICONTROL **Continuar**] para salvar a conexão e retornar ao módulo

## [!DNL Workfront Proof] módulos e seus campos

Ao configurar módulos do [!DNL Workfront Proof], o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL Workfront Proof] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)
* [Pesquisas](#searches)

### Triggers

* [Assistir provas](#watch-proofs)
* [Aguarde o resumo do PDF](#watch-for-pdf-summary)
* [[!UICONTROL Atividade Assistir Prova]](#watch-proof-activity)

#### [!UICONTROL Assistir Provas]

Esse módulo de acionador agendado executa um cenário quando alguém cria ou toma uma decisão sobre uma prova.

O módulo retorna uma lista de todos os registros encontrados durante o período especificado, juntamente com seus tipos. Também retorna os valores dos campos especificados. Se o módulo encontrou decisões tomadas na prova, ele inclui os valores anterior e atual, em campos separados. Você pode mapear essas informações em módulos subsequentes no cenário.

Isso acontece em um intervalo programado regularmente especificado por você.

Você deve ter permissões suficientes para acessar a prova ou provas em [!DNL Workfront Proof] para recuperar essas informações.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Workfront Proof] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo de registro</td> 
   <td>Selecione o tipo de registro [!DNL Workfront Proof] que você deseja que o módulo assista.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Saídas</td> 
   <td> <p>Selecione as informações que deseja incluir no pacote de saída deste módulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Limite</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atenção ao Resumo de PDF]

Esse módulo de acionador instantâneo executa um cenário quando alguém cria um resumo de PDF para uma prova.

Um webhook é necessário neste módulo.

O módulo retorna todos os campos padrão associados à prova, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Ele também cria uma nova assinatura de evento para resumos de PDF e gera o conteúdo do atributo &quot;pdf_url&quot; enviado na carga. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Workfront Proof] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td>Você pode selecionar um webhook existente ou criar um novo. Para obter mais informações, consulte <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Acionadores instantâneos (webhooks) em [!DNL Adobe Workfront Fusion]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite]</td> 
   <td>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atividade Assistir Prova]

Esse módulo de acionamento executa um cenário quando uma atividade especificada ocorre em uma prova de prova.

O módulo retorna todos os campos padrão associados à prova, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Ele também cria uma nova assinatura de evento para resumos de PDF e gera o conteúdo do atributo `pdf_url` enviado na carga. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Workfront Proof] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de atividade]</td> 
   <td>Selecione se você deseja observar qualquer nova decisão (incluindo as alterações de status da [!UICONTROL proof]) ou somente as alterações de status da prova geral.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite]</td> 
   <td>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Criar prova]](#create-proof)
* [[!UICONTROL Chamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Baixar Prova]](#download-proof)
* [[!UICONTROL Ler um Registro]](#read-a-record)
* [[!UICONTROL Solicitar Resumo de PDF]](#request-pdf-summary)
* [[!UICONTROL Atualizar Prova]](#update-proof)
* [[!UICONTROL Carregar arquivo]](#upload-file)

#### [!UICONTROL Criar prova]

Este módulo de ação cria uma nova prova ou uma nova versão de uma prova no [!DNL Workfront Proof].

Especifique os parâmetros para a nova prova e a prova de origem se estiver criando uma nova versão.

O módulo retorna a ID da nova prova ou versão de prova. Você pode mapear essas informações nos módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Workfront Proof] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Prova]</td> 
   <td> <p>Especifique se deseja que a prova criada tenha um fluxo de trabalho básico ou um [!UICONTROL Fluxo de trabalho automatizado].</p> <p>Em seguida, preencha os campos exibidos para o tipo de prova escolhido. Por exemplo, se você escolher [!UICONTROL Fluxo de Trabalho Automatizado], preencha o campo <strong>[!UICONTROL Fases de Fluxo de Trabalho]</strong> para configurar as etapas.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Permitir o download do arquivo original]</td> 
   <td>Selecione se deseja permitir que o arquivo original, do qual a prova foi criada, seja baixado.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Visualizador Clássico de Prova]</td> 
   <td>Selecione se você está usando o Visualizador de prova clássico.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Combinar todos os arquivos em uma única prova]</td> 
   <td>Habilite essa opção para combinar todos os arquivos em uma única prova de várias páginas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Criar uma nova versão de prova]</td> 
   <td>Selecione esta opção se desejar que o módulo crie uma nova versão de uma prova existente. Em seguida, no campo <strong>[!UICONTROL ID de Prova Existente]</strong> que é exibido, mapeie ou insira o ID exclusivo da prova.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rótulo de Link Personalizado]</td> 
   <td>Insira ou mapeie um rótulo para o link de prova personalizado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL de Link Personalizado]</td> 
   <td>Insira ou mapeie o URL do link personalizado.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Notificações de email padrão para assinantes]</td> 
   <td>Digite um dos números a seguir para indicar qual das seguintes configurações de notificação por email padrão você deseja usar para a prova que foi criada.
    <ul>
     <li><strong>1</strong> - Todos os novos comentários e respostas</li>
     <li><strong>2</strong> - Respostas aos meus comentários</li>
     <li><strong>3</strong> - Resumo diário</li>
     <li><strong>4</strong> - Resumo por hora</li>
     <li><strong>5</strong> - Somente decisões</li>
     <li><strong>9</strong> - Desabilitado</li>
    </ul></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Desabilitar Resumo do Excel]</td> 
   <td>Selecione se você deseja desativar a capacidade de baixar comentários de prova para um arquivo do Excel.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Desabilitar Resumo de PDF]</td> 
   <td>Selecione se deseja desativar a capacidade de baixar comentários de prova para um arquivo PDF.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Desabilitar Email de Assinatura]</td> 
   <td>Selecione se deseja desabilitar o email de assinatura para esta prova.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Habilitar Reprodutor Incorporado]</td> 
   <td>Selecione se deseja ativar o reprodutor incorporado para esta prova.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Habilitar Assinaturas]</td> 
   <td>Selecione se as pessoas que não são participantes têm permissão para assinar a prova.<br>Se você selecionar esta opção, também poderá selecionar a Função Padrão para assinantes, conforme descrito nesta tabela.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Habilitar Validação de Assinaturas]</td> 
   <td>Selecione se deseja habilitar a validação de email de assinatura. Se isso estiver ativado, o assinante deve clicar em um link em um email para acessar uma prova.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Habilitar URL da Equipe]</td> 
   <td>Selecione se deseja que a prova criada oculte ou mostre o URL da equipe.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Hash do Arquivo] <span style="font-weight: normal;">ou</span> [!UICONTROL Hashes do Arquivo]</td> 
   <td>Adicione a ID do arquivo ou arquivos a partir dos quais deseja criar uma prova ou provas.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Nomes de Arquivos]</td> 
   <td>Adicione o nome do arquivo ou nomes para a prova criada. Este campo é obrigatório.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Bloquear prova quando todas as decisões necessárias forem tomadas]</td> 
   <td>Especifique se deseja que a prova criada seja bloqueada depois que todas as decisões necessárias forem tomadas.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Notificar recipients sobre esta prova]</td> 
   <td>Selecione uma opção para indicar se deseja que os recipients sejam notificados quando a prova for criada.&gt;</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome da prova]</td> 
   <td>Digite um nome para a prova criada. Este campo é obrigatório. Use um símbolo de barra vertical (|) para separar nomes para várias provas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do proprietário da prova]</td> 
   <td>Insira ou mapeie a ID do proprietário da prova. Se esse campo ficar em branco, o proprietário da prova será definido como o usuário atual.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Referência]</td> 
   <td>Insira a ID de referência da prova.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Requer assinatura eletrônica]</td> 
   <td>Selecione se você deseja que uma pessoa que toma uma decisão sobre uma prova envie uma assinatura eletrônica.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Exigir logon]</td> 
   <td> <p>Especifique se deseja que a prova criada exija um logon. </p> <p>Isso é o mesmo que a configuração [!UICONTROL Logon Necessário] explicada em <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Definir Configurações de Prova] em [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID de Resolução]</td> 
   <td>Insira a ID da resolução que deseja usar para a prova. Para obter uma lista de IDs de resolução, consulte a [!DNL Workfront Proof] <a href="https://api.proofhq.com/home/objects/soapworkflowproofobject.html">documentação da API</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL SWF]</td> 
   <td>Insira o tipo de prova de SWF.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Mostrar] [item]</td> 
   <td>Para cada item, selecione se deseja mostrá-lo na prova.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Workspace ID]</td> 
   <td>Digite a ID do espaço de trabalho no qual deseja criar a prova. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Destinatários]</td> 
   <td>Adicione os endereços de email dos destinatários que deseja para a prova criada.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Prazo]</td> 
   <td> <p>Especifique o prazo desejado para a prova criada. Use o seguinte formato de data:</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Chamada de API personalizada]

Este módulo de ação permite fazer uma chamada autenticada personalizada para a API [!DNL Workfront Proof]. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pelos outros módulos do [!DNL Workfront Proof].

O módulo retorna o código de status, os cabeçalhos e o corpo. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Workfront Proof] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Método]</td> 
   <td>Defina a ação para a chamada de API. Para ver as ações disponíveis, consulte a <a href="https://api.proofhq.com/">documentação da API de prova</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Corpo (XML)]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar instruções condicionais como <code>if</code> em seu JSON, coloque as aspas fora da instrução condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemplo:**
>
>![](assets/wfp-api-module-example-350x586.png)

#### [!UICONTROL Baixar Prova]

Esse módulo de ação baixa o arquivo de origem de uma prova específica que você identifica usando sua ID.

Especifique a ID da prova.

O módulo retorna o conteúdo do arquivo de origem usado para criar a prova. Você pode mapear essas informações nos módulos subsequentes no cenário.

Você deve ter permissões suficientes para acessar o registro em [!DNL Workfront Proof] para recuperar essas informações.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Workfront Proof] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID da Prova]</td> 
   <td> <p>Digite o identificador exclusivo da prova, encontrado na página [!UICONTROL Detalhes da Prova]. Para obter mais informações, consulte <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Gerenciar detalhes da prova em [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ler um Registro]

Este módulo de ação lê os dados de uma única prova no [!DNL Workfront Proof].

Especifique a ID da prova e as informações que deseja obter da prova.

O módulo retorna os valores dos campos escolhidos para a prova, juntamente com seus tipos. Você pode mapear essas informações em módulos subsequentes no cenário.

Você deve ter permissões suficientes para acessar o registro em [!DNL Workfront Proof] para recuperar essas informações.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Workfront Proof] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Registro]</td> 
   <td>Selecione se deseja ler uma prova, comentários de prova ou revisores de prova.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Saídas]</td> 
   <td> <p>Selecione as informações que deseja incluir no pacote de saída deste módulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Insira ou mapeie a ID [!DNL Workfront Proof] exclusiva do registro que você deseja que o módulo leia.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Solicitar Resumo de PDF]

Este módulo de ação solicita o resumo de PDF para uma prova específica em [!DNL Workfront Proof].

Especifique a ID da prova.

O módulo retorna as informações de resumo do PDF. Você pode mapear essas informações em módulos subsequentes no cenário.

Você deve ter permissões suficientes para acessar o registro em [!DNL Workfront Proof] para recuperar essas informações.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Workfront Proof] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID da Prova]</td> 
   <td> <p>Digite o identificador exclusivo [!DNL Workfront Proof] da prova para a qual você deseja solicitar um resumo de PDF.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL URL de retorno]</td> 
   <td>Insira ou mapeie o URL para onde deseja que o resumo do PDF seja enviado.</td> 
  </tr> 
 </tbody> 
</table>

##### Possível erro

* **Erro**: &quot;[!UICONTROL Você não tem privilégio para executar esta solicitação. O estágio deve conter pelo menos um destinatário.]&quot;
* **Solução**: verifique se você não é o único atribuído aos estágios do fluxo de trabalho. Deve haver outro usuário atribuído aos estágios do fluxo de trabalho.

#### [!UICONTROL Atualizar Prova]

Este módulo de ação atualiza uma prova existente no [!DNL Workfront Proof].

Especifique a ID da prova, o tipo de registro e quais campos deseja incluir na saída.

O módulo retorna quaisquer campos padrão associados ao registro, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Você deve ter permissões suficientes para acessar o registro em [!DNL Workfront Proof] para recuperar essas informações.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Workfront Proof] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID da Prova]</td> 
   <td> <p>Digite o identificador exclusivo da prova, encontrado na página [!UICONTROL Detalhes da Prova]. Para obter mais informações, consulte <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Gerenciar detalhes da prova em [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Prazo]</td> 
   <td> <p>Especifique o prazo desejado para a prova criada. Use o seguinte formato de data:</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Notificações de email padrão para assinantes]</td> 
   <td>Selecione qual das seguintes configurações de notificação por email padrão você deseja usar para a prova criada.
    <ul>
     <li> [!UICONTROL Todos os novos comentários e respostas]</li>
     <li>[!UICONTROL Respostas aos meus comentários]</li>
     <li>[!UICONTROL Resumo diário]</li>
     <li> [!UICONTROL Resumo por hora]</li>
     <li> [!UICONTROL Somente Decisões]</li>
     <li> [!UICONTROL Desabilitado]</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Função Padrão]</td> 
   <td>Selecione a função padrão para a prova.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Desabilitar Email de Assinatura]</td> 
   <td>Selecione se deseja desabilitar o email de assinatura para esta prova.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Habilitar Assinaturas]</td> 
   <td>Selecione se as pessoas que não são participantes têm permissão para assinar a prova.<br>Se você selecionar esta opção, também poderá selecionar a [!UICONTROL Função Padrão] para assinantes, conforme descrito nesta tabela.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Habilitar Validação de Assinaturas]</td> 
   <td>Selecione se deseja habilitar a validação de email de assinatura. Se isso estiver ativado, o assinante deve clicar em um link em um email para acessar uma prova.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Habilitar URL da Equipe]</td> 
   <td>Selecione se deseja que a prova criada oculte ou mostre o URL da equipe.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Bloquear prova quando todas as decisões necessárias forem tomadas]</td> 
   <td>Especifique se deseja que a prova criada seja bloqueada depois que todas as decisões necessárias forem tomadas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mensagem]</td> 
   <td>Insira ou mapeie uma mensagem que você deseja acompanhar a prova.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID da Prova] </td> 
   <td>Insira ou mapeie a ID da prova que deseja atualizar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome da Prova]</td> 
   <td>Insira ou mapeie o nome da prova que deseja atualizar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Exigir logon]</td> 
   <td> <p>Especifique se deseja que a prova criada exija um logon. </p> <p>Isso é o mesmo que a configuração [!UICONTROL Logon Necessário] explicada em <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Definir Configurações de Prova] em [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mostrar Versões Como]</td> 
   <td>Selecione se deseja mostrar um link para outras versões desta prova.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assunto]</td> 
   <td>Insira ou mapeie o assunto da prova</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Carregar arquivo]

Este módulo de ação carrega um arquivo para usar com o módulo [!UICONTROL Criar Prova] em [!DNL Workfront Proof].

O módulo retorna uma ID de hash para o arquivo carregado. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Workfront Proof] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL arquivo Source]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Pesquisas

* [[!UICONTROL Listar Modelos de Fluxo de Trabalho]](#list-workflow-templates)
* [[!UICONTROL Pesquisa]](#search)

#### [!UICONTROL Listar Modelos de Fluxo de Trabalho]

Este módulo de pesquisa lista todos os templates de workflow disponíveis.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Workfront Proof] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Saídas]</td> 
   <td> <p>Selecione as informações que deseja incluir no pacote de saída deste módulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de modelos que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Pesquisa]

Este módulo de pesquisa procura registros em um objeto em [!DNL Workfront Proof] que correspondam à consulta de pesquisa especificada.

O módulo retorna a ID da prova se estiver procurando uma prova. Ou retorna as IDs de usuário, emails, nomes, posições e aliases de email dos destinatários, se estiver procurando destinatários. Você pode mapear essas informações nos módulos subsequentes do cenário.

Você deve ter permissões suficientes para acessar o registro em [!DNL Workfront Proof] para recuperar essas informações.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Workfront Proof] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Procurar</td> 
   <td> <p>Consulte [!UICONTROL ] selecionar o tipo de registro que deseja que o módulo procure.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Prova]</strong> </p> <p>Digite o nome da prova da prova que você deseja pesquisar.</p> </li> 
     <li> <p><strong>[!UICONTROL Destinatário]</strong> </p> <p>Insira o endereço de email do destinatário que deseja pesquisar.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Conjunto de Resultados]</td> 
   <td>Indique se o módulo pesquisará por <strong>[!UICONTROL Todos os Registros Correspondentes]</strong> ou somente por <strong>[!UICONTROL Primeiro Registro Correspondente]</strong>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Classificar por]</td> 
   <td>Selecione o campo pelo qual deseja classificar os resultados.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Direção de Classificação]</td> 
   <td> <p>Selecione se deseja classificar os resultados em ordem crescente ou decrescente.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listar Modelos de Fluxo de Trabalho]

Este módulo de pesquisa lista todos os templates de workflow disponíveis.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Workfront Proof] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Saídas]</td> 
   <td> <p>Selecione as informações que deseja incluir no pacote de saída deste módulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de modelos que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>
