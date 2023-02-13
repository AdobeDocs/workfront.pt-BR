---
title: Revisar limitações de colaboração com pessoas fora de sua organização
description: Revisar limitações de colaboração com pessoas fora de sua organização
author: Courtney
draft: Probably
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Revisar limitações de colaboração com pessoas fora de sua organização

Há algumas limitações a serem observadas ao se comunicar com pessoas fora da organização quando elas forem adicionadas a uma prova, especificamente se a pessoa fora da organização tiver acesso à prova em um ambiente separado.

## Contatos com distinção entre membros

Existem três tipos de contatos em um ambiente de prova:

* **Usuários**: Os usuários têm um logon da Workfront Proof no ambiente de sua organização.
* **Membros**: Os membros têm seu próprio logon na Workfront Proof em outro ambiente da organização (não o seu). Não é possível converter membros em usuários em seu ambiente.
* **Convidados**: Os convidados não têm seu próprio logon na Workfront Proof no ambiente de sua organização, mas você adicionou seus detalhes à conta (por exemplo, revisores convidados em provas). Você pode converter convidados em usuários.

Como os membros não podem ser convertidos em usuários, a capacidade de adicionar tags às pessoas em comentários de prova é limitada aos usuários de *sua organização original*.

**Exemplo:** A Empresa A convida um usuário externo para revisar uma prova. Esse usuário já existe em um ambiente de prova separado, Empresa B.

 

Quando a Empresa A convida o usuário externo para a prova, o usuário externo é adicionado à lista de contatos da Empresa A como Membro. Os revisores no workflow de prova da Empresa A podem marcar o usuário externo em comentários de prova porque agora estão no diretório de contato da Empresa A.

 

O usuário externo não pode marcar usuários da Empresa A, mesmo que eles estejam no mesmo fluxo de trabalho de prova, pois os usuários da Empresa A não foram adicionados como contatos à Empresa B.

 

O usuário externo da Empresa B pode marcar outros usuários da Empresa B se estiverem no fluxo de trabalho de prova ou se tiverem permissão para compartilhar a prova com novos usuários, pois esses usuários existem como contatos na Empresa B.
