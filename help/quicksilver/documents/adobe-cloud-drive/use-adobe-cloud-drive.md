---
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: Usar o Adobe Cloud Drive
description: Trabalhe com seus projetos de armazenamento em nuvem da Adobe diretamente do Localizador ou do Explorador de arquivos usando o Adobe Cloud Drive. Abra e edite arquivos em qualquer aplicativo, trabalhe offline e resolva conflitos.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: c16dc2b8b508f71767999aec7029664f5d31f23f
workflow-type: tm+mt
source-wordcount: '3955'
ht-degree: 1%
---
# Usar o Adobe Cloud Drive

Depois de instalar o Adobe Cloud Drive, você pode trabalhar com seus projetos de armazenamento em nuvem da Adobe diretamente do Localizador ou do Explorador de arquivos. Você pode abrir e editar arquivos em qualquer aplicativo, trabalhar offline e permitir que o Adobe Cloud Drive sincronize suas alterações na nuvem.

Para obter informações sobre como instalar o Adobe Cloud Drive, consulte [Instalar o Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Versão do Adobe Workfront</td> 
   <td>Ultimate de fluxo de trabalho, com o Adobe Cloud Storage ativado</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>
      <p>Visualizar o acesso a um projeto para vê-lo no Adobe Cloud Drive</p>
      <p>Editar o acesso a um projeto para adicionar, editar ou excluir arquivos nele</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Acessar os projetos

1. Abra o Localizador (Mac) ou o Explorador de Arquivos (Windows).
1. Navegue até **Adobe Cloud Drive**.
1. Navegue na lista de projetos aos quais você tem acesso no Workfront. Abra qualquer pasta do projeto para visualizar seus arquivos e subpastas.

   >[!NOTE]
   >
   >* As pastas do projeto são somente leitura no nível superior. Não é possível renomear, excluir ou mover as próprias pastas do projeto.
   >* Você pode trabalhar com arquivos e pastas dentro de uma pasta de projeto — abrir, editar, criar, excluir e assim por diante.
   >* Os projetos herdados do Workfront não aparecem no Adobe Cloud Drive. Somente projetos armazenados no armazenamento em nuvem do Adobe estão disponíveis.

## Indicadores de status de arquivo

O Adobe Cloud Drive usa indicadores visuais para mostrar o status de sincronização de arquivos. Os ícones diferem entre Windows e Mac.

### Indicadores de status de arquivo no Windows

| Ícone | Status | Significado do arquivo | Significado da pasta |
| --- | --- | --- | --- |
| ![Ícone somente online](assets/acd-windows-online-only.png) | Somente online | O arquivo está sincronizado, mas só está disponível online. | Todos os arquivos dentro de estão disponíveis online. |
| ![Ícone de sincronização](assets/acd-windows-syncing.png) | Sincronizando | As atualizações mais recentes do arquivo estão sendo sincronizadas com o cache local ou com o armazenamento em nuvem do Adobe. | Pelo menos um arquivo na pasta está sendo sincronizado. |
| ![Ícone offline disponível](assets/acd-windows-available-offline.png) | Disponível offline | O arquivo foi sincronizado e está disponível offline. | Pelo menos um arquivo da pasta está disponível offline. |
| ![Ícone fixado](assets/acd-windows-pinned.png) | Fixado (Sempre Manter no Dispositivo) | O arquivo é sincronizado e sempre mantido offline. O Adobe Cloud Drive não limpa o conteúdo fixado automaticamente. | Todos os arquivos da pasta estão no cache local e disponíveis offline. |
| ![Ícone somente leitura](assets/acd-windows-read-only.png) | Somente leitura | O arquivo é somente leitura. | A pasta é somente leitura. |
| ![Ícone de erro de sincronização](assets/acd-windows-sync-error.png) | Erro de sincronização | O arquivo não pode ser sincronizado. Passe o mouse sobre o ícone para obter detalhes. | A pasta não pode ser sincronizada. Passe o mouse sobre o ícone para obter detalhes. |
| ![Ícone Sincronizar excluído](assets/acd-windows-sync-excluded.png) | Sincronização excluída | O arquivo não pode ser sincronizado devido a um tipo ou nome sem suporte. | A pasta não pode ser sincronizada devido a um nome sem suporte. |

### Indicadores de status de arquivo no Mac

| Ícone | Status | Significado do arquivo | Significado da pasta |
| --- | --- | --- | --- |
| (Nenhum ícone) | Disponível offline | O arquivo foi sincronizado e está disponível offline. | Todos os arquivos estão disponíveis offline. |
| ![Ícone somente online](assets/acd-mac-online-only.png) | Somente online | O arquivo está sincronizado e disponível somente online. | Pelo menos um arquivo da pasta está online. |
| ![Ícone de sincronização](assets/acd-mac-syncing.png) | Sincronizando | As atualizações mais recentes do arquivo estão sendo sincronizadas com o cache local ou com o armazenamento em nuvem do Adobe. | O conteúdo da pasta está sendo sincronizado. |
| ![Ícone de erro de sincronização](assets/acd-windows-sync-error.png) | Erro de sincronização | O arquivo não pode ser atualizado ou sincronizado. Passe o mouse sobre o ícone para obter detalhes. | A pasta não pode ser atualizada ou sincronizada. Passe o mouse sobre o ícone para obter detalhes. |
| ![Ícone Sincronizar excluído](assets/acd-windows-sync-excluded.png) | Sincronização excluída | Arquivo excluído da sincronização. | A pasta foi excluída da sincronização. |
| ![Ícone somente leitura](assets/acd-mac-read-only.png) | Somente leitura | O arquivo é somente leitura. | A pasta é somente leitura. |
| ![Ícone fixado](assets/acd-windows-pinned.png) | Fixado (Sempre Manter no Dispositivo) | O arquivo está fixado para ficar disponível offline. O Adobe Cloud Drive não limpa o conteúdo fixado automaticamente. | A pasta está fixada para estar disponível offline. |

### Dicas de ferramenta de erro

Quando ocorrer um erro de sincronização ou um problema, passe o mouse sobre o ícone do arquivo ou da pasta para ver uma dica de ferramenta que descreve o problema.

| Categoria de erro | Dica de ferramenta | Significado |
|---|---|---|
| Sincronização excluída | Tipo de arquivo incompatível | O tipo de arquivo não é compatível com o Adobe Cloud Drive. |
| Sincronização excluída | Nome de arquivo não suportado | O nome do arquivo não é compatível com o Adobe Cloud Drive. |
| Sincronização excluída | Projeto primário excluído | O projeto pai do Workfront foi excluído. |
| Sincronização suspensa | Conteúdo de arquivo não suportado | O conteúdo do arquivo não pode ser sincronizado (por exemplo, um problema de segurança foi detectado). |
| Sincronização suspensa | Caracteres inválidos no nome do arquivo | O nome do arquivo contém caracteres inválidos. |
| Sincronização suspensa | Caminho completo muito longo | O caminho do arquivo excede o comprimento máximo permitido. |
| Sincronização suspensa | Sem permissão de gravação | Seu acesso de gravação a este arquivo ou projeto foi revogado. |
| Erro de sincronização | Problema de autenticação | Há um problema com suas credenciais de entrada. |
| Erro de sincronização | Armazenamento na nuvem indisponível | Os serviços em nuvem do Adobe estão temporariamente indisponíveis. |
| Erro de sincronização | Armazenamento na nuvem cheio | A cota de armazenamento na nuvem está cheia. |
| Erro de sincronização | Disco local cheio | O disco local não tem espaço livre suficiente. |
| Erro de sincronização | Sem conexão com a Internet | Seu dispositivo não está conectado à Internet. |
| Erro de sincronização | Erro inesperado | Ocorreu um erro inesperado durante a sincronização. |
| Erro de sincronização | Conta bloqueada | Sua conta foi bloqueada pelo serviço. |

>[!NOTE]
>
>Erros no nível do sistema — como desconectado, falha de autenticação, rede indisponível, disco local cheio ou armazenamento na nuvem cheio — são mostrados na bandeja do sistema (Windows) ou na barra de menu (Mac), não em arquivos individuais.

### Sincronizar lista de exclusão

O Adobe Cloud Drive exclui determinados arquivos gerados pelo sistema, temporários e bloqueados da sincronização. Os seguintes tipos de arquivos e padrões são excluídos:

| Categoria | Tipos/padrões de arquivos | Descrição |
|---|---|---|
| Arquivos do sistema | `.DS_Store`, `Thumbs.db` | Metadados do sistema operacional e arquivos de cache de miniaturas. |
| Arquivos de memória virtual e do sistema | `*.sys` (por exemplo, `hiberfil.sys`, `pagefile.sys`, `swapfile.sys`) | Grandes arquivos do sistema usados para memória virtual, hibernação ou outras funções do sistema operacional. |
| Arquivos de indexação do macOS | `.Spotlight-V100`, `.fseventsd` | Arquivos de indexação e rastreamento de eventos do sistema de arquivos do macOS Spotlight. |
| Arquivos temporários e de backup | `*.tmp`, `*.swp`, `*~`, `*.bak` | Arquivos temporários, transitórios ou de backup gerados por aplicativos. |

## Abrir um arquivo

1. No Adobe Cloud Drive, navegue até o arquivo.
1. Clique duas vezes no arquivo.

   O arquivo é aberto no aplicativo padrão.

O Adobe Cloud Drive é compatível com qualquer tipo de arquivo que um aplicativo instalado em seu computador possa abrir, incluindo:

* Formatos do Adobe Creative Cloud (PSD, AI, INDD, PROJ, AEP e assim por diante)
* Documentos do Microsoft Office (DOCX, XLSX, PPTX)
* Imagens (JPG, PNG, GIF e assim por diante)
* Arquivos de vídeo (MP4, MOV e assim por diante)

>[!NOTE]
>
>Os formatos de documento da nuvem (PSDC, AIDC e assim por diante) são abertos como seus equivalentes padrão (PSD, AI e assim por diante) quando você os acessa pelo Adobe Cloud Drive.

## Editar e salvar um arquivo

1. Abra um arquivo no Adobe Cloud Drive.
1. Faça as alterações no aplicativo.
1. Salve o arquivo selecionando **Arquivo** > **Salvar** ou pressionando Ctrl+S (Windows) ou Cmd+S (Mac).

   Suas alterações são sincronizadas automaticamente com o armazenamento em nuvem do Adobe.

>[!IMPORTANT]
>
>Salve os arquivos usando **Arquivo** > **Salvar** ou o atalho de teclado. Evite usar **Salvar como** para criar cópias, pois ele gera arquivos duplicados na unidade.

## Criar ou adicionar um novo arquivo

Você pode criar um novo arquivo diretamente em um projeto ou adicionar um arquivo existente do armazenamento local.

### Criar um novo arquivo a partir de um aplicativo

1. Abra o aplicativo que deseja usar para criar o arquivo.
1. Crie o arquivo normalmente.
1. Ao salvar, escolha um local dentro de uma pasta do projeto do Adobe Cloud Drive.

   O arquivo aparece no Adobe Cloud Drive e é sincronizado com o armazenamento na nuvem da Adobe.

### Adicionar um arquivo existente a um projeto

1. No Localizador (Mac) ou no Explorador de arquivos (Windows), abra a pasta do projeto no Adobe Cloud Drive.
1. Arraste ou copie arquivos do armazenamento local para a pasta do projeto.

   Os arquivos são sincronizados automaticamente com o armazenamento em nuvem do Adobe.

## Disponibilizar arquivos e pastas offline

Quando um arquivo ou pasta está disponível offline, você pode abri-lo e editá-lo sem uma conexão com a Internet. Arquivos offline usam espaço em disco local.

### Manter um arquivo ou pasta no dispositivo

1. Clique com o botão direito do mouse no arquivo ou pasta no Adobe Cloud Drive.
1. Selecione **Sempre Manter Neste Dispositivo**.

   O arquivo ou pasta é baixado para o cache local e você pode trabalhar com ele mesmo quando estiver offline.

### Remova o acesso offline para liberar espaço

1. Clique com o botão direito do mouse no arquivo ou pasta offline.
1. Selecione **Liberar Espaço**.

   O arquivo ou pasta permanece no armazenamento na nuvem, mas é removido do cache local.

>[!NOTE]
>
>Arquivos e pastas offline usam o espaço em disco local. Remova o acesso off-line para arquivos e pastas de que você não precisa mais liberar espaço.

## Copiar um arquivo para o armazenamento local

Você pode copiar um arquivo do Adobe Cloud Drive para a unidade local. O original permanece no Adobe Cloud Drive e a cópia se torna um arquivo local independente.

1. Clique com o botão direito do mouse no arquivo no Adobe Cloud Drive.
1. Selecione **Copiar** e cole o arquivo no local na unidade local onde você deseja que ele esteja.

   O arquivo copia para o destino. O original permanece no Adobe Cloud Drive.

>[!NOTE]
>
>Os arquivos copiados para o armazenamento local são cópias independentes. As alterações feitas em uma cópia local não são sincronizadas com o armazenamento na nuvem da Adobe.

<!-- Courtney check me: New sections below (Upload to Cloud through Open in Workfront) added for Adobe Cloud Drive v1.2.0, per helpxNewFeature.pdf from Pulkit Goel. Verify content, placement, and heading order. -->

## Fazer upload de arquivos para a nuvem (Upload direto) {#direct-upload}

<!-- Courtney check me: Source PDF calls this "Upload to Cloud (Direct Upload)". Confirm heading wording. -->

O Upload direto envia arquivos do seu computador diretamente para o armazenamento na nuvem da Adobe, sem primeiro copiá-los na pasta do Adobe Cloud Drive.

<!-- Courtney check me: Removed folder mentions from the Direct Upload section (intro, heading, step 1, 500-file bullet, hidden files bullet, and the Sync Activity link text), per Pulkit: folder support isn't available yet. Confirm nothing else should change. -->

### Fazer upload de arquivos

1. Clique com o botão direito do mouse em um arquivo no Finder (Mac) ou no Explorador de Arquivos (Windows).
1. Selecione **Carregar para a nuvem**.
1. No seletor de destino, selecione um local em um dos projetos no Adobe Cloud Drive e clique **Fazer upload aqui**.
1. Monitore o progresso na seção **Upload Direto** da janela Sincronizar Atividade.

### O que você deve saber sobre o upload direto

* O carregamento direto copia o item para a nuvem. O item original permanece no local atual.
* Você pode selecionar vários itens para fazer upload de uma só vez.
* A seção Upload direto lista somente arquivos individuais, até um máximo de 500.
* Você pode fazer upload de itens do seu diretório inicial de usuário ou de qualquer unidade externa anexada. Outros locais de armazenamento na nuvem, como o iCloud Drive ou `~/Library/CloudStorage`, não têm suporte.
* Você deve estar conectado com uma conta da Adobe qualificada. Você não precisa de uma conexão com a Internet para iniciar um upload. Sem uma conexão, os uploads permanecem na fila.
* Pausar a sincronização cancela os uploads que estão em andamento. Os uploads enfileirados são retomados automaticamente quando você retoma a sincronização.
* Se você sair do Adobe Cloud Drive durante um upload, os uploads em andamento serão marcados como cancelados. Os uploads em fila são retomados automaticamente ao reiniciar o aplicativo.
* Arquivos ocultos, links simbólicos e aliases não são compatíveis.
* O Adobe Cloud Drive controla quantos uploads são executados ao mesmo tempo. Os uploads restantes permanecem na fila até que um slot se torne disponível.
* Uma contagem ativa de uploads, incluindo uploads com falha, é exibida. Por exemplo, &quot;3 arquivos de upload&quot;. Quando todos os uploads são concluídos com êxito, a contagem é alterada para um resumo, como &quot;3 arquivos carregados&quot;. Selecione **Dispensar** para removê-lo.

<!-- Courtney check me: "Pausing sync cancels uploads in progress" and the quit behavior are from the PDF. Confirm with dev that both are intended. -->

### Status do upload

<!-- Courtney check me: Icons extracted from the PDF (48x48 px, low resolution) and named by table order. Verify each icon matches its status and ask Pulkit's team for higher-resolution originals. Add alt text review too. -->

| Ícone | Status | Descrição | Ações disponíveis |
| --- | --- | --- | --- |
| ![Ícone na fila](assets/acd-upload-status-queued.png) | Na fila | O upload está aguardando para ser iniciado. | **Cancelar** cancela este item. |
| ![Carregando ícone](assets/acd-upload-status-uploading.png) | Fazendo upload | O upload está em andamento. | **Cancelar** cancela este item. |
| ![Ícone Concluído](assets/acd-upload-status-completed.png) | Concluídos | O upload foi concluído com sucesso. | **Abrir no Workfront** abre o ativo na interface da Web do Workfront. |
| ![Ícone de falha](assets/acd-upload-status-failed.png) | Falhou | O upload não pôde ser concluído. | **Mostrar arquivo de origem** revela o arquivo original. **Repetir** repete o carregamento. A opção Repetir está disponível somente para determinadas falhas. |
| ![Ícone de cancelado](assets/acd-upload-status-cancelled.png) | Cancelado | O upload foi interrompido por você ou pelo sistema. | Nenhum. Os uploads cancelados não são repetidos. Você deve iniciar um novo upload. |

Para ver o motivo de uma falha, passe o mouse sobre o item com falha.

### Gerenciar a lista de uploads

Cada ação está disponível somente quando se aplica.

* **Cancelar todos os carregamentos:** Disponível quando os carregamentos estão na fila ou em andamento. Cancela todos eles.
* **Repetir uploads com falha:** Disponível quando há uploads com falha que podem ser repetidos. Tenta novamente todos eles. Os uploads que não podem ser repetidos permanecem inalterados.
* **Limpar:** Disponível quando nenhum carregamento está na fila ou em andamento. Remove todos os itens concluídos, com falha e cancelados. Os arquivos locais e o conteúdo já carregado não são afetados.
* **Limpeza automática:** itens concluídos, com falha e cancelados são removidos automaticamente 24 horas após sua última atualização. Os itens em fila e em andamento nunca são removidos automaticamente.

## Pausar e retomar sincronização {#pause-resume-sync}

Você pode pausar o Adobe Cloud Drive quando não quiser que ele carregue ou baixe arquivos, por exemplo, em uma conexão de Internet lenta ou limitada. Enquanto a sincronização estiver pausada, suas alterações não serão enviadas para a nuvem e as alterações da nuvem não serão baixadas para o computador. A sincronização permanece pausada até que você a retome.

### Pausar sincronização

1. Clique no ícone do Adobe Cloud Drive na bandeja do sistema (Windows) ou na barra de menus (Mac).
1. Clique no ícone **Menu** ( ✔) no canto superior direito da janela Adobe Cloud Drive.
1. Selecione **Pausar sincronização**.

   >[!TIP]
   >
   >Com a janela do Adobe Cloud Drive aberta, você também pode pressionar Ctrl+P (Windows) ou Command+P (Mac).

   A janela Unidade de Nuvem do Adobe mostra **Sincronização pausada** e a mensagem **Arquivos não serão sincronizados até que você retome**. Ao passar o mouse sobre o ícone do Adobe Cloud Drive, ele mostra **Adobe Cloud Drive (Pausado)**.

>[!NOTE]
>
>A sincronização de pausa está disponível somente quando você está conectado e o Adobe Cloud Drive está conectado.

### Retomar sincronização

1. Clique no ícone do Adobe Cloud Drive na bandeja do sistema (Windows) ou na barra de menus (Mac).
1. Siga um destes procedimentos:

   * Clique em **Retomar**.
   * Clique no ícone **Menu** ( ✔) e selecione **Retomar sincronização**. Com a janela aberta, você também pode pressionar Ctrl+R (Windows) ou Command+R (Mac).

   O Adobe Cloud Drive inicia a sincronização novamente, incluindo todas as alterações feitas enquanto a sincronização estava pausada.

## Exibir e gerenciar o histórico de versões {#version-history}

Você pode usar o Histórico de versões no Adobe Cloud Drive para procurar versões salvas da nuvem de um arquivo compatível, exibir detalhes e miniaturas de versão e reverter para uma versão anterior. Você também pode editar o nome e a descrição de uma versão se tiver as permissões necessárias.

### Exibir histórico de versões

1. Navegue até a pasta do Adobe Cloud Drive no Localizador ou no Explorador de arquivos.
1. Selecione um arquivo compatível.
1. Clique com o botão direito do mouse no arquivo e selecione **Histórico de Versões**.
1. Selecione uma versão para exibir os detalhes e a miniatura disponíveis.

   Se o arquivo não tiver versões anteriores, **Nenhuma versão anterior** será exibida. Miniaturas podem não estar disponíveis para todos os arquivos ou versões.

### Editar informações de versão

1. Abra o Histórico de versão do arquivo.
1. Selecione a versão que deseja atualizar.
1. Abra o menu de opções da versão e selecione **Editar informações da versão**.
1. Insira um **Nome da versão** ou **Descrição**.
1. Selecione **Salvar**.

   As informações atualizadas são salvas e exibidas ao reabrir o Histórico de versões.

### Reverter para uma versão anterior

1. Abra o Histórico de versão do arquivo.
1. Selecione a versão que deseja restaurar.
1. Selecione **Reverter para esta versão**, se disponível.
1. Aguarde a conclusão da sincronização.
1. Reabra o arquivo para verificar se o conteúdo da versão selecionada agora está atual.

## Gerenciar armazenamento local {#manage-local-storage}

Você pode usar Gerenciar Armazenamento Local no Adobe Cloud Drive para monitorar o uso do disco local, definir um limite de armazenamento e exibir arquivos marcados como **Sempre neste dispositivo**.

<!-- Courtney check me: PDF says "Always on this device" here but this article uses "Always Keep On This Device" for the right-click option. Confirm which label the UI shows in each place. -->

### Exibir uso de armazenamento local

1. Selecione o ícone do Adobe Cloud Drive e abra o menu de opções.
1. Selecione **Gerenciar Armazenamento Local**.
1. Revise o uso de armazenamento atual e a lista de arquivos marcados como **Sempre neste dispositivo**.
1. Classifique a lista de arquivos por **Nome** ou **Tamanho** para localizar arquivos específicos.

### Alterar o limite de armazenamento local

1. Abra **Gerenciar Armazenamento Local** no menu de opções do Adobe Cloud Drive.
1. Insira o limite de armazenamento desejado.
1. Selecione **Salvar** para aplicar a alteração.

>[!NOTE]
>
>Verifique se há espaço livre em disco suficiente disponível no dispositivo ao definir o limite de armazenamento.

## Exibir atividade de sincronização {#sync-activity}

A atividade de sincronização mostra a atividade recente entre a pasta Adobe Cloud Drive no computador e o Adobe Cloud Storage. Use-a para monitorar uploads e downloads, revisar alterações concluídas e identificar itens que não puderam ser sincronizados.

### Exibir atividade de sincronização

1. Selecione o ícone do Adobe Cloud Drive na barra de menu (Mac) ou na bandeja do sistema (Windows).
1. Expanda a seção atividade de sincronização usando a seta ao lado do resumo do status.
1. Revise os itens listados e seus indicadores de status. Passe o mouse sobre um indicador de status para ver o progresso da transferência, a operação concluída ou uma mensagem de erro.
1. Selecione o menu de mais ações ao lado de um item para ver as ações disponíveis para esse item.

### O que você deve saber sobre a Atividade de sincronização

* A sincronização normal rastreia alterações feitas por meio da pasta do Adobe Cloud Drive, incluindo uploads, downloads, criações, renomeações, movimentações e exclusões.
* A lista de sincronização normal contém até 500 entradas recentes. Entradas novas ou atualizadas aparecem na parte superior. As entradas mais antigas podem ser removidas à medida que a lista atinge seu limite.
* Uma entrada pode exibir inicialmente **Preparando...** enquanto seu nome ou metadados estão sendo resolvidos.
* O resumo exibe o número de itens sincronizados no momento. **Sincronização concluída** significa que não há itens ativos no momento. Inspecione a lista em busca de itens com falha ou excluídos, em vez de tratar esse resumo como uma confirmação de que cada item foi bem-sucedido.
* Os arquivos e pastas excluídos da sincronização podem aparecer com um erro que explica o nome incompatível, o tipo incompatível ou outro motivo de exclusão.
* A atividade é limpa ao sair. A lista é uma visualização de atividade, não um histórico de auditoria permanente.

### Status de sincronização

<!-- Courtney check me: The PDF has two sync status tables (page 7 with 4 statuses, page 8 with 3 statuses and icons). I used the page 8 icons with the page 7 descriptions where they overlap. Confirm and decide whether to keep both tables. -->

| Ícone | Status | Descrição | Ações disponíveis |
| --- | --- | --- | --- |
| Indicador de espera | Aguardando sincronização | O item está aguardando o início de sua operação. | **Mostrar no Localizador** (Mac) ou **Mostrar no Explorer** (Windows), onde aplicável. |
| ![Carregando ícone](assets/acd-sync-status-uploading.png) | Upload / Download | O conteúdo do arquivo está sendo transferido. Passe o mouse sobre o indicador para ver a direção e a porcentagem de transferência quando disponíveis. Em 100%, a dica de ferramenta pode mostrar **Finalizando...** até que o processamento seja concluído. | **Mostrar no Localizador** ou **Mostrar no Explorer**, onde aplicável. |
| ![Ícone Concluído](assets/acd-sync-status-completed.png) | Operação sincronizada/concluída | A operação foi concluída. A dica de ferramenta pode identificar Carregados, Baixados, Criados, Renomeados, Renomeados na nuvem, Movidos, Excluídos ou Excluídos na nuvem. | **Mostrar no Localizador** ou **Mostrar no Explorador** para itens não excluídos. **Abrir no Workfront** para itens qualificados concluídos, não excluídos. |
| ![Ícone de falha](assets/acd-sync-status-failed.png) | Sincronização falhou/excluída | O item não pôde ser sincronizado ou foi excluído da sincronização. Passe o mouse sobre o indicador do motivo. | **Mostrar no Localizador** ou **Mostrar no Explorer**, onde aplicável. Resolva o problema relatado antes de esperar a sincronização do item. |

Itens excluídos não podem ser revelados localmente ou abertos no Workfront a partir de sua entrada de atividade.

### Gerenciar a lista de atividades

| Ação | Descrição |
| --- | --- |
| Expandir ou recolher | Use a seta ao lado do resumo de sincronização para mostrar ou ocultar entradas individuais. |
| Mostrar no Localizador / Mostrar no Explorer | Localize um item não excluído na pasta Adobe Cloud Drive. |
| Abrir no Workfront | Abra um item concluído elegível no Workfront em seu navegador. Esta ação não está disponível para entradas de sincronização normal ativas, com falha ou excluídas. |
| Limpar | Disponível quando nenhum item de sincronização normal estiver ativo. Apaga as entradas concluídas, incluindo as entradas com falha, da exibição de atividade. A limpeza do histórico não exclui arquivos locais ou conteúdo de nuvem e não resolve uma falha de sincronização. |
| Descartar | Depois de limpar um lote concluído, um resumo de itens sincronizados pode ser exibido. Selecione o botão Fechar para descartar o resumo. |

>[!NOTE]
>
>As linhas de sincronização normal não fornecem as ações **Repetir** ou **Cancelar** por item usadas pelo Upload Direto. Para obter informações sobre o Direct Upload, consulte [Fazer upload de arquivos para a nuvem (Direct Upload)](#direct-upload).

## Abrir um item no Workfront {#open-in-workfront}

Abrir no Workfront leva você de um item no Adobe Cloud Drive para o local correspondente no Workfront em seu navegador. Use-o para continuar trabalhando com o item de nuvem no Workfront sem pesquisá-lo manualmente.

### Abrir um item no Localizador ou no Explorador de Arquivos

1. Abra a pasta Adobe Cloud Drive no Finder (Mac) ou no Explorador de arquivos (Windows).
1. Selecione um único arquivo ou pasta associado a um item do Workfront.
1. Clique com o botão direito no item e selecione **Abrir no Workfront**.

   Seu navegador abre o local correspondente do Workfront. Se solicitado, entre com uma conta que tenha acesso a esse item.

### Abrir um item da Atividade de Sincronização

1. Selecione o ícone do Adobe Cloud Drive na barra de menu (Mac) ou na bandeja do sistema (Windows).
1. Expanda a seção atividade de sincronização.
1. Para um item qualificado concluído e não excluído, abra o menu de mais ações e selecione **Abrir no Workfront**.
1. Para um arquivo carregado por meio do Upload Direto, use a mesma ação em sua entrada concluída na seção **Upload Direto**.

### O que você deve saber sobre o Open in Workfront

* Selecione apenas um item por vez. Não há suporte para abrir vários itens selecionados no Workfront.
* No Explorador de arquivos, o comando fica oculto para itens fora da pasta do Adobe Cloud Drive e para a própria raiz da unidade. Está desativado quando vários itens são selecionados.
* Um item deve ter um local correspondente do Workfront. Algumas pastas ou outros itens podem não ter um mapeamento do Workfront, mesmo que estejam visíveis no Adobe Cloud Drive.
* Um novo item local que ainda não terminou de ser carregado pode não ter um link do Workfront. Aguarde a conclusão do upload antes de tentar novamente.
* Na Atividade Sincronizada normal, a ação é oferecida somente para entradas concluídas elegíveis. Ele não é oferecido para entradas ativas, com falha ou excluídas.
* No Upload direto, a ação é oferecida para uploads concluídos, não para entradas em fila, com falha ou canceladas.
* Você deve estar conectado ao Adobe Cloud Drive. O Workfront também pode pedir que você faça logon separadamente no navegador e suas permissões do Workfront ainda se aplicam.
* Você precisa de uma conexão com a Internet para recuperar um link não armazenado em cache e acessar o Workfront. Um link resolvido anteriormente não fornece acesso offline ao Workfront.
* Essa ação abre o Workfront em um navegador. Ele não abre o arquivo em seu aplicativo de desktop, não carrega outra cópia nem altera sua disponibilidade offline local.

### Abrir na disponibilidade do Workfront

| Item ou estado | Abrir no comportamento do Workfront | O que fazer |
| --- | --- | --- |
| Único item elegível no Adobe Cloud Drive | Abre o local correspondente do Workfront. | Selecione **Abrir no Workfront**. |
| Vários itens selecionados | Não há suporte para abrir vários itens. O Explorador de Arquivos desabilita o comando. | Selecione um único item. |
| O novo item ainda está sendo carregado | O link do Workfront pode ainda não estar disponível. | Aguarde a conclusão do upload e tente novamente. |
| Entrada de sincronização normal concluída | Disponível quando o item é elegível e não foi excluído. | Use o menu de mais ações da entrada. |
| Entrada de carregamento direto concluída | Disponível após a conclusão do upload. | Use o menu de mais ações da entrada. |
| Item sem um mapeamento Workfront | Uma mensagem indica que o item não está disponível no Workfront. | Verifique o item diretamente no Workfront ou escolha outro item compatível. |
| Entrada de sincronização normal excluída | Ação não disponível. | Use o Workfront diretamente se precisar investigar o item excluído. |

## Sair do Adobe Cloud Drive

Se você sair do Adobe Cloud Drive, o drive permanecerá visível no Finder ou no Explorador de Arquivos. No entanto, todas as alterações feitas na unidade enquanto você estiver desconectado e todas as alterações que não foram sincronizadas antes de sair não são sincronizadas com a nuvem.

O que acontece a seguir depende da conta com a qual você faz logon novamente.

### Entrar novamente com a mesma conta

O Adobe Cloud Drive preserva a pasta montada local ao sair. Se você fizer logon novamente com as mesmas credenciais:

* O Adobe Cloud Drive reutiliza a montagem existente automaticamente.
* Quaisquer alterações não sincronizadas que você tenha feito antes do logout são mantidas e são sincronizadas assim que a conexão é restaurada.
* Nenhuma ação é necessária.

### Entrar com uma conta diferente

Se você fizer logon com uma conta diferente da Adobe após fazer logoff:

* A pasta montada atual é automaticamente renomeada e copiada em backup. O nome da pasta de backup usa este formato: `Adobe Cloud Drive <usermail>_<short_guid> (backup yyyy-MM-dd HH-mm-ss)`.
* O Adobe Cloud Drive mapeado para a nova conta fica disponível no Finder ou no Explorador de arquivos como de costume.
* Você pode recuperar manualmente qualquer trabalho não sincronizado da pasta de backup antes de removê-lo.

>[!NOTE]
>
>As pastas de backup são salvas em `~/Library/CloudStorage` no Mac e `C:\Users\<user>\` no Windows. Se você alternar várias contas, várias pastas de backup com carimbo de data e hora serão criadas. Revise e limpe backups periodicamente para liberar espaço em disco.

## Resolver conflitos de arquivo

Conflitos podem ocorrer em qualquer uma das seguintes situações:

* Vários usuários editam ou excluem o mesmo arquivo ao mesmo tempo.
* Um arquivo é modificado enquanto outro usuário o abre.
* Interrupções de rede causam problemas de sincronização.

### Como o Adobe Cloud Drive resolve conflitos

O Adobe Cloud Drive usa uma estratégia de duplicação para conflitos:

* **Nenhum bloqueio de arquivo.** Vários usuários podem editar arquivos ao mesmo tempo.
* **Duplicação automática.** Quando o Adobe Cloud Drive detecta um conflito, ele preserva ambas as versões.
* **Limpar nomenclatura.** Os arquivos de conflito incluem nome de usuário e carimbo de data/hora neste formato: `filename (Conflicted copy from username on date_time).extension`. Por exemplo: `hero-banner (Conflicted copy from John on 2026-02-10_16-06-44).psd`.

### Resolver um conflito manualmente

1. Identifique o arquivo de conflito. Os arquivos em conflito têm &quot;Cópia em conflito&quot; no nome do arquivo.
1. Revise ambas as versões para determinar qual está correto.
1. Mantenha a versão correta e exclua a outra versão.
1. Dê um nome adequado ao arquivo retido.

>[!TIP]
>
>Para minimizar conflitos:
>
>* Verifique o status da sincronização antes de editar os arquivos.
>* Comunique-se com os membros da equipe sobre quem está editando quais arquivos.
>* Salve com frequência para que as alterações sejam sincronizadas imediatamente.
>* Feche os arquivos quando terminar de editar.
