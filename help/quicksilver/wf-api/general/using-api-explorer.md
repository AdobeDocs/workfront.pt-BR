---
content-type: api
navigation-topic: general-api
title: Utilização do API Explorer
description: Utilização do API Explorer
author: Becky
feature: Workfront API
role: Developer
exl-id: dcb7dadb-4dd8-48da-a559-cbe8ad99ff9e
TQID: https://experienceleague.adobe.com/Y-qv5r6ygRA-V7mQSM3wzjaOt58myb64Vxa7UZGsAVo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 368
ht-degree: 100%

---

# Utilização do API Explorer

Ao usar a API principal do Adobe Workfront, o API Explorer é uma ferramenta de referência legada que cataloga os relacionamentos entre recursos, parâmetros e variáveis compatíveis.

## Acessar o API Explorer:

1. Use um navegador da web para acessar o [API Explorer](https://developer.adobe.com/workfront/api-explorer/)\
   ![Navegar até o API Explorer](assets/mceclip1-350x149.png)

1. No canto superior direito do API Explorer, selecione a **versão da API** desejada do Workfront. Por padrão, a versão mais atual é selecionada automaticamente
1. O campo **Filtro** pode ser usado para filtrar os objetos listados por nome e truncar a lista de objetos exibidos de acordo:

   ![Campos do API Explorer](assets/mceclip2-350x147.png)

   * **Campos**: campos disponíveis dentro do objeto especificado.
   * **Referências**: variáveis de referência disponíveis para o objeto especificado. Uma referência é um alias para uma variável. Depois de inicializada, uma referência pode ser usada alternadamente com o nome da variável. Uma referência usa memória inicializada.
   * **Coleções**: coleções disponíveis para o objeto. Coleções são variáveis que representam uma relação “um para muitos” entre o objeto e o recurso.
   * **Pesquisa**: recursos de pesquisa disponíveis para o objeto. Os resultados de uma pesquisa se baseiam nos parâmetros de consulta especificados pelo recurso de pesquisa na solicitação de API.
   * **Ações**: ações compatíveis com o objeto. As ações podem ser procedimentos simples ou complexos executados em relação a um recurso ou conjunto de recursos. Uma determinada ação também pode afetar os recursos relacionados.

1. Abra uma guia e, em seguida, clique na ID do objeto para exibir as variáveis aplicáveis.\
   ![Exibir variáveis](assets/approval-350x89.png)\
   Dependendo do objeto selecionado, as seguintes variáveis podem ser aplicadas:

   | Variável | Definição |
   |---|---|
   | Nome do campo | O nome de um campo usado em uma operação na API do Workfront. |
   | Tipo de campo | O tipo de valores que podem ser inseridos em um campo específico em uma tabela de dados. Os possíveis valores de tipo de campo incluem string, double, int, dateTime. |
   | Tipo enumerado | Os tipos de valores que podem ser usados para identificar um tipo de dados. |
   | Valores possíveis | Valores aceitáveis para o objeto. |
   | Tipo de atributo ObjCode | Atributos que podem ser usados para modificar a classe de objeto. |
   | URL | O caminho de entrada que permite ao aplicativo se comunicar com a API do Workfront. |
   | Argumentos | As variáveis do objeto que podem ser transmitidas entre seu aplicativo e o Workfront. |
   | Tipo de resultado | Tipos de dados permitidos que podem ser retornados por um método. |
