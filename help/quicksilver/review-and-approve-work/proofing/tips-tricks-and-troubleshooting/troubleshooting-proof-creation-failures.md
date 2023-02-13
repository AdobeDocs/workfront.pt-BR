---
filename: troubleshooting-proof-creation-failures
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: use-the-desktop-proofing-viewer
title: Solucionar problemas de falhas de criação de prova
description: O processo de criação de prova inclui a importação e a geração de prova. Ocasionalmente, ao criar uma prova, um arquivo pode falhar na importação ou a prova pode não ser gerada após a importação do arquivo.
author: Courtney
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---


# Solucionar problemas de falhas de criação de prova

O processo de criação de prova inclui a importação e a geração de prova. Ocasionalmente, ao criar uma prova, um arquivo pode falhar na importação ou a prova pode não ser gerada após a importação do arquivo.

>[!NOTE]
>
> Se o documento que você está tentando provar não corresponder a nenhum dos critérios listados nesta seção, entre em contato com o Suporte da Adobe Workfront para obter mais investigações.

## Motivos para falha na importação

* Você criou uma prova combinada contendo mais de 50 arquivos.

## Motivos para falha na geração de prova

* Não há suporte para o tipo de arquivo.\
   Para obter uma lista de tipos de arquivos suportados, consulte [Visão geral dos tipos de arquivos de prova suportados e limites de tamanho](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

* A estrutura de arquivo é uma estrutura não padrão para o tipo de arquivo.
* O arquivo é protegido por uma senha ou tem a cópia de conteúdo desativada.

   Diferentemente de outros tipos de arquivos, os arquivos PDF podem ser gerados em provas se a configuração de segurança para cópia de conteúdo estiver definida como Permitido no PDF.

* A duração da página ou a contagem da página excede o limite.

   O comprimento máximo de página permitido é de 195 polegadas após rasterização; a contagem máxima de páginas permitida é de 1.000 páginas para uma única prova.

* O arquivo está danificado ou corrompido.
* O prazo do workflow em uma nova versão de prova já era.

   Isso ocorre ao criar uma nova versão de prova usando um método de prova rápida e **Gerar provas automaticamente ao carregar documentos** está selecionada. A nova versão de prova tenta obter os prazos do fluxo de trabalho da prova gerada anteriormente. A geração de prova falha se esses prazos estiverem no passado. Para corrigir isso, você pode definir os prazos do fluxo de trabalho na versão anterior no futuro ou gerar uma nova versão de prova. Se você gerar uma nova versão, use **Mais > Nova versão > Prova** e selecione **Prazos de workflow no futuro**.

* Ao revisar arquivos PDF, os motivos para falha de geração de prova incluem:

   * Fontes e imagens são vinculadas de fontes externas (como de seu sistema de arquivos local)

      As fontes e imagens devem ser incorporadas no arquivo PDF para serem exibidas em outro computador ou dentro da Workfront Proof.

   * O arquivo PDF contém camadas vazias ou campos transparentes ou sobrepostos.

      Se não for possível determinar qual camada ou objeto causa isso, exporte o design/documento como um PDF otimizado (isso remove todos os elementos indesejados).

