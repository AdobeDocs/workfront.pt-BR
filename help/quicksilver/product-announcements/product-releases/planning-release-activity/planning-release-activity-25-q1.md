---
content-type: release-notes
title: Atividade de Versão do Adobe Workfront Planning para a Versão 25.1
description: Esta é a atividade de lançamento do produto Adobe Workfront Planning para o Primeiro Trimestre de 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: ef0b719c-6d2e-4d3e-9522-da6dbd71c248
source-git-commit: a6104204cae2a2d8fb021da254437008d55a43b6
workflow-type: tm+mt
source-wordcount: '2112'
ht-degree: 0%

---

# Atividade da versão do primeiro trimestre de 2025 para o Adobe Workfront Planning

Este artigo descreve os recursos que estão sendo lançados para o Workfront Planning durante a versão do Primeiro Trimestre de 2025.

<!--keep the sentence below for all future quarterly release pages-->

Para obter uma lista de todos os recursos lançados para o Adobe Workfront Planning, consulte [atividade de versão do Adobe Workfront Planning: índice do artigo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Agora os campos de conexão com ativos do Adobe Experience Manager são permitidos em formulários de solicitação

>[!NOTE]
>
>Versão de pré-visualização: 20 de dezembro de 2024; Versão de produção para todos os clientes: 16 de janeiro de 2025

Agora é possível adicionar campos de conexão com ativos AEM a um formulário de solicitação de tipo de registro no Workfront Planning.

Antes desse aprimoramento, esses tipos de campos não podiam ser adicionados aos formulários de solicitação.

Para obter informações, consulte [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Configuração de aprovações para solicitações do Workfront Planning

>[!NOTE]
>
>Versão de pré-visualização: 16 de dezembro de 2024; Versão de produção para todos os clientes: 16 de janeiro de 2025

Agora é possível associar uma aprovação a um formulário de solicitação do Workfront Planning. Você pode adicionar somente usuários como aprovadores de uma solicitação. Depois que a solicitação é enviada, ela é enviada primeiro a todos os aprovadores para aprovação antes de criar um registro.

Para obter informações, consulte [Adicionar uma aprovação a um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/add-approval-to-request-form.md).


## Notificações para envio de solicitação, aprovações e alterações de status

>[!NOTE]
>
>Versão de pré-visualização: 16 de dezembro de 2024; Versão de produção para todos os clientes: 16 de janeiro de 2025

Agora você receberá uma notificação no aplicativo, bem como um email, para as seguintes ações depois de enviar uma solicitação no Workfront Planning:

* Um solicitante recebe uma notificação de que uma solicitação foi enviada com êxito

* Um solicitante recebe uma notificação de que uma solicitação foi aprovada ou rejeitada

* Um aprovador recebe uma notificação de que uma solicitação foi enviada a ele para aprovação.

>[!NOTE]
>
>A instância da Workfront de sua organização deve ser integrada à Experiência unificada do Adobe para que os usuários possam receber notificações por email e no aplicativo.

Para obter informações sobre como enviar ou aprovar solicitações, consulte os seguintes artigos:

* [Enviar solicitações do Adobe Workfront Planning para criar registros](/help/quicksilver/planning/requests/submit-requests.md)

* [Aprovar uma solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/approve-request.md).

## Pesquisa inteligente ao procurar um tipo de campo

>[!NOTE]
>
>Versão de pré-visualização: 5 de dezembro de 2024; Versão de produção para todos os clientes: 5 de dezembro de 2024

Adicionamos a funcionalidade de pesquisa inteligente ao procurar um tipo de campo no Workfront Planning. Agora é possível encontrar tipos de campo ao digitar uma palavra-chave. Por exemplo, digitar &quot;Preço&quot; localiza os tipos de campo Número e Moeda. Antes dessa melhoria, você poderia pesquisar somente pelo nome do tipo de campo real.

Para obter informações, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

## Seletor de cores personalizado para opções codificadas por cores de campos de seleção única ou múltipla

>[!NOTE]
>
>Versão de pré-visualização: 5 de dezembro de 2024; Produção para lançamento rápido: Com lançamento do 24.12 (12 de dezembro de 2024); Produção para lançamento trimestral: Com lançamento do 25.1 (janeiro de 2025)

Agora, você pode fazer escolhas de cores personalizadas ao criar ou editar um campo de seleção única ou múltipla. Ao criar ou editar campos com opções codificadas por cores, clicar no ícone de cor abre uma caixa do seletor de cores. Você pode escolher entre cores predefinidas ou criar cores personalizadas usando códigos hexadecimais ou um espectro de cores.

Para obter informações, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

## Importar campos existentes do Workfront para tipos de registro do Workfront Planning

>[!NOTE]
>
>Versão de pré-visualização: 27 de novembro de 2024; Produção para lançamento rápido: Com o lançamento 24.12 (12 de dezembro de 2024); Produção para lançamento trimestral: Com o lançamento 25.1 (janeiro de 2025)

Agora, ao adicionar campos a um tipo de registro, você tem a opção de importar campos personalizados ou nativos existentes do Workfront e associá-los ao tipo de registro selecionado. A importação de campos existentes cria uma cópia dos campos do Workfront no Workfront Planning. Os campos copiados são independentes das versões originais.

Antes desse aprimoramento, era necessário criar manualmente todos os campos e associá-los aos tipos de registro.

Os campos calculados não são compatíveis no momento.

Para obter informações, consulte [Importar campos do Adobe Workfront](/help/quicksilver/planning/fields/import-fields-from-workfront.md)

## Criar tipos de registro, registros e campos importando um arquivo CSV ou do Excel

>[!NOTE]
>
>Versão de pré-visualização: 27 de novembro de 2024; Produção para lançamento rápido: Com o lançamento 24.12 (12 de dezembro de 2024); Produção para lançamento trimestral: Com o lançamento 25.1 (janeiro de 2025)

Agora é possível importar novos tipos de registro importando um arquivo CSV ou do Excel.

As seguintes informações são importadas:

* O nome da planilha ou do arquivo é importado como o nome do tipo de registro.

* A primeira linha de cada coluna é importada como um novo campo. É possível ter até 500 campos em cada planilha importada.

* Cada linha é importada como um novo registro. Você pode ter até 10.000 registros em cada planilha.

Para obter mais informações, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

## Evitar referências circulares em fórmulas

>[!NOTE]
>
>Versão de pré-visualização: 27 de novembro de 2024; Produção para lançamento rápido: Com o lançamento 24.12 (12 de dezembro de 2024); Produção para lançamento trimestral: Com o lançamento 25.1 (janeiro de 2025)

Introduzimos uma mensagem de aviso ao editar ou criar um campo de fórmula que pode criar uma referência circular a si mesmo ou campos compartilhados. Não é possível salvar um campo de fórmula que faça referência a ele mesmo ou a itens referenciados em seu cálculo.

Para obter informações, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

## Adicionar páginas de exibição de conexão à página de um registro para exibir registros conectados em uma exibição de tabela

>[!NOTE]
>
>Versão de pré-visualização: 27 de novembro de 2024; Produção para lançamento rápido: Com o lançamento 24.12 (12 de dezembro de 2024); Produção para lançamento trimestral: Com o lançamento 25.1 (janeiro de 2025)

É possível adicionar páginas à área de detalhes de um registro para exibir registros conectados em uma exibição de tabela. É possível adicionar uma página por registro conectado.

As páginas adicionadas são somente leitura.

Para obter informações, consulte [Gerenciar o layout da página de registro](/help/quicksilver/planning/records/manage-the-record-page.md).

## Novas guias Workfront e Planejamento na seção Enviado da área Solicitações

>[!NOTE]
>
>Versão de pré-visualização: 27 de novembro de 2024; Produção para lançamento rápido: Com o lançamento 24.12 (12 de dezembro de 2024); Produção para lançamento trimestral: Com o lançamento 25.1 (janeiro de 2025)

Agora é possível encontrar solicitações do Workfront Planning na seção Enviado da área Solicitações do Workfront. A seção Enviado agora exibe as seguintes guias:

* Workfront: exibe solicitações enviadas no Workfront.
* Planning: exibe solicitações enviadas usando um formulário de solicitação do Workfront Planning.

Você deve usar um link para o formulário de solicitação para poder adicionar solicitações a um tipo de registro do Workfront Planning. A submissão de uma solicitação do Workfront Planning a partir da área Solicitações do Workfront estará disponível em uma data posterior.

Sua organização deve comprar um pacote do Workfront Planning antes que a guia Planejamento esteja disponível na área Solicitações.

Para obter informações, consulte [Enviar solicitações do Adobe Workfront Planning para criar registros](/help/quicksilver/planning/requests/submit-requests.md).

## Tipos de campos adicionais agora são aceitos em formulários de solicitação

>[!NOTE]
>
>Versão de pré-visualização: 27 de novembro de 2024; Produção para lançamento rápido: Com o lançamento 24.12 (12 de dezembro de 2024); Produção para lançamento trimestral: Com o lançamento 25.1 (janeiro de 2025)

Agora é possível adicionar os seguintes tipos de campo a um formulário de solicitação de tipo de registro no Workfront Planning:

* Pessoas
* Conexões do Workfront

Antes desse aprimoramento, esses tipos de campos não podiam ser adicionados a formulários de solicitação no Workfront Planning.

Para obter informações, consulte [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Limitar o compartilhamento público de formulários de solicitação que contêm determinados tipos de campo

>[!NOTE]
>
>Versão de pré-visualização: 27 de novembro de 2024; Produção para lançamento rápido: Com o lançamento 24.12 (12 de dezembro de 2024); Produção para lançamento trimestral: Com o lançamento 25.1 (janeiro de 2025)

Não é mais possível compartilhar um formulário de solicitação publicamente se ele contiver qualquer um dos seguintes tipos de campo:

* Fórmula
* Conexões do Workfront e do AEM Assets
* Campos de pesquisa
* Pessoas

Para obter informações, consulte [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).


## Exibir registros na exibição de calendário por semana

>[!NOTE]
>
>Versão de pré-visualização: 26 de novembro de 2024; Produção para lançamento rápido: Com o lançamento 24.12 (12 de dezembro de 2024); Produção para lançamento trimestral: Com o lançamento 25.1 (janeiro de 2025)

Agora é possível exibir registros na exibição de calendário por semana. Antes dessa melhoria, você poderia exibir a exibição do calendário somente por mês.

Para obter informações, consulte [Gerenciar a exibição de calendário](/help/quicksilver/planning/views/manage-the-calendar-view.md).

## Restaurar registros excluídos

>[!NOTE]
>
>Versão de pré-visualização: 22 de novembro de 2024; Produção para lançamento rápido: Com o lançamento 24.12 (12 de dezembro de 2024); Produção para lançamento trimestral: Com o lançamento 25.1 (janeiro de 2025)

Após a exclusão dos registros, eles agora são movidos temporariamente para um compartimento Excluído recentemente por 30 dias. Você pode acessar o compartimento Recentemente excluído na página do tipo de registro e ele contém apenas registros de um tipo específico.

Os gerentes do Workspace podem restaurar registros do lixo por até 30 dias após a exclusão. Os registros conectados e suas informações de campo também são restaurados.

Antes desse aprimoramento, não era possível restaurar os registros excluídos.

Para obter mais informações, consulte [Restaurar registros excluídos](/help/quicksilver/planning/records/records-information.md).

## Assistente de IA de Adobe disponível nas áreas de detalhes de registro

>[!NOTE]
>
>Versão de pré-visualização: 21 de novembro de 2024; Produção para lançamento rápido: Com o lançamento 24.12 (12 de dezembro de 2024); Produção para lançamento trimestral: Com o lançamento 25.1 (janeiro de 2025)

Para facilitar a realização do trabalho, adicionamos o Assistente de IA de Adobe à visualização dos detalhes de um registro ou à página do registro. Você pode usar o Assistente de IA dentro de uma página de registro para atualizar informações sobre o registro.

Para obter informações, consulte [visão geral do Assistente de IA do Adobe Workfront Planning](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

## Nova experiência ao adicionar uma miniatura e uma imagem de capa a uma página de registro

>[!NOTE]
>
>Versão de pré-visualização: 20 de novembro de 2024; Produção para lançamento rápido: Com o lançamento 24.12 (12 de dezembro de 2024); Produção para lançamento trimestral: Com o lançamento 25.1 (janeiro de 2025)

Ao abrir uma visualização ou página de registro e o registro não tiver uma miniatura ou uma imagem de capa, passe o mouse sobre a área acima do nome do registro no cabeçalho para ver as opções de adição de uma capa e uma imagem de miniatura ao registro. Antes dessa melhoria, as imagens vazias de espaço reservado para a miniatura e a capa são exibidas acima do nome do registro.

Para obter mais informações, consulte os seguintes artigos:

* [Adicionar uma imagem da capa a um registro](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
* [Adicionar uma imagem em miniatura a um registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

## Novos tipos de exibição para campos do tipo porcentagem na exibição de tabela

>[!NOTE]
>
>Versão de pré-visualização: 7 de novembro de 2024; Produção para lançamento rápido: Com lançamento do 24.12 (12 de dezembro de 2024); Produção para lançamento trimestral: Com lançamento do 25.1 (janeiro de 2025)

Para facilitar a leitura dos números na exibição de tabela, agora é possível selecionar entre as seguintes opções para alterar a forma como um campo do tipo Porcentagem é exibido na exibição de tabela:

* Número
* Barra
* Círculo

Esse tipo de exibição é compatível somente na exibição de tabela.

Antes dessa melhoria, você poderia exibir valores percentuais somente como números.

Para obter mais informações, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

## Agora os campos de conexão são aceitos em formulários de solicitação

>[!NOTE]
>
>Versão de pré-visualização: 31 de outubro de 2024; Produção para lançamento rápido: Com o lançamento do 24.11 (14 de novembro de 2024); Produção para lançamento trimestral: Com o lançamento do 25.1 (janeiro de 2025)

Agora é possível adicionar campos conectados para registros do Workfront Planning a um formulário de solicitação de tipo de registro.

Não é possível adicionar campos de pesquisa de conexão ou campos conectados para objetos Workfront no formulário de solicitação.

Antes desse aprimoramento, esses tipos de campos não podiam ser adicionados a formulários de solicitação no Workfront Planning.

Para obter informações, consulte [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Aviso de conexão ao conectar registros que já estão vinculados a outros registros

>[!NOTE]
>
>Versão de pré-visualização: 31 de outubro de 2024; Produção para lançamento rápido: Com o lançamento do 24.11 (14 de novembro de 2024); Produção para lançamento trimestral: Com o lançamento do 25.1 (janeiro de 2025)

Ao tentar conectar registros que já estão conectados em outro lugar e que pertencem a um tipo de registro conectado por meio de um tipo de conexão Um para muitos ou Um para um, agora você recebe um aviso de que os registros já estão conectados. Se você confirmar que deseja prosseguir com a conexão, os registros selecionados serão removidos do registro original e adicionados ao registro que você está editando no momento.

Para obter informações sobre tipos de conexão, consulte [Visão geral dos tipos de registro conectados](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Ícone Novas informações com a descrição dos campos na página de detalhes do registro

>[!NOTE]
>
>Versão de pré-visualização: 30 de outubro de 2024; Produção para lançamento rápido: Com o lançamento do 24.11 (14 de novembro de 2024); Produção para lançamento trimestral: Com o lançamento do 25.1 (janeiro de 2025)

Adicionamos um ícone de informações à direita dos nomes de campo em uma página de registro. Clicar no ícone de informações exibe a descrição do campo, quando existe uma descrição. Antes dessa melhoria, a descrição do campo era exibida quando você passava o mouse sobre o nome do campo.

Para obter informações, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

## Novo tipo de campo do Workfront para conexões do Planning

>[!NOTE]
>
>Versão de pré-visualização: 24 de outubro de 2024; Produção para lançamento rápido: Com o lançamento do 24.11 (14 de novembro de 2024); Produção para lançamento trimestral: Com o lançamento do 25.1 (janeiro de 2025)

Para continuar unindo objetos do Workfront aos registros do Workfront Planning, adicionamos um novo tipo de campo nos formulários personalizados do Workfront chamado Conexão do Planning. Ao adicionar esse tipo de campo em um formulário personalizado do Workfront e, por fim, em um objeto do Workfront, agora é possível fazer o seguinte:

* Exibir registros conectados a um objeto do Workfront no formulário personalizado.

* Conectar e desconectar registros do Workfront Planning de um objeto do Workfront.

Você pode adicionar o novo campo a formulários para todos os tipos de objeto. No entanto, você pode editar as informações no campo somente a partir de formulários anexados aos seguintes objetos do Workfront que podem ser conectados a partir dos tipos de registro do Workfront Planning: Portfolio, Programa, Projeto, Empresa, Grupo.

A edição de campos de conexão do Planning para objetos do Workfront em massa ainda não está disponível.

Para obter informações, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

[Exibir uma demonstração em vídeo deste recurso](https://video.tv.adobe.com/v/3435633/){target=_blank}
