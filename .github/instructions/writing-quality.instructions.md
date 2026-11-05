---
description: Padrões técnicos de escrita do Workfront para artigos de ajuda. Aplica os princípios Guia de estilo de documentação do Workfront e Desenvolvimento de informações técnicas de qualidade (DQTI).
applyTo: "help/**/*.md"
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 1%
---

# Qualidade de escrita

Aplicar esses padrões sempre que editar, revisar ou escrever um artigo de ajuda.
Preserve a intenção e a precisão técnica do autor. Para o completo
pontuação, terminologia, capitalização e referência de procedimento, ler
[.cursor/skills/writing-quality/reference.md](../../.cursor/skills/writing-quality/reference.md).

**não** aplique essas regras às notas de versão em
`help/quicksilver/product-announcements/product-releases/` — use o
instruções de release-notes-formatter em vez disso.

## Voz e ponto de vista

- Use **segunda pessoa** (&quot;Você pode...&quot;) ao endereçar o leitor.
- Use contrações para um tom de conversação (não, não pode, é, eles são).
- Use &quot;Recomendamos&quot; para práticas recomendadas — não &quot;É recomendado&quot; ou &quot;Você deveria&quot;.
- Ao escrever para um grupo de usuários, faça referência a outras funções em terceiros.
- Nunca use pronomes de gênero — reestruturar a frase ou usar &quot;eles&quot;.
- Sem barra para opções — use &quot;ou&quot; (&quot;ele ou ela&quot; e não &quot;ele/ela&quot;).

## Clareza (DQTI)

- Uma ideia por frase; mantenha as sentenças abaixo de ~25 palavras quando possível.
- Iniciar com a ação ou o resultado, não o contexto do plano de fundo.
- Use a palavra mais simples (&quot;usar&quot; não &quot;utilizar&quot;, &quot;iniciar&quot; não &quot;iniciar&quot;).
- Evite nomeações (&quot;criar&quot; não &quot;a criação de&quot;).
- Use uma linguagem específica e concreta — evite termos vagos (&quot;vários&quot;, &quot;vários&quot;).
- Evite negativos duplos.

## Concretização e orientação de tarefas (DQTI)

- Use exemplos específicos com valores realistas; nomeie elementos e campos exatos da interface do usuário.
- Concentre-se no que o usuário pode *fazer*, não no que o sistema *é*.
- Conduzir procedimentos com verbos imperativos (&quot;Criar uma tarefa&quot;, &quot;Configurar notificações&quot;).
- Forneça contexto suficiente para agir, mas não mais.
- Incluir um link para a ajuda detalhada (&quot;Para obter mais informações, consulte o [artigo].&quot;).

## Uso de letras maiúsculas

- **Cabeçalhos**: caso de sentença sempre (&quot;Criar uma tarefa&quot;, não &quot;Criar uma tarefa&quot;).
- **Termos do Workfront**: use letras maiúsculas somente ao fazer referência direta a um elemento da interface do usuário.
  - Direto: &quot;Preencha o campo Data de conclusão planejada&quot;.
  - Indireto: &quot;Cada tarefa deve ter uma data de conclusão planejada&quot;.
  - Dica: se você puder colocar &quot;o&quot; ou &quot;a&quot; na frente do termo, ele geralmente ficará em minúsculas.
- **Botões**: siga as letras maiúsculas da interface do usuário; os botões com todas as letras maiúsculas tornam-se letras maiúsculas e minúsculas.
- **Funções**: &quot;Administrador do Sistema&quot; para a função na interface do usuário; &quot;Workfront
administrador&quot; para a pessoa.

## Cabeçalhos

- Comando imperativo em caso de sentença, baseado em tarefa (&quot;Configurar níveis de acesso&quot;).
- Os artigos de visão geral terminam com &quot;visão geral&quot; (&quot;Visão geral dos projetos&quot;).
- Divida seções longas em vários cabeçalhos com submetas claras.

## Referências cruzadas e links

| Situação | Formato |
|-----------|--------|
| Vincular após fornecer informações | &quot;Para obter mais informações, consulte [Nome do artigo].&quot; |
| Link sem informações anteriores | &quot;Para obter informações, consulte [Nome do artigo].&quot; |
| Link para uma seção em outro artigo | &quot;Para obter mais informações, consulte [Nome da seção] em [Nome do artigo].&quot; |
| Link para uma seção no mesmo artigo | &quot;Para obter mais informações, consulte [Nome da seção] neste artigo.&quot; |

- Em um parágrafo: em linha. Em uma etapa de procedimento: em uma nova linha após a etapa.
- Vários links: use uma lista com marcadores.
- Use &quot;canto superior direito&quot; / &quot;canto superior esquerdo&quot; para posições de tela.

## Negrito e itálico

- **Ações clicáveis** em negrito e elementos da interface **somente nas etapas de procedimento**.
- Não colocar em negrito elementos da interface, nomes de caixas de diálogo, nomes de páginas, nomes de ícones ou menu
nomes fora das etapas de procedimento.
- Use *itálico* para o texto que o usuário deve digitar (&quot;Type *my.workfront.com*...&quot;).
- Nunca use itálico para ênfase — reestruturar a frase em vez disso.

## Notas, dicas e avisos

Use com moderação. O uso excessivo os torna invisíveis.

- Máximo de uma nota/dica/aviso por seção; nunca os empilhe.
- Combinar notas relacionadas em uma nota com uma lista com marcadores.
- Não use notas para anunciar novas funcionalidades — retrabalhe o texto do artigo.

| Tipo | Finalidade |
|------|---------|
| `>[!NOTE]` | Informações que não se encaixam no parágrafo; controle de versão/compatibilidade |
| `>[!TIP]` | Sugestões interessantes que facilitam a vida do usuário |
| `>[!IMPORTANT]` | Informações vitais para a etapa ou procedimento |
| `>[!WARNING]` | Alertar o usuário sobre possível perda de dados |

## Procedimentos

- Use cabeçalhos de comando imperativos; introduções somente quando necessário.
- Formato de introdução preferencial: frase infinitiva + dois pontos (&quot;Para criar uma variável
senha:&quot;).
- Os procedimentos de etapa única ainda usam uma lista numerada.
- Use &quot;type&quot; ou &quot;select&quot; — evite palavras vagas como &quot;set&quot; ou &quot;specified&quot;.
- Etapas condicionais: &quot;(Condicional) Se você for membro de mais de uma equipe,
selecione...&quot;. Etapas opcionais: &quot;(Opcional) Para adicionar um emoji, clique em...&quot;.
- Descreva a resposta do sistema antes que ocorra ou imediatamente depois.
- Vários métodos: documente primeiro a maneira mais simples e, em seguida, use &quot;Ou&quot;.
- Navegação de menu/guia: &quot;Clique em **Email** > **Notificações**&quot; (negrito para os nomes, não
os colchetes; espaços ao redor dos colchetes). Não usar colchetes no menu principal
navegação — use o trecho do menu principal.

## Referência rápida de pontuação

| Regra | Exemplo |
|------|---------|
| Vírgula de Oxford sempre | &quot;motivo, meios e oportunidade&quot; |
| Vírgula antes de &quot;then&quot; em procedimentos | &quot;Clique em Configurar e depois em Interface.&quot; |
| Vírgula após ano em uma data no meio da frase | &quot;A edição de 2 de janeiro de 2016 do...&quot; |
| Sem vírgula com mês-ano apenas | &quot;Janeiro de 2016&quot; |
| Dois pontos antes de uma lista, minúsculas depois de | &quot;Selecione uma das opções a seguir: opção A&quot; |
| Nenhum sinal de dois pontos após os cabeçalhos do procedimento | &quot;Criar uma tarefa&quot; |
| Traços eme com moderação | Reestruturar a sentença, se possível |
| Períodos em extensões de arquivo | &quot;Carregar um arquivo PDF&quot; |

## Organização (DQTI)

- Estrutura lógica com divulgação progressiva (visão geral → detalhes → referência).
- Um tópico por seção; use listas para mais de 3 itens paralelos.
- Mantenha os itens da lista e seus leads em paralelo gramaticalmente.
- Use tabelas para comparações estruturadas ou descrições de campo.
- Evite parágrafos na parede do texto — quebre em partes digeríveis.

## Lista de verificação de validação

- [ ] Segunda pessoa através de, contrações usadas.
- [ ] Primeira letra da sentença em maiúscula em todos os cabeçalhos.
- [ ] termos do Workfront escritos corretamente em maiúsculas (referência direta ou indireta).
- [ ] Negrito somente em ações clicáveis nas etapas de procedimento.
- [ ] As referências cruzadas usam o formato padrão.
- [ ] Notas/dicas/avisos não empilhados, máx. um por seção.
- [ ] Vírgula de Oxford usada de forma consistente.
- [ ] As etapas do procedimento usam verbos específicos (digite, selecione, clique).
- [ ] Etapas condicionais/opcionais rotuladas corretamente.
- [ ] Nenhum pronome de gênero.
- [ ] Frases são claras, concretas e orientadas a tarefas; a estrutura paralela é mantida.
