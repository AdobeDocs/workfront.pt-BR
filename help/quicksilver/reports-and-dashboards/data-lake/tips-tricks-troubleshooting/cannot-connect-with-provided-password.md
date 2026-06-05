---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: A ferramenta Power BI não conseguiu se conectar com a senha fornecida
description: Ao tentar fazer logon no Data Connect pela ferramenta do Power BI, você recebe um erro de logon.
author: Courtney
feature: Reports and Dashboards
exl-id: c3f2b4a9-0831-48f0-871b-486d09ae5ea4
TQID: https://experienceleague.adobe.com/Z4RrMAPGd3CCti-cQFiJ7hlf-h8-suXeuoYfzk-9aKo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 229
ht-degree: 5%

---

# A ferramenta Power BI não consegue se conectar com a senha fornecida

## Problema

Ao tentar fazer logon no Data Connect a partir da ferramenta Power BI, você vê o seguinte erro:

`Cannot connect from BI tool with provided password`

## Causa

Ao criar a conexão JDBC, o Workfront fornece uma senha temporária para a Conexão de dados.

Antes de acessar a Conexão de dados por meio do Power BI, primeiro faça logon usando os detalhes de conexão fornecidos, atualize a senha temporária e prossiga com o logon.


## Solução

Redefina a senha da conexão no Workfront e crie uma nova senha com o link fornecido na caixa de diálogo Editar conexão.

### Redefinir senha de conexão no Workfront

1. Acesse Workfront > Configuração > Sistema > Conexão de dados.
1. Localize e abra a conexão na lista.
1. Em **Redefinir Senha da Conexão**, marque a caixa para confirmar se deseja redefinir a senha.
1. Clique em **Redefinir Senha da Conexão**.
   ![redefinir senha de conexão](assets/reset-password.png)
1. Prossiga para a seção abaixo.

### Criar uma nova senha para a conexão

1. Copie o URL e cole-o em uma nova guia do navegador.
1. No Workfront, copie e cole o Nome de usuário da conexão e a Senha padrão na nova guia do navegador.
   ![copiar url e senha padrão](assets/link-password.png)
1. Clique em **Fazer logon**.
1. Digite uma nova senha e clique em **Enviar**.
1. Acesse a ferramenta Power BI e faça logon com a nova senha.
