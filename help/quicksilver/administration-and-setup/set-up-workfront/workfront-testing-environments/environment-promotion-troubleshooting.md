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
source-git-commit: e9df34c206dd65ccc2edec00087248eb4ed16f54
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---

# Solução de problemas de promoção do ambiente

Se o pacote de promoção do ambiente estiver sendo paralisado ou falhar, tente o seguinte:

* Se a instalação de um pacote parar após 10-15 minutos, ou se a instalação de um pacote falhar, remonte o pacote existente ou crie um novo pacote.

* Se a instalação de um pacote falhar, pode haver um problema com um ou mais objetos. Verifique as mensagens de erro, que identificam o objeto e podem ajudar a identificar o problema. Depois de solucionar o problema com o objeto, remonte o pacote e tente instalar novamente.

* Se você ainda tiver problemas com uma instalação, tente replicar a instalação em um ambiente de destino diferente. Mantenha o mais próximo possível da instalação original, incluindo objetos e ações de instalação selecionadas.

* Recomendamos sempre verificar o conteúdo do pacote após a montagem para confirmar que ele contém os objetos esperados.
