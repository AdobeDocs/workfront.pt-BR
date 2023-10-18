---
title: Atividade de lançamento do Adobe Maestri
description: Use o Maestri para criar objetos, campos e espaços de trabalho personalizados.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 53911aa3-74fd-4747-9008-f86a521ffba6
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '1626'
ht-degree: 0%

---

# Atividade de lançamento do Adobe Maestri

>[!IMPORTANT]
>
>As informações neste artigo referem-se ao Adobe Maestro, que é uma nova oferta do Adobe.
>
>Atualmente, o Adobe Maestro faz parte de um programa beta aberto a um número limitado de clientes.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro/maestro-overview.md).

Este artigo lista os recursos que foram lançados após o lançamento do programa beta fechado do Maestro, em 22 de maio de 2023.

Os recursos lançados são listados na ordem de lançamento, com o mais recente primeiro. Os clientes que estão participando do programa beta fechado Maestro podem acessar todos os recursos em seus ambientes de Pré-visualização e Produção.

>[!IMPORTANT]
>
>A documentação referenciada nas seções abaixo estará disponível algum tempo depois que os recursos forem lançados para produção.

Esta seção lista os recursos e patches que foram lançados após o lançamento do programa beta fechado do Maestro, em 22 de maio de 2023.

Os recursos são lançados semanalmente e são listados na ordem de lançamento, com o mais recente primeiro. Os clientes que estão participando do programa beta fechado Maestro podem acessar todos os recursos em seus ambientes de Pré-visualização e Produção.

## Semana de 16 de outubro de 2023

### Novo tipo de campo Pessoas

Pré-visualização e produção: 16 de outubro de 2023

Agora você pode adicionar um campo do tipo Pessoas aos tipos de registro Maestro. Você pode usar campos do tipo Pessoas para associar usuários existentes a um registro. Para obter informações, consulte [Criar campos](../maestro/architecture-and-fields/create-fields.md).


### Formato Rich Text para campos de parágrafo

Pré-visualização e produção: 16 de outubro de 2023

Adicionamos controles de formato Rich Text para campos do tipo Parágrafo. É possível formatar campos de parágrafo usando Rich Text na exibição de Tabela de um tipo de registro ou na página Detalhes de um registro. Para obter mais informações, consulte [Editar registros](../maestro/records/edit-records.md).


## Semana de 9 de outubro de 2023

### Pesquisar na exibição de tabela

Pré-visualização e produção: 9 de outubro de 2023

Agora é possível pesquisar uma palavra-chave para localizar rapidamente um registro na exibição de tabela. Você pode usar palavras-chave e caracteres especiais em qualquer campo visível na tela para localizar um registro. Para obter informações, consulte [Gerenciar a exibição de tabela](../maestro/views/manage-the-table-view.md).

## Semana de 18 de setembro de 2023

### Reordenar linhas

Pré-visualização e produção: 20 de setembro de 2023

Agora é possível reordenar uma ou várias linhas (ou registros) na exibição Tabela de uma página do tipo de registro. Para obter informações, consulte [Gerenciar a exibição de tabela](../maestro/views/manage-the-table-view.md).

## Semana de 4 de setembro de 2023

### Conectar registros do Maestri com empresas e grupos da Workfront

Pré-visualização e produção: 5 de setembro de 2023

Agora você pode conectar um registro Maestro com empresas e grupos Workfront. Primeiro, você deve criar uma conexão entre um tipo de registro Maestro e os tipos de objeto de empresas e grupos do Workfront. Em seguida, você pode conectar um único registro Maestro do tipo de registro selecionado a empresas e grupos individuais da Workfront.

Considere o seguinte:

* Você deve criar uma conexão entre os tipos de registro Maestro e os tipos de objeto Empresa e Grupo do Workfront para cada Espaço de trabalho.

* Não é possível conectar tipos de registro de taxonomia a tipos de objeto do Workfront.

* Você pode conectar vários registros do Maestro à mesma empresa ou grupo da Workfront, e várias empresas ou grupos ao mesmo registro do Maestro.

* Você não pode editar empresas ou grupos no Maestro. Todas as alterações de empresa ou grupo realizadas no Workfront são visíveis no Maestro, ao revisar os registros vinculados ao Maestro.

  Para obter mais informações, consulte os seguintes artigos:

   * [Conectar tipos de registro](../maestro/architecture-and-fields/connect-record-types.md)
   * [Conectar registros](../maestro/records/connect-records.md)

### Suporte de URL para campos de texto de linha única

Pré-visualização e produção: 7 de setembro de 2023

Para melhor visibilidade ao trabalhar com links na visualização Tabela, adicionamos suporte para URLs em campos de texto de linha única. Usar URLs para outros sites ou unidades externas ao atualizar um campo de texto de linha única, agora os identifica como links e permite clicar neles na tabela. Antes desse aprimoramento, os links eram exibidos como texto.

## Semana de 28 de agosto de 2023

### Menu de visibilidade de campo da barra de ferramentas Exibição em tabela

Pré-visualização e produção: 31 de agosto de 2023

Para exibir as informações certas em um determinado conjunto de registros, especialmente se você pretende compartilhar a exibição com outras pessoas que precisam ver alguns, mas não todos os campos de um tipo de registro, agora é possível selecionar quais campos (ou colunas) exibir e quais ocultar na exibição Tabela.

Você pode ocultar ou mostrar campos individuais de cada cabeçalho das colunas de campo ou gerenciar todos os campos do tipo de registro de uma configuração na barra de ferramentas da exibição de tabela.

Para obter mais informações, consulte [Gerenciar a exibição de tabela](../maestro/views/manage-the-table-view.md).

## Semana de 21 de agosto de 2023

### Conectar registros do Maestro a programas e portfólios

Pré-visualização e produção: 24 de agosto de 2023

Agora você pode conectar um registro do Maestro com programas e portfólios da Workfront. Você deve criar uma conexão entre um tipo de registro Maestro e um programa ou portfólio que cria um campo conectado. Em seguida, você pode conectar qualquer registro Maestro de todos os outros tipos de registro no mesmo espaço de trabalho a programas e portfólios específicos que criam um tipo de registro de Portfolio Workfront ou Programa Workfront somente leitura no mesmo espaço de trabalho. Considere o seguinte:

* Os tipos de registro do conector do Workfront são exclusivos para cada espaço de trabalho.
* Você pode conectar vários registros do Maestro ao mesmo programa ou portfólio do Workfront, e vários programas e portfólios ao mesmo registro do Maestro.
* Não é possível editar programas e portfólios no Maestro. Todas as alterações de programa e portfólio realizadas no Workfront são visíveis no Maestro, ao revisar os registros vinculados.

### Nova funcionalidade de classificação para a exibição de tabela

Pré-visualização e produção: 24 de agosto de 2023

Agora é possível classificar registros na exibição de tabela de uma página do tipo de registro.
Os seguintes recursos estão disponíveis:

* Classificação no nível da tabela, em que é possível classificar por vários campos ao mesmo tempo.
* Classificação no nível da coluna ou do campo, em que é possível classificar por um campo individual de cada vez.

### Melhorias na visualização da linha do tempo: nova aparência para agrupamentos e a opção de visualização Compacta/Padrão

Pré-visualização e produção: 24 de agosto de 2023

Introduzimos as seguintes melhorias na visualização da linha do tempo:

* Agora é possível exibir a exibição de linha do tempo nos seguintes modos:

   * Standard: exibe registros em linhas separadas.
   * Compacto: exibe os registros cujas datas não se cruzam na mesma linha.

* Alteramos a aparência das linhas de agrupamento na exibição de linha do tempo para exibição acima da linha do tempo dos registros que elas contêm. Antes dessa melhoria, as linhas de agrupamento eram exibidas em toda a extensão da linha do tempo.

## Semana de 14 de agosto de 2023

### Reordenar colunas na exibição de tabela

Agora você pode reordenar colunas na exibição de tabela Maestri. Considere o seguinte ao reordenar colunas:

* O campo Nome é sempre o primeiro campo na exibição de tabela de uma página do tipo registro

* Não é possível mover o campo Nome para outra posição

* O campo Nome está congelado e não faz parte da rolagem horizontal.

### Rolagem horizontal para exibição da linha do tempo

Agora é possível rolar horizontalmente na exibição de linha do tempo de um tipo de registro.

## Semana de 7 de agosto de 2023

### Importar tipos de registro de um arquivo do Excel

Pré-visualização e produção: 10 de agosto de 2023

Agora você pode importar um arquivo do Excel para criar tipos de registro em um espaço de trabalho. As folhas do arquivo se tornam os tipos de registro e as colunas do arquivo se tornam seus respectivos campos.

### Experiência aprimorada para conectar tipos de registro e projetos

Pré-visualização e produção: 10 de agosto de 2023

Melhoramos a maneira como você conecta tipos de registros, incluindo a conexão com projetos do Workfront. Como parte dessa melhoria, fizemos as seguintes alterações ao adicionar um campo para um tipo de registro na exibição de tabela:

* O campo Tipo de relação foi removido da guia &quot;Novo campo&quot;.

* Adicione uma guia &quot;New connection&quot; onde você pode selecionar diretamente o tipo de registro ou objeto ao qual deseja se conectar, eliminando a necessidade de um campo do tipo Relacionamento.

## Semana de 10 de julho de 2023

### Atualizar a aparência de um tipo de registro

Pré-visualização e produção: 13 de julho de 2023

Agora é possível selecionar um ícone personalizado para um tipo de registro e uma cor personalizada para o ícone de tipo de registro.

### Novo tipo de campo da caixa de seleção

Pré-visualização e produção: 13 de julho de 2023

Agora você pode adicionar um tipo de campo Caixa de seleção aos tipos de registro Mestre. Você pode usar um campo do tipo Caixa de seleção para adicionar uma única opção de caixa de seleção a um registro. Você pode usar esse campo para indicar um atributo ou status específico para esse registro específico. Por exemplo, você pode usá-lo como um sinalizador para rastrear a conclusão, a aprovação ou qualquer outro atributo binário para cada registro.

## Semana de 26 de junho de 2023

### Ativação rápida do menu contextual em uma tabela

Pré-visualização e produção: 28 de junho de 2023

Ativamos a capacidade de ativar o menu contextual clicando com o botão direito do mouse em qualquer lugar em uma linha de registro, ao visualizar os registros na exibição de tabela ou em um tipo de registro. Agora é possível visualizar, excluir ou copiar rapidamente um link para a página Detalhes do registro ao acessar o menu contextual de qualquer lugar na exibição de tabela de um tipo de registro. Antes desse aprimoramento, o menu contextual era acessível somente pelo menu Mais na coluna Nome de um registro.

## Semana de 19 de junho de 2023

### Os nomes dos campos de registro são exclusivos

Introduzimos um requisito agora que os nomes de campos de um tipo de registro Maestri devem ter nomes únicos. Os campos que pertencem a tipos de registro diferentes não precisam ter nomes exclusivos.

## Semana de 5 de junho de 2023

### Conectar registros do Maestri com projetos da Workfront

Pré-visualização e produção: 5 de junho de 2023

Agora você pode conectar um registro Maestro com projetos Workfront. Você deve criar um tipo de registro conector Maestri para estabelecer a conexão entre os registros Maestri e os projetos Workfront. Em seguida, é possível conectar qualquer registro Maestro de todos os outros tipos de registro ao registro conector usando o campo Relacionamento. Considere o seguinte:

* Você deve ter um tipo de registro de conector para o Workfront para cada Espaço de trabalho.
* Você pode conectar vários registros do Maestro ao mesmo projeto do Workfront, e vários projetos ao mesmo registro do Maestro.
* Não é possível editar projetos no Maestro. Todas as alterações de projeto realizadas no Workfront são visíveis no Maestro, ao revisar os registros vinculados.

## Semana de 29 de maio de 2023

### Requisito de duas datas para criar uma exibição de Linha do tempo

Pré-visualização e produção: 31 de maio de 2023

Você deve ter pelo menos dois campos de data associados a um tipo de registro para criar um modo de exibição de Linha do Tempo.
