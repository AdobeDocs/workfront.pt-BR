---
source-git-commit: b3148e5706abd75f2dd260f32507dedf8e259f57
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 1%

---
# Mensagens de Git commit

Sempre aplique esta regra. Ao rascunhar ou gerar uma mensagem de confirmação do Git (por exemplo, na caixa de confirmação do Source Control ou quando solicitado no bate-papo do agente), siga esse formato.

## Linha de assunto (somente primeira linha)

- Cerca de **50 caracteres ou menos**.
- Resuma a alteração no **humor imperativo** (por exemplo, &quot;Adicionar...&quot;, &quot;Corrigir...&quot;, &quot;Refatorar...&quot;).

## Linha em branco

Deixe uma **linha em branco** após o assunto antes do corpo da mensagem.

## Corpo (descrição detalhada)

- Quebrar linhas com aproximadamente **72 caracteres** (incluindo o prefixo do marcador e o espaço).
- Use **linhas de marcador** para a explicação. Cada marcador deve começar com exatamente um de:
   - **📖** — use quando a alteração **adicionar** algo novo: novos arquivos, novas seções, novos recursos, novos cabeçalhos, novas linhas ou outro conteúdo de greenfield.
   - **✏️** — use quando a alteração **modificar** o trabalho existente: edições em linhas existentes, atualizações em seções existentes, refatoração de código existente ou alterações no conteúdo atual.

Aplique **📖** ou **✏️** a cada marcador do corpo, de modo que fique claro o que foi introduzido em relação ao que foi alterado.

## Modelo

Preencha os espaços reservados (não deixe colchetes na mensagem final):

```
<Summarize change(s) in around 50 characters or less>

<More detailed explanatory description of the change wrapped into about 72
characters with bullets. >
```

## Exemplo

```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```
