---
filename: troubleshooting-proof-creation-failures
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: use-the-desktop-proofing-viewer
title: Solução de problemas de falhas de criação de prova
description: O processo de criação de prova inclui a importação e a geração de prova. Ocasionalmente, ao criar uma prova, um arquivo pode não ser importado ou a prova pode não ser gerada após a importação do arquivo.
author: Courtney
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---


# Solução de problemas de falhas de criação de prova

O processo de criação de prova inclui a importação e a geração de prova. Ocasionalmente, ao criar uma prova, um arquivo pode não ser importado ou a prova pode não ser gerada após a importação do arquivo.

>[!NOTE]
>
> Se o documento que você está tentando provar não corresponder a nenhum dos critérios listados nesta seção, entre em contato com o Suporte da Adobe Workfront para obter mais informações.

## Motivos para falha de importação

* Você criou uma prova combinada contendo mais de 50 arquivos.

## Motivos para falha na geração de prova

* O tipo de arquivo não é compatível.\
  Para obter uma lista de tipos de arquivos com suporte, consulte [Visão geral sobre tipos de arquivos com suporte e limites de tamanho](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

* A estrutura do arquivo é uma estrutura não padrão para o tipo de arquivo.
* O arquivo está protegido por uma senha ou o conteúdo de cópia está desabilitado.

  Diferentemente de outros tipos de arquivos, os arquivos PDF podem ser gerados em provas se a configuração de segurança para cópia de conteúdo estiver definida como Permitido no PDF.

* O comprimento ou a contagem de páginas excede o limite.

  O comprimento máximo permitido da página é de 195 polegadas após a rasterização; a contagem máxima permitida de páginas é de 1.000 páginas para uma única prova.

* O arquivo está danificado ou corrompido.
* O prazo do fluxo de trabalho em uma nova versão de prova está no passado.

  Isso ocorre quando você está criando uma nova versão de prova usando um método de prova rápida e **Gerar provas automaticamente ao carregar documentos** está selecionado. A nova versão de prova tenta pegar os prazos do fluxo de trabalho da prova gerada anteriormente. A geração de prova falha se esses prazos estiverem no passado. Para corrigir isso, você pode definir os prazos do fluxo de trabalho na versão anterior no futuro ou gerar uma nova versão de prova. Se você gerar uma nova versão, use **Mais > Nova Versão > Prova** e selecione **Prazos finais do fluxo de trabalho no futuro**.

* Ao revisar arquivos PDF, os motivos para falha na geração de prova incluem:

   * Fontes e imagens são vinculadas de fontes externas (como do sistema de arquivos local)

     Fontes e imagens devem ser incorporadas ao arquivo PDF para serem exibidas em outro computador ou no Workfront Proof.

   * O arquivo PDF contém camadas vazias ou campos transparentes ou sobrepostos.

     Se você não puder determinar qual camada ou objeto causa isso, exporte o design/documento como um PDF otimizado (isso remove todos os elementos indesejados).

