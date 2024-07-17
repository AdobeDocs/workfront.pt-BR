---
title: Prova de limitações de colaboração com pessoas de fora da organização
description: Prova de limitações de colaboração com pessoas de fora da organização
author: Courtney
draft: Probably
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Prova de limitações de colaboração com pessoas de fora da organização

Há algumas limitações que devem ser observadas ao se comunicar com pessoas de fora da sua organização quando adicionadas a uma prova, especificamente se a pessoa de fora da sua organização tiver acesso à prova em um ambiente separado.

## Contatos com a distinção entre Estados-Membros

Há três tipos de contatos que existem em um ambiente de prova:

* **Usuários**: os usuários têm um logon do Workfront Proof no ambiente de sua organização.
* **Membros**: os membros têm seu próprio logon no Workfront Proof no ambiente de outra organização (não o seu). Não é possível converter membros em usuários em seu ambiente.
* **Convidados**: os convidados não têm seu próprio logon no Workfront Proof no ambiente de sua organização, mas você adicionou os detalhes deles à sua conta (por exemplo, revisores convidados em provas). Você pode converter convidados em usuários.

Como os Membros não podem ser convertidos em usuários, sua capacidade de marcar pessoas em comentários de prova é limitada aos usuários de *sua organização original*.

**Exemplo:** a Empresa A convida um usuário externo para analisar uma prova. Esse usuário já existe em um ambiente de prova separado, Empresa B.

 

Quando a Empresa A convida o usuário externo para a prova, o usuário externo é adicionado à lista de contatos da Empresa A como membro. Os revisores no fluxo de trabalho de prova da Empresa A podem marcar o usuário externo em comentários de prova, pois eles agora estão no diretório de contato da Empresa A.

 

O usuário externo não pode marcar os usuários da Empresa A, mesmo que eles estejam no mesmo fluxo de trabalho de prova, pois os usuários da Empresa A não foram adicionados como contatos à Empresa B.

 

O usuário externo da Empresa B pode marcar outros usuários da Empresa B se eles estiverem no fluxo de trabalho de prova ou se tiverem permissão para compartilhar a prova com novos usuários, pois esses usuários existem como contatos na Empresa B.
