---
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: Usar o Adobe Cloud Drive
description: Trabalhe com seus projetos de armazenamento em nuvem da Adobe diretamente do Localizador ou do Explorador de arquivos usando o Adobe Cloud Drive. Abra e edite arquivos em qualquer aplicativo, trabalhe offline e resolva conflitos.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: d5dd769447e81d5d95b4907f8a01016b118f2322
workflow-type: tm+mt
source-wordcount: 1723
ht-degree: 2%

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
