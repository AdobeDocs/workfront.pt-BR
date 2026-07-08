---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: Solução de problemas do Adobe Cloud Drive
description: Revise limitações, considerações sobre desempenho e soluções para problemas comuns com o Adobe Cloud Drive no Mac e Windows.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 6ad89f8d00dd3a06eb160863c3213a9f80b1a44b
workflow-type: tm+mt
source-wordcount: 928
ht-degree: 0%

---

# Solução de problemas do Adobe Cloud Drive

Este artigo descreve as limitações do Adobe Cloud Drive, as considerações sobre desempenho que devem ser levadas em conta e as soluções para problemas comuns que você pode encontrar.

Para obter informações sobre como trabalhar com o Adobe Cloud Drive, consulte [Usar o Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md).

## Limitações

### Operações de arquivos e pastas

* As pastas do projeto são somente leitura no nível superior. Não é possível renomear, excluir ou movê-los do Adobe Cloud Drive. Para criar, renomear ou excluir um projeto, use a interface da Web do Workfront.
* As operações de arquivos e pastas dentro de uma pasta do projeto são totalmente compatíveis.

### Limites de arquivo e caminho

* Os nomes de arquivo não podem exceder 255 caracteres em qualquer plataforma.
* O caminho de arquivo completo (todos os nomes de pasta mais o nome de arquivo) não pode exceder 1024 caracteres. Os arquivos com caminhos mais longos do que esse limite não aparecem no Adobe Cloud Drive, mesmo se estiverem visíveis na interface da Web do Workfront.
* Se você vir um erro de **Caminho completo muito longo** em um arquivo, reduza os nomes das pastas ou reduza a profundidade de aninhamento de pastas para colocar o caminho dentro do limite.

### Armazenamento

* Os arquivos salvos no Adobe Cloud Drive usam o espaço em disco localmente em seu dispositivo.
* Arquivos somente na nuvem não usam armazenamento local.
* Remova o acesso off-line dos arquivos que não são mais necessários. Para obter mais informações, consulte [Remover acesso offline para liberar espaço](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md#remove-offline-access-to-free-up-space) em [Usar a Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md).

## Considerações sobre desempenho

* **Tamanho do arquivo:** O tempo necessário para a sincronização depende do tamanho do arquivo. Arquivos maiores geralmente levam mais tempo.
* **Velocidade da rede**: conexões mais rápidas oferecem melhor desempenho de sincronização. A sincronização é retomada automaticamente após uma interrupção.
* **Acesso pela primeira vez:** os arquivos são baixados sob demanda na primeira vez que você os acessa. O acesso subsequente é mais rápido porque o arquivo é armazenado em cache localmente.

## Problemas comuns

### O Adobe Cloud Drive não está aparecendo

**Causas possíveis:**

* O Adobe Cloud Drive não está instalado.
* A instalação não foi concluída com êxito.
* Sua organização não tem uma versão do Workfront compatível com o armazenamento em nuvem da Adobe.

**Soluções:**

* Verifique se o Adobe Cloud Drive está instalado. Verifique **Aplicativos** (Mac) ou **Programas** (Windows).
* Inicie o Adobe Cloud Drive manualmente.
* Entre em contato com o administrador do Workfront para confirmar se sua organização tem uma versão do Workfront compatível com o armazenamento em nuvem da Adobe.
* Reinstale o Adobe Cloud Drive, se necessário. Para obter mais informações, consulte [Instalar a Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md).

### O ícone do Adobe Cloud Drive não está visível na barra de menus ou na barra de tarefas

**Causas possíveis:**

* A barra de menus (Mac) ou a bandeja do sistema (Windows) não têm espaço suficiente para exibir o ícone.

**Soluções:**

* **Mac:** Segure Cmd e arraste os ícones existentes da barra de menus para reorganizá-los ou removê-los, criando espaço para o ícone do Adobe Cloud Drive.
* **Windows:** clique na seta para cima (**Mostrar ícones ocultos**) na barra de tarefas para localizar o ícone da Adobe Cloud Drive e arraste-o para a área visível.

### Os projetos não estão sendo exibidos ou alguns projetos estão ausentes

**Causas possíveis:**

* Você não tem acesso a nenhum projeto.
* Sincronização não concluída.
* Problema de conectividade de rede.

**Soluções:**

* Verifique o acesso ao projeto na interface da Web do Workfront.
* Verifique sua conexão de rede.
* Saia do Adobe Cloud Drive e entre novamente.

### Os arquivos não estão sendo sincronizados

**Causas possíveis:**

* Problema de conectividade de rede.
* Há um erro de sincronização no arquivo ou pasta.
* Você não tem espaço em disco suficiente.

**Soluções:**

* Verifique sua conexão com a Internet.
* Verifique se há espaço em disco suficiente disponível.
* Verifique se há erros de sincronização nos indicadores de status do arquivo. Para obter mais informações, consulte [Indicadores de status do arquivo](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md#file-status-indicators) em [Usar a Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md).
* Reinicie o Adobe Cloud Drive.
* Verifique o status do Adobe Cloud Drive na bandeja do sistema (Windows) ou na barra de menus (Mac).

### Você não pode abrir um arquivo

**Causas possíveis:**

* O arquivo é somente na nuvem e o download falhou.
* O aplicativo necessário para abrir o arquivo não está instalado.
* O arquivo está corrompido.

**Soluções:**

* Verifique o indicador de status do arquivo.
* Verifique se o aplicativo necessário está instalado.
* Clique com o botão direito do mouse no arquivo, selecione **Manter neste Dispositivo** e tente abri-lo novamente.
* Verifique se o arquivo não está corrompido na interface da Web do Workfront.

### A sincronização está lenta

**Causas possíveis:**

* O arquivo é grande.
* A conexão de rede está lenta.
* Muitos arquivos estão sendo sincronizados ao mesmo tempo.

**Soluções:**

* Seja paciente com arquivos grandes. A sincronização pode ser retomada, portanto, continua de onde parou após uma interrupção.
* Verifique a velocidade da sua rede.
* Limitar o número de operações de arquivos simultâneas.
* Mantenha arquivos grandes somente na nuvem, a menos que precise de acesso offline.

### Os arquivos offline estão ocupando muito espaço

**Soluções:**

* Clique com o botão direito em arquivos offline e selecione **Liberar Espaço**.
* Verifique o espaço em disco regularmente.
* Mantenha arquivos grandes que você raramente acessa no modo somente na nuvem.

### Não é possível criar, editar ou excluir arquivos ou pastas

**Causas possíveis:**

* Você está tentando criar, renomear ou excluir uma pasta de projeto. As pastas do projeto são somente leitura no nível superior.
* O projeto é somente leitura para você e, portanto, não é possível criar, editar ou excluir arquivos ou pastas nele.

**Soluções:**

* Para criar, renomear ou excluir um projeto, use a interface da Web do Workfront.
* Peça ao proprietário do projeto para compartilhar o projeto com você com acesso de edição.

## Obter ajuda

Para perguntas sobre licença, problemas de acesso ao projeto ou configuração específica da organização, entre em contato com o administrador do Workfront.

Para compartilhar logs com o suporte da Adobe, siga as etapas em [Executar a ferramenta coletor de logs do Adobe](https://helpx.adobe.com/br/creative-cloud/apps/troubleshoot/diagnostics-repair-tools/run-log-collector-tool.html).

## Práticas recomendadas

* **Planejar trabalho offline.** Baixe arquivos antes de viajar ou trabalhar em áreas com baixa conectividade.
* **Monitorar status de sincronização.** Verifique os indicadores de arquivo antes de fechar os aplicativos.
* **Siga a estrutura de pastas do projeto.** Organize os arquivos nas pastas do projeto como o proprietário do projeto pretende.
* **Usar nomes de arquivo descritivos.** Ajude os membros da equipe a encontrar o que precisam.
* **Evite criar duplicatas.** Não faça cópias desnecessárias de arquivos.
