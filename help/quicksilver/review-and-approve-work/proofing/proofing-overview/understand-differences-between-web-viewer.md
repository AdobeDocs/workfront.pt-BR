---
content-type: reference
product-area: documents
navigation-topic: proofing-overview
title: Diferenças entre o Visualizador de provas da Web e a visão geral do Visualizador de provas do desktop
description: Saiba mais sobre as diferenças entre os visualizadores de desktop e de prova na web.
author: Courtney
feature: Digital Content and Documents
exl-id: 72ce147b-29c9-4c3b-a03c-2da0758bc178
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '865'
ht-degree: 0%

---

# Diferenças entre o Visualizador de provas da Web e a visão geral do Visualizador de provas do desktop

O Adobe Workfront fornece dois revisores de prova diferentes:

* **Visualizador de provas da web:** Projetado principalmente para prova de arquivos estáticos e de vídeo. É executado no Google Chrome, Firefox ou Safari.
* **Visualizador de provas de desktop:** Projetado para revisar arquivos interativos, assim como arquivos de vídeo e estáticos. É executado como um aplicativo independente na estação de trabalho. Para obter mais informações, consulte [Entender o visualizador de provas de desktop](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md)

* Se sua organização não puder usar o aplicativo Visualizador de provas de desktop por motivos de segurança, o administrador do Workfront poderá configurar seu sistema para que você possa revisar o conteúdo interativo, incluído em um arquivo ZIP, no Visualizador de provas de web. Para obter mais informações, consulte  [Configurar prova de conteúdo interativa no Visualizador de Prova da Web](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/interactive-content-in-web-viewer.md).

A lista a seguir pode ajudá-lo a entender o Visualizador de provas que pode ser usado para revisar determinados tipos de conteúdo:

* **Conteúdo interativo da Web - URL**: Se você criar uma prova para conteúdo da Web usando um URL e quiser fazer a prova do conteúdo interativamente, deverá usar o Visualizador de provas da área de trabalho.
* **Conteúdo interativo da Web - Arquivo ZIP**: Se você criar uma prova para conteúdo da Web usando um arquivo ZIP, poderá usar o Visualizador de provas da Web (com algumas limitações) ou o Visualizador de provas da área de trabalho. Para obter informações sobre as limitações envolvidas no uso do Web Proofing Viewer para conteúdo interativo, consulte [Configurar prova de conteúdo interativa no Visualizador de Prova da Web](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/interactive-content-in-web-viewer.md).

* **Conteúdo estático e de vídeo**: Se você criar uma prova com conteúdo estático, poderá usar o Visualizador de provas da Web ou o Visualizador de provas da área de trabalho.

## Provas estáticas

| **Recurso** | **Visualizador de provas da web** | **Visualizador de provas de desktop** |
|---|---|---|
| Abrir provas estáticas | ✓ µ | ✓&#42; |
| Visualizações únicas, de revista e contínuas | ✓ | ✓&#42; |
| Panorâmica | ✓ | ✓&#42; |
| Zoom | ✓ | ✓&#42; |
| Girar | ✓ | ✓&#42; |
| Ferramenta de medição | ✓ ➡ (definir uma área com tamanho personalizado) | ✓&#42; |
| Exibição em miniatura | ✓ | ✓&#42; |
| Navegador de prova estática | ✓ | ✓&#42; |
| Pesquisa de documentos | ✓ | ✓&#42; |
| Publicar comentário em várias páginas | ✓ (disponível em todas as exibições) | ✓ µ&#42; (disponível em todas as exibições) |
| Atalhos de prova estáticos avançados | ✓ (para obter mais informações, consulte [Atalhos de teclado no visualizador de provas](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) | ✓ µ&#42;(para obter mais informações, consulte [Atalhos de teclado no visualizador de provas](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) |

{style="table-layout:auto"}

&#42; Essa funcionalidade funciona somente se o administrador do Workfront tiver configurado o Visualizador de provas de área de trabalho como o visualizador padrão para todas as provas.

## Provas de vídeo

| **Recurso**  | **Visualizador de provas da web** | **Visualizador de provas de desktop** |
|---|---|---|
| Abrir provas de vídeo | ✓ | ✓&#42; |
| Buffering | ✓ | ✓&#42; |
| Revisar usando o tempo | ✓ | ✓&#42; |
| Revisar usando quadros ou código de tempo | ✓ | ✓&#42; |
| Revisar mais rápido ou mais lento | ✓ | ✓&#42; |
| Regulação de volume | ✓ | ✓&#42;  |
| modo de tela cheia | ✓ | ✓&#42;  |
| Comentários de intervalo | ✓ | ✓&#42;  |
| Executar provas de vídeo em loop (os vídeos são concluídos e iniciados automaticamente) | ✓ | ✓&#42;  |
| Atalhos de vídeo avançados | ✓ (para obter mais informações, consulte [Atalhos de teclado no visualizador de provas](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) | ✓&#42;  |

{style="table-layout:auto"}

&#42; Essa funcionalidade funciona somente se o Visualizador de provas da área de trabalho estiver configurado como o visualizador padrão para todas as provas.

## Provas interativas

| **Recurso**  | **Visualizador de provas da web** | **Visualizador de provas de desktop** |
|---|---|---|
| Abrir provas interativas criadas a partir de conteúdo agrupado em um arquivo ZIP | ✓ | ✓ ➡ (recomendado) |
| Abrir uma prova interativa criada a partir de um URL | Não suportado | ✓ |
| Exibir provas interativas (criadas a partir do conteúdo agrupado em um arquivo ZIP) em vários tamanhos de tela | ✓ | ✓ |
| Visualizar provas interativas (criadas a partir de conteúdo agrupado em um arquivo ZIP) para vários dispositivos | Não suportado | ✓ |
| Revisar sites não seguros (HTTP) | Não suportado | ✓ |
| Revisar sites protegidos pelo iFrame (sites protegidos contra visualização em um iFrame) | Não suportado | ✓ |

{style="table-layout:auto"}

## Comentários

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Recurso</th> 
   <th>Visualizador de provas da web </th> 
   <th>Visualizador de provas de desktop </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Adicionar, excluir e editar comentários</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Adicionar e excluir respostas</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Ferramentas de marcação de retângulo, seta, linha, à mão livre e realce</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Ferramenta Poligonal</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Ferramentas de marcação da máscara de corte</p> </td> 
   <td>Não suportado</td> 
   <td>Não suportado</td> 
  </tr> 
  <tr> 
   <td> <p>Ferramenta Marcação de seleção de texto</p> </td> 
   <td>✓ µ Somente provas estáticas</td> 
   <td>✓ µ Somente provas estáticas</td> 
  </tr> 
  <tr> 
   <td> <p>Alterar cor de marcação</p> </td> 
   <td>✓ (32 cores disponíveis) </td> 
   <td>✓ (32 cores disponíveis) </td> 
  </tr> 
  <tr> 
   <td> <p>Alterar opacidade da marcação</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Alterar espessura da marcação</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Recortar, copiar e colar marcações</p> </td> 
   <td> Não suportado</td> 
   <td> Não suportado</td> 
  </tr> 
  <tr> 
   <td> <p>Desfazer e refazer a última operação</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Marcações duplicadas</p> </td> 
   <td> Não suportado</td> 
   <td> Não suportado</td> 
  </tr> 
  <tr> 
   <td>Definir ações como comentários</td> 
   <td>✓ (As ações ficam visíveis nos comentários imediatamente após a definição da ação)</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Definir cor de marcação como padrão</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Resolver comentários</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Bloquear comentários</p> </td> 
   <td>Não suportado</td> 
   <td> Não suportado</td> 
  </tr> 
  <tr> 
   <td> <p>Marcar usuários</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Retomar comentários</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Exibir a lista de comentários em uma exibição compacta</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Exibir a lista de comentários em uma visualização padrão, completa ou única</p> </td> 
   <td>Planejado para o futuro</td> 
   <td>Planejado para o futuro</td> 
  </tr> 
  <tr> 
   <td> <p>Pesquisar comentários</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Filtrar comentários por usuário</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Filtrar comentários e respostas por usuário</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Classificar comentários</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Atualizações automáticas de comentário</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Decisões

| Recurso | Visualizador de provas da web | Visualizador de provas de desktop |
|---|---|---|
| Tomar decisões | ✓ | ✓ |
| Personalizar decisões | ✓ | ✓ |

{style="table-layout:auto"}

## Comparar provas

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Recurso</th> 
   <th>Visualizador de provas da web </th> 
   <th>Visualizador de provas de desktop </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Comparar diferentes versões de provas</td> 
   <td>✓</td> 
   <td>✓<br></td> 
  </tr> 
  <tr> 
   <td>Comparar provas separadas</td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

## Operações de prova

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Recurso</th> 
   <th>Visualizador de provas da web </th> 
   <th>Visualizador de provas de desktop </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Alterar a versão da prova </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td>Criar uma nova versão</td> 
   <td> <p>Disponível somente na Prova do Workfront (planejado para o futuro ao fazer a prova no Workfront)<br></p> </td> 
   <td>Disponível somente na Prova do Workfront (planejado para o futuro ao fazer a prova no Workfront)</td> 
  </tr> 
  <tr> 
   <td>Revisar detalhes da prova </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Revisar fluxos de trabalho de prova</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Editar estágios de fluxo de trabalho</td> 
   <td>Não suportado</td> 
   <td>Não suportado</td> 
  </tr> 
  <tr> 
   <td>Compartilhar provas</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Obter URL da equipe</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Alterar notificações por email</td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Baixar arquivo original</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Bloquear e desbloquear provas e estágios</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Imprimir resumo da prova</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Excluir provas</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Gerenciar provas na mesma pasta</td> 
   <td><strong>Disponível somente na prova do Workfront</strong> </td> 
   <td><strong>Disponível somente na prova do Workfront</strong> </td> 
  </tr> 
  <tr> 
   <td>Marcas (logotipos personalizados)</td> 
   <td>✓</td> 
   <td> ✓ µ<br>(Logotipo do Workfront na página de lançamento) </td> 
  </tr> 
  <tr> 
   <td>Links personalizados (somente Workfront Proof)</td> 
   <td>Não suportado</td> 
   <td> Não suportado </td> 
  </tr> 
  <tr> 
   <td>Integrações do carimbo de base (somente Workfront Proof) </td> 
   <td>Planejado para o futuro</td> 
   <td>Planejado para o futuro</td> 
  </tr> 
  <tr> 
   <td>Indicador de presença </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Atualizações automáticas de prova (alterações de permissão e novas versões)</td> 
   <td>✓</td> 
   <td>✓ </td> 
  </tr> 
 </tbody> 
</table>

## Minivisualizador

| **Recurso**  | **Visualizador de provas da web**  | **Visualizador de provas de desktop** |
|---|---|---|
| Código incorporado | Planejado para o futuro para provas de vídeo estáticas e nativas | Não suportado  |

{style="table-layout:auto"}

## Traduções

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Recurso</strong> </th> 
   <th><strong>Visualizador de provas da web</strong> </th> 
   <th><strong>Visualizador de provas de desktop</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Idiomas de suporte diferentes do inglês</td> 
   <td>✓</td> 
   <td>✓<br></td> 
  </tr> 
 </tbody> 
</table>
