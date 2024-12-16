---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Solução de problemas de promoção do ambiente
description: Solucionar problemas comuns com a promoção do ambiente.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 830dd573-d954-4ba2-a1d3-d1645b3fbac8
source-git-commit: c3c9a423bd60b26b2605a1b52bd706c9bc6acdec
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---

# Solução de problemas de promoção do ambiente

Este artigo descreve como solucionar problemas de promoção de ambientes.

## Problema: o pacote de promoção do ambiente está travando ou falhando

Se o pacote de promoção do ambiente estiver sendo paralisado ou falhar, tente o seguinte:

* Se a instalação de um pacote parar após 10-15 minutos, ou se a instalação de um pacote falhar, remonte o pacote existente ou crie um novo pacote.

* Se a instalação de um pacote falhar, pode haver um problema com um ou mais objetos. Verifique as mensagens de erro, que identificam o objeto e podem ajudar a identificar o problema. Depois de solucionar o problema com o objeto, remonte o pacote e tente instalar novamente.

* Se você ainda tiver problemas com uma instalação, tente replicar a instalação em um ambiente de destino diferente. Mantenha o mais próximo possível da instalação original, incluindo objetos e ações de instalação selecionadas.

* Recomendamos sempre verificar o conteúdo do pacote após a montagem para confirmar que ele contém os objetos esperados.


## Problema: falha ao promover o formulário personalizado

Isso pode ocorrer porque o formulário personalizado inclui um campo calculado. Se um campo calculado referenciar um campo que não esteja referenciado em um formulário personalizado, um pacote que inclua esse formulário não será promovido e o usuário poderá ver a seguinte mensagem:

&quot;Os seguintes campos são inválidos: Expressão personalizada inválida Expressão inválida: expressão personalizada inválida.&quot;

Esse problema pode surgir ao referenciar um campo existente que não está anexado a nenhum formulário personalizado no ambiente de destino ou com um campo recém-criado.

Para resolver esse problema, siga um destes procedimentos:

* Crie um pacote com um formulário personalizado do tipo projeto que inclua o campo referenciado. Depois de promover esse pacote para o ambiente de destino, promova o pacote originalmente pretendido que contém o campo calculado.
* Crie manualmente o campo referenciado no ambiente de destino e associe-o a um formulário personalizado do tipo projeto. Depois disso, o campo será reconhecido e você poderá promover o pacote sem encontrar o erro.
