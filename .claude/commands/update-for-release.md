---
name: update-for-release
description: ""
source-git-commit: 4c2305da7635694d9d7bc174b5837a0d57fb7ac0
workflow-type: tm+mt
source-wordcount: '2009'
ht-degree: 0%

---


# Atualização para lançamento (Workfront)

Essa habilidade aborda a atualização de artigos de ajuda do Workfront para uma versão futura de recursos. O fluxo de trabalho é o inverso de `remove-preview-highlighting`: o novo comportamento está sendo adicionado aos artigos, marcados como Pré-visualização e (posteriormente, no GA) limpos por essa outra habilidade.

## Escopo

Aplicar quando **todos** forem verdadeiros:

1. O usuário está atualizando os artigos de ajuda do Workfront para um recurso que está sendo enviado (normalmente, Visualizar primeiro).
2. A alteração introduz um novo comportamento ou interface do usuário, não uma limpeza de DG. Para limpeza de GA, use **remove-preview-highlighting**.
3. O arquivo **não** é uma nota de versão. Para notas de versão, use **release-notes-formatter**.
4. O usuário forneceu o contexto do recurso: no mínimo, uma descrição curta e uma captura de tela; idealmente um URL PRD (Adobe Wiki).

Se o escopo não estiver claro, confirme antes de iniciar.

## Fluxo de trabalho necessário (humano no loop)

Faça **não** edição em massa do repositório. Mova um artigo de cada vez. Após cada artigo, pergunte se deseja continuar no próximo.

### &#x200B;1. Coletar contexto de recurso

Confirme com o usuário:

- **O que mudou** (resumo de 1-2 frases do novo comportamento ou interface do usuário).
- **Captura(s) de tela** da nova interface. Se fornecido, salve na pasta `assets/` do artigo de destino com um nome de arquivo kebab-case descritivo (por exemplo, `add-custom-message.png`). Se não for fornecido, pergunte se deve aguardar um ou continuar com uma referência de espaço reservado.
- **PRD URL** (Adobe Wiki), se disponível. Busque-o com a ferramenta `get_wiki_content` do MCP `user-Adobe Wiki Confluence`. Leia-o para encontrar comportamentos que o usuário não pode ver na interface do usuário: efeitos colaterais de notificação, o que acontece quando algo é editado ou adicionado posteriormente, limites de caracteres não exibidos, permissões etc.
- **Disponibilidade**: somente visualização, Visualização + versão rápida ou já disponível. Isso direciona a escolha do trecho na etapa 3.
- **Exclusões explícitas**: todos os artigos que o usuário deseja ignorar (por exemplo, &quot;este recurso não está em modelos&quot;).

### &#x200B;2. Artigos afetados pelo inventário

Pesquise o repositório com as palavras-chave da área de recursos (por exemplo, `approval workflow`, `document approval`, o rótulo de campo específico). Criar uma lista de candidatos:

- Artigos explicativos na árvore `help/quicksilver/.../` relevante.
- Artigos de visão geral e perguntas frequentes que mencionam a área de recursos.
- **Excluir** `product-announcements/` (as notas de versão usam uma habilidade diferente).
- **Excluir** páginas de índice/índice nas quais a única menção é o texto do link para outro artigo.
- **Excluir** artigos que o usuário disse para ignorar na etapa 1.

Apresentar a lista de candidatos ao usuário. Pergunte o que atualizar e o que ignorar. Referência cruzada `help/quicksilver/TOC.md` se um artigo irmão parecer ausente.

### &#x200B;3. Escolha o trecho de visualização

Leia `help/_includes/snippets.md` e escolha por disponibilidade:

| Disponibilidade | Trecho |
| --- | --- |
| Somente visualização — o conteúdo destacado é novo em um artigo disponível ao público em geral | `{{highlighted-preview}}` |
| Somente visualização — todo o artigo é novo | `{{highlighted-preview-article-level}}` |
| Pré-visualização + clientes de lançamento rápido, geral | `{{preview-fast-release-general}}` |

Se um trecho específico da versão já existir para o trimestre atual, prefira isso ao genérico. Confirme a escolha com o usuário antes de aplicar.

### &#x200B;4. Por artigo — mostrar primeiro, editar após OK

Para cada artigo na lista confirmada pelo usuário:

1. **Leia o arquivo.**

2. **Determinar o padrão de realce.** Pergunte ao usuário que se encaixa neste artigo (a resposta pode diferir de acordo com o artigo):

   - **Duplicação por seção**: anexar `in Production` ao cabeçalho de seção existente. Adicione uma nova seção com `in Preview` anexada, encapsulada em `<div class="preview"> ... </div>`. Use quando o novo comportamento altera o procedimento de forma significativa — etapas extras ou reordenadas, uma nova imagem ou texto de etapa diferente. Típica para procedimentos de instrução.
   - **Duplicação por linha**: para uma descrição de campo baseada em tabela em que apenas uma linha é alterada e o restante da tabela/procedimento permanece inalterado, deixe a linha byte por byte existente inalterada e adicione um novo `<tr class="preview">` diretamente após ela. Não teça novas frases na linha original. Consulte &quot;Duplicação por linha&quot; em Regras de conteúdo para obter as convenções exatas.
   - **Encapsulamento por linha**: adicione a(s) nova(s) frase(s) embutida(s) dentro da seção existente, encapsulada em `<span class="preview"> ... </span>`. Use quando a adição for uma frase ou duas que se encaixem naturalmente em um parágrafo existente ou em uma resposta de perguntas frequentes (não uma linha da tabela — use a duplicação por linha para essas perguntas).
   - **Misto**: algumas seções no mesmo artigo usam padrões diferentes para conteúdo diferente. Use essa opção quando o artigo misturar tabelas de procedimentos, seções de estilo de perguntas frequentes e parágrafos simples.

3. **Coloque o trecho** em sua própria linha imediatamente após o cabeçalho H1, com uma linha em branco acima e abaixo. O trecho fica **antes** do parágrafo de introdução.

4. **Armazenar novos detalhes em &quot;sempre incluir&quot; vs. &quot;pronto para revisão&quot;.** Este é o passo mais importante.

   - **Sempre incluir** (aplicar automaticamente, sem prompt): comportamentos invisíveis que o usuário não pode observar ao interagir com a interface. Exemplos:
     - Efeitos colaterais (por exemplo, &quot;editar novamente o email para todos os participantes&quot;)
     - Comportamento em outros objetos ou eventos posteriores
     - Pré-requisitos e permissões
     - Limites não mostrados na interface
     - Tudo o que o usuário pode aprender somente com o PRD, os documentos ou a equipe de produtos
   - **Acima para revisão** (presente ao usuário com `AskQuestion` como uma seleção múltipla): fatos que o usuário pode ver na tela ao usar o recurso. Exemplos:
     - Um contador de caracteres que a interface do usuário já mostra (ex.: `0 / 500`)
     - O estado expandido/recolhido padrão de um campo
     - Estado padrão selecionado de uma caixa de seleção visível
     - Rótulos de botão ao lado do campo
     - Mensagens de validação que aparecem em linha

   Para cada item &quot;up for review&quot;, forneça uma lógica de uma frase (&quot;Ajuda os novatos a planejar uma mensagem mais longa&quot;, &quot;Ajuda os usuários que não a veem em estágios posteriores a saberem expandi-la&quot;). Inclua apenas os itens que o usuário escolher. O princípio padrão é &quot;se o usuário puder vê-lo na tela enquanto está fazendo a tarefa, não reitere&quot; — mas o usuário recebe a chamada final.

   **Ao redigir as sentenças reais** para qualquer um dos compartimentos, aplique `~/.cursor/skills/writing-quality/SKILL.md` regras de voz e tom enquanto escreve — uma descrição de campo/comportamento simples, não uma entrada de log de alterações (&quot;foi removido&quot;, &quot;foi adicionado&quot;) e não reafirme uma instrução inalterada apenas para anexar uma nota de visualização a ela. Faça o rascunho certo na primeira vez em vez de corrigir o tom em uma passagem posterior.

5. **Faça uma aprovação final na qualidade de gravação** no texto em rascunho antes de mostrá-lo. Essa é uma rede de segurança, não a primeira vez que essas regras se aplicam — capture qualquer etapa 4 perdida (redundância, tom, incompatibilidade de voz com linhas ao redor).

6. **Propor edições.** Mostrar trechos antes/depois (ou uma descrição focalizada no estilo diff) do artigo, abrangendo: inserção de trechos, renomeações de cabeçalhos, novo conteúdo na Pré-visualização e onde ele se encontra, referência de captura de tela e quaisquer `class="preview"` wraps incorporados.

7. **Aguarde a aprovação explícita** (&quot;ok&quot;, &quot;apply&quot;, &quot;yes&quot;) antes de gravar o arquivo.

8. **Validar.** Depois de gravar, execute `ReadLints` no arquivo e relate quaisquer problemas. Leia novamente a seção alterada para confirmar a estrutura.

### &#x200B;5. Após cada artigo

Pergunte se deseja mover para o próximo artigo, parar, ignorar ou revisitar o atual.

### &#x200B;6. Fim de sessão — copiar/colar nota de versão

Quando o usuário terminar a sessão (diz &quot;concluído&quot;, &quot;é isso&quot;, &quot;parar&quot; ou não quer continuar no próximo artigo), pergunte:

> &quot;Deseja copiar/colar a entrada da nota de versão para a página de aprimoramento?&quot;

Em caso afirmativo, gere uma entrada de rascunho usando o contexto do recurso da etapa 1 e o artigo de ajuda principal atualizado nesta sessão. **Não o grave em nenhum arquivo** — forneça-o somente como copiar/colar texto.

Formate a entrada para corresponder à estrutura da página de área de produto da habilidade **notas-de-versão-formatter**:

```markdown
## {Feature name}

>[!NOTE]
>
>Preview: {date or TBD}
>Production fast release: {date or TBD}
>Production for everyone: {date or TBD}

{1–3 sentences describing what changed and why it helps users. Lead with the benefit, not the UI action.}

For more information, see [{Primary article title}](/help/quicksilver/{path-to-article}.md).
```

Regras:

- Use `TBD` para qualquer data ainda não conhecida; pergunte ao usuário se ele tem as datas.
- O nome do recurso é primeira letra maiúscula e os substantivos próprios.
- A descrição deve se concentrar no que os usuários agora podem fazer, não nos detalhes de implementação.
- O link para o artigo de instruções mais específico foi atualizado, não uma página de visão geral.
- Não inclua um bloco de datas `>[!NOTE]` se todas as datas forem desconhecidas e o usuário não quiser espaços reservados — omita-o e observe que ele precisa ser adicionado posteriormente.

## Regras de conteúdo

### Cabeçalhos

- Anexe exatamente **`in Production`** aos cabeçalhos de seção existentes que permanecem como referência do lado da produção.
- Acrescentar exatamente **`in Preview`** aos novos títulos de seção.
- Mantenha o restante do cabeçalho em maiúsculas e minúsculas (por `writing-quality`).

### Visualizar invólucros

- **Nível de seção**: quebra automática em `<div class="preview"> ... </div>`. Coloque tags de abertura e fechamento em suas próprias linhas, com uma linha em branco acima e abaixo de cada tag, de modo que os cabeçalhos e listas dentro ainda sejam renderizados.
- **Inline (nível de frase)**: quebra automática em `<span class="preview"> ... </span>` dentro do parágrafo, célula de tabela ou resposta da Pergunta frequente existente.
- Nunca aninhe um `<span class="preview">` dentro de um `<div class="preview">`.

### Duplicação por linha

Para uma descrição de campo baseada em tabela em que apenas o *comportamento* do campo é alterado (não o procedimento ao redor):

- Deixe o `<tr>` existente completamente inalterado — ele agora representa o comportamento atual/de produção. Nunca cole novas frases ou extensões nela.
- Adicione uma nova linha diretamente após ela:

  ```html
  <tr class="preview">
  <td><span class="preview"><strong>{new label} in preview</strong></span></td>
  <td><span class="preview">{self-contained description}</span></td>
  </tr>
  ```

- **Rótulo**: não use apenas o rótulo de campo original e anexe `(in Preview)`. Escreva um rótulo curto e natural para o novo recurso em si (por exemplo, rótulo original &quot;Adicionar nomes ou emails&quot; → novo rótulo &quot;Adicionar pessoas ou equipes&quot;), em seguida, anexe `in preview` em minúsculas sem parênteses: &quot;Adicionar pessoas ou equipes na pré-visualização&quot;.
- **Descrição**: escreva uma descrição de frase 1-3 nova somente sobre o novo comportamento, na voz existente do artigo. Não reutilize as frases da linha original como base e insira adições nelas — a nova linha deve ler como uma descrição completa e independente por conta própria.
- **Observações complementares**: anexe com uma quebra de linha `<br>` seguida de `Note:` na próxima linha, dentro do mesmo `<span class="preview">` — não aninhe um `<p>Note: ...</p>`. Como a nova linha é independente, reafirme qualquer fato ainda relevante da nota da linha original brevemente aqui, em vez de assumir que o leitor também o viu (por exemplo, uma restrição &quot;um estágio aberto por vez&quot; no modo Avançado que se aplica igualmente à nova linha).
- **Várias variantes**: se o mesmo campo estiver sendo atualizado em mais de um procedimento no mesmo artigo (Básico versus Avançado, herdado versus ESM e assim por diante) e o comportamento subjacente realmente diferir entre elas (por exemplo, o herdado mantém um padrão de aceitação enquanto o ESM sempre se expande), escreva cada linha para corresponder ao comportamento real dessa variante. Não copie as palavras de uma variante na linha de outra.

### Posicionamento do trecho

- A linha de trecho vai imediatamente após o H1, com uma linha em branco acima e abaixo.
- O trecho fica **antes** do parágrafo de introdução, da chamada `>[!IMPORTANT]` e de qualquer bloco de requisitos de acesso.
- Um trecho por artigo.

### Capturas de tela

- Salve novas capturas de tela na pasta `assets/` do artigo com um nome de arquivo de caso kebab descritivo.
- Faça referência à nova captura de tela na nova seção Visualização. Se a captura de tela de uma seção em produção não refletir mais o recurso com precisão, deixe-a no lugar — ela ainda representa o comportamento de produção até a data de disponibilidade geral.
- Não fabrique nomes de arquivo de captura de tela; se nenhuma captura de tela tiver sido fornecida ainda, pergunte ao usuário.
- **Espaço reservado para uma captura de tela que ainda não existe**: se o usuário quiser continuar sem aguardar o ativo, adicione um comentário do HTML diretamente após a referência de captura de tela existente (produção), reutilizando esse nome de arquivo com um sufixo `-v2`:

  ```html
  <!--
  preview screen![{same alt text}](assets/{existing-filename}-v2.png)
  -->
  ```

  Troque a referência real (e remova o comentário) assim que a captura de tela for fornecida.

### Notas e dicas

- Máximo de um `>[!NOTE]` (ou `>[!TIP]`, `>[!IMPORTANT]`, `>[!WARNING]`) por seção. Se a seção existente já tiver uma nota, combine o novo conteúdo relacionado na mesma nota como uma lista com marcadores em vez de empilhar.

### O que não fazer

- Não editar artigos em `product-announcements/`.
- Não edite em massa; um artigo de cada vez, com aprovação explícita a cada vez.
- Não inclua fatos observáveis da interface do usuário sem exibi-los ao usuário primeiro.
- Não modifique o conteúdo nos comentários do HTML `<!-- ... -->`, a menos que o usuário diga explicitamente para.
- Não altere `author:` ou campos de material de frente não relacionados.

## Verificações de qualidade antes de apresentar edições

Executar esta lista de verificação completa para **a cada** artigo na sessão — incluindo artigos secundários nos quais você está &quot;apenas adicionando um marcador&quot;, não apenas o primeiro/principal.

- O trecho aparece uma vez, em sua própria linha, depois do H1, com linhas em branco acima e abaixo.
- Os cabeçalhos de seção existentes terminam com `in Production`.
- Os novos cabeçalhos de seção terminam com `in Preview` e a seção está dentro de `<div class="preview">`.
- Adições embutidas estão dentro de `<span class="preview">`.
- Duplicações por linha: o original `<tr>` é byte por byte inalterado; o novo `<tr class="preview">` tem ambas as células encapsuladas em `<span class="preview">`; o rótulo é um rótulo novo curto + minúsculas &quot;na pré-visualização&quot; (não o rótulo original + &quot;(na Pré-visualização)&quot;); qualquer nota suplementar usa `<br>` + `Note:` embutido, não um `<p>` aninhado.
- Se o mesmo campo aparecer em mais de uma variante de procedimento (Básico/Avançado, herdado/ESM), cada nova linha da redação corresponderá ao comportamento real dessa variante em vez de ser copiada e colada de outra variante.
- A nova prosa marcada como pré-visualização é lida como uma descrição de campo/comportamento simples, não uma entrada de log de alterações, e não reafirma redundantemente uma instrução inalterada.
- `ReadLints` está limpo no arquivo editado.
- O artigo é lido corretamente em ambos os estados (com o conteúdo da pré-visualização exibido e oculto).

## Referências

- Estilo da documentação do Workfront: consulte a habilidade **qualidade de escrita** em `~/.cursor/skills/writing-quality/SKILL.md`.
- Catálogo de trechos: `help/_includes/snippets.md` no repositório de documentos.
- Limpeza de GA (fluxo de trabalho inverso): consulte a habilidade **remove-preview-highlighting** em `.cursor/skills/remove-preview-highlighting/SKILL.md`.
- Adobe Wiki MCP para PRDs: servidor `user-Adobe Wiki Confluence`, ferramenta `get_wiki_content`.
