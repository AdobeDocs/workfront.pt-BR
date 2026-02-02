---
title: 'Manual: dimensionamento gerenciado, após a primeira vitória'
description: Saiba como implantar o Adobe Workfront Planning após sua primeira implementação bem-sucedida
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 28913661935d5a030cb33dd204fcb3c08daf0b26
workflow-type: tm+mt
source-wordcount: '2025'
ht-degree: 0%

---


# Manual: dimensionamento gerenciado, após a primeira vitória

**Versão**: 1.0

**Contexto**: &quot;Chegamos ao nosso primeiro caso de uso e agora todos querem entrar.&quot;



## &#x200B;1. A &quot;Armadilha de Sucesso&quot;

Às vezes, pode parecer que a fase mais perigosa da adoção do WFP é imediatamente após o primeiro caso de uso bem-sucedido ou POC. O entusiasmo é grande, mas o medo da &quot;dívida técnica&quot; e da &quot;expansão administrativa excessiva&quot; pode levar a duas respostas igualmente prejudiciais:

1. **Governança excessiva**: bloquear o sistema tão rigorosamente que novas equipes revertem para planilhas.

2. **Governança zero**: permitir que cada equipe crie seus próprios campos e tipos de registro, recriando a subutilização de metadados fragmentados encontrada em ambientes herdados.



## &#x200B;2. A filosofia central: WFP como o &quot;mecanismo de reconciliação&quot;

Em vez de tentar impedir que as equipes sejam diferentes, posicionamos o WFP como o local onde essas diferenças são **tornadas visíveis para que possam ser reconciliadas**.



* **Gerenciamento da adoção Velocity**: é natural ter cautela com a expansão para uma nova ferramenta antes de &quot;limpar&quot; os ambientes existentes. Embora a opção de **Simplificar Primeiro** forneça uma base altamente controlada, ela pode atrasar o tempo de implantação das equipes prontas para alinhamento. Acreditamos que a maneira mais eficaz de conduzir essa alteração é reconhecer que a **visibilidade é a Etapa 1**. O ímpeto em direção a uma ferramenta compartilhada e pronta para a empresa (afastando-se da proliferação de PPTs e planilhas) é o que finalmente desbloqueia objetivos de longo prazo.



  **Recomendação**: em vez de uma exigência de &quot;Limpeza primeiro&quot;, recomendamos alocar uma parte menor dos recursos para a manutenção contínua e uma parte significativamente maior para solucionar necessidades comerciais urgentes. Por exemplo, passar um ano apenas &quot;limpando&quot; taxonomias rende pouco valor incremental. No entanto, oferecer **visibilidade entre equipes** (por exemplo, por meio de um Calendário corporativo unificado ou de um roteiro de GTM consolidado) fornece o valor transformador de que suas partes interessadas precisam, ao mesmo tempo que fornece a estrutura de dados unificada necessária para administrar o ambiente ao longo do tempo.

* **Reconheça a realidade**: as equipes independentes desenvolvem naturalmente seus próprios processos, que geralmente ficam ocultos em planilhas isoladas. A transição para o PAM não cria uma confusão; ela ilumina aquela que já existe. Ao tornar esses processos visíveis em um ambiente compartilhado, você os coloca em um lugar onde eles podem finalmente ser abordados e aprimorados.

* **O sinal de progresso**: quando uma equipe solicita seus próprios campos, não é &quot;subutilização&quot;; é **Adoção**. Significa que eles veem o WFP como seu espaço de trabalho.

* **Gerenciar Dívida, Não Ocultar**: é natural se preocupar com o esforço necessário para limpar taxonomias divergentes posteriormente. No entanto, a alternativa — forçando padrões rigorosos muito cedo — muitas vezes leva as equipes de volta às planilhas onde seus processos (e suas dívidas) permanecem ocultos. Ao permitir que as equipes comecem no WFP com suas classificações atuais, você está movendo essa dívida para um ambiente visível e governado. Isso faz da reconciliação final uma tarefa iterativa em vez de um projeto de migração único e esmagador.



## &#x200B;3. O modelo de governação das &quot;vias rodoviárias&quot;

Escale sem dívidas definindo &quot;Pistas Globais&quot; e &quot;Playgrounds Locais&quot;.



### A. As rotas globais

* **Objetos Controlados**: objetos que cada equipe deve usar para os relatórios da empresa (por exemplo, `Strategic Pillar`, `Region`, `Fiscal Quarter`).

* **Gerenciado Por**: O Administrador Central De COE/Operações De Marketing.

* **Regra**: esses campos são &quot;Compartilhados&quot; e obrigatórios.



### B. Os Playgrounds locais (Raios)

* **Objetos experimentais**: campos ou tipos de registro específicos às necessidades táticas de uma equipe (por exemplo, `Influencer Handle` de uma equipe do Social ou `URL Slug` de uma equipe da Web).

* **Gerenciado por**: O Líder da Equipe (com orientação simples).

* **Regra**: as equipes podem inovar aqui. Se um campo &quot;Local&quot; é adotado por >3 equipes, é &quot;Promovido&quot; a uma pista global.



## &#x200B;4. O Paradoxo Da Governança: Equipes Em Primeiro Lugar, Padrões Seguem

Um desafio comum no dimensionamento do WFP é decidir qual vem primeiro: **Governança Empresarial** ou **Alinhamento Operacional da Equipe**.



Acreditamos que a maneira mais eficiente de fazer isso é reconhecer que o valor empresarial é construído em uma rua de mão dupla:

1. **As equipes precisam de relevância**: a empresa só percebe valor quando suas equipes estão em execução ativa. Portanto, a governança deve **atender às equipes**, fornecendo uma estrutura que ofereça suporte às suas necessidades operacionais conhecidas.

2. **A Empresa precisa de visibilidade**: a Liderança só pode tomar decisões informadas quando os dados estiverem limpos o suficiente para serem agregados. Portanto, as equipes devem **atender à empresa** fornecendo os metadados viáveis mínimos necessários para a visibilidade do portfólio.



O objetivo da &quot;escala gerenciada&quot; é encontrar a interseção dessas duas necessidades — padronizar o suficiente para fornecer visibilidade, mas não tanto para interromper a execução da equipe.



### A. Alinhamento de prioridades: dados vs. visualização

Ao dimensionar, reconheça que a definição de &quot;Valor&quot; difere entre as personas:

* **O Proprietário de Admin/Produto**: Valores de **taxonomias e classificações unificadas**. Sua meta é uma arquitetura de dados limpa que ofereça suporte à escalabilidade a longo prazo.

* **A Parte Interessada/Líder**: Valores de **visualização e insight** (por exemplo, um Calendário Global ou uma Linha do Tempo do Portfolio). Seu objetivo é o &quot;Momento Relâmpago&quot; que torna os dados acionáveis.



**A Estratégia**: Use a necessidade de visualização das partes interessadas como o *incentivo* para que a equipe esteja em conformidade com a necessidade de padrões de dados do administrador. Você obtém a taxonomia unificada fornecendo o &quot;Super Calendário&quot; que a liderança exige.



### B. A Fase De Observação &quot;Liderada Por Serviços&quot;

Durante o scale-up inicial, o papel do administrador é facilitar esse intercâmbio entre as equipes e a empresa.

* **Priorizar a Operação em vez da Padronização**: é melhor ter equipes planejando ativamente em espaços de trabalho isolados do que paralisá-las devido à falta de definições globais. Essa atividade são os &quot;dados brutos&quot; necessários para criar padrões saudáveis e reais.

* **Identificar os &quot;Mínimos de visibilidade&quot;**: trabalhe com liderança para identificar os 3 a 5 campos que *deve* limpar para os relatórios da empresa (por exemplo, `Strategic Alignment`, `Start Date`, `Budget`). Concentre sua energia de fiscalização SOMENTE aqui.



### B. Harmonização retroativa (governação como serviço)

Assim que surgir um padrão de &quot;necessidades conhecidas&quot; entre as equipes, a empresa poderá consolidar esses padrões em um serviço global.

1. **Observar padrões bem-sucedidos**: identifique as taxonomias &quot;vencedoras&quot; que as equipes já criaram e adotaram.

2. **O Handshake Colaborativo**: junte os campeões de equipe para refinar os sucessos locais em um padrão corporativo compartilhado.

3. **Implantar como um serviço**: implante as novas faixas globais não como uma &quot;restrição&quot;, mas como uma maneira de simplificar os relatórios e o alinhamento entre equipes para as pessoas que estão fazendo o trabalho.



**Principais argumentos**: a governança deve ser uma resposta ao sucesso operacional, não um pré-requisito para ela.



## &#x200B;5. Mecânica de dimensionamento: o modelo de crescimento baseado em padrões

A aplicação dessa filosofia requer uma abordagem cuidadosa da estrutura de dados. Para evitar a &quot;Subutilização de governança&quot;, resista ao anseio de criar campos globais para cada solicitação individual. Em vez disso, use o **Caminho de maturidade do campo** para permitir que o uso real oriente seus padrões corporativos:



1. **Nível 1: Experimento local**: a Equipe A cria um campo personalizado em seu espaço de trabalho.

2. **Nível 2: Reconhecimento de Padrão**: Os Administradores percebem que as Equipes B e C estão usando ou solicitando um campo semelhante.

3. **Nível 3: Padronização Empresarial**: o Administrador cria uma única versão padronizada desse campo como um tipo de registro na **Workspace de Taxonomia Global** e a associa às equipes.



### A Mecânica da &quot;Aposentadoria Suave&quot;

Como o WFP não tem um recurso nativo de &quot;Arquivamento&quot; para campos, retirar um campo local requer um processo deliberado de &quot;Aposentadoria Temporária&quot; para preservar dados históricos sem desorganizar a interface do usuário:



1. **Migração de Dados**: Use uma exibição de tabela (ou Fusion) para copiar valores em massa do campo &quot;Sombra&quot; local para o novo campo Faixa Global. Verifique se os dados estão validados e limpos durante essa movimentação.

2. **Renomear para descontinuação**: renomeie o campo local com um prefixo como `[DEPRECATED]` ou `z_` (por exemplo, `z_Language (Old)`). Isso empurra o campo para a parte inferior dos seletores de campo e sinaliza aos usuários que ele não é mais a &quot;Source da verdade&quot;.

3. **Remoção de Formulário**: **Esta é a etapa mais crítica.** Remova o campo obsoleto de todos os **Registrar Forms**. Isso evita que novos dados sejam inseridos, mantendo os dados antigos visíveis nas exibições de tabela ou relatórios existentes, se necessário.

4. **Período de &quot;Desativação&quot;**: mantenha o campo obsoleto (prefixado e fora de forma) por 30 a 60 dias para garantir que nenhum dado tenha sido perdido durante a migração. Após esse período, se os dados forem totalmente reconciliados no Caminho global, o campo local poderá ser excluído do espaço de trabalho.



## &#x200B;6. Evitar a &quot;deriva do núcleo&quot; (a regra de abstração)

Para evitar que o Planning se torne tão desorganizado quanto o Principal:

* **A Camada de Abstração**: cada campo no WFP deve responder a uma **Pergunta Estratégica**. Se um campo for usado apenas para rastreamento tático (por exemplo, &quot;Esta prova foi aprovada?&quot;), mantenha-o no Core.

* **Consolidação primeiro**: se uma equipe quiser um novo campo de metadados, convide-a para verificar a Taxonomia global primeiro. Isso requer a concessão de **acesso Somente Leitura** aos clientes potenciais da equipe para o espaço de trabalho de Taxonomia Global (consulte a Seção 7). Ao mapear suas necessidades táticas para um campo estratégico existente, você evita duplicações desnecessárias e mantém a integridade dos relatórios.



## &#x200B;7. O modelo de visibilidade &quot;Acesso somente leitura&quot;

Resolva a sensação de &quot;Siloed&quot; sem o barulho do trabalho &quot;Siloed&quot;.

* **O problema**: as equipes em spokes se sentem isoladas porque só veem seus próprios registros.

* **A Correção**: conceder às equipes **acesso Somente Leitura aos espaços de trabalho designados como &#39;Primários&#39; para esses tipos de registros compartilhados**.

* **O Resultado**: eles podem ver o contexto corporativo mais amplo para inspiração e alinhamento, mas seu espaço de trabalho local permanece limpo e focado em suas tarefas específicas.



## &#x200B;8. Gerenciando o crescimento através de workshops

Dimensionar o PAM é tanto um desafio cultural quanto técnico. Use workshops direcionados para preencher a &quot;lacuna de governança&quot;.



### A. Workshop de descoberta da &quot;bagunça necessária&quot;

* **Público-alvo**: líderes regionais de marketing e especialistas em operações.

* **Meta**: documentar a &quot;Realidade Silonizada&quot; atual (os dados operacionais fragmentados).

* **A Mensagem**: &quot;Não estamos aqui para excluir seus campos. Estamos aqui para entender como eles se ligam à estratégia global.&quot;

* **Resultado**: um mapeamento de rascunho de campos táticos locais para rotas estratégicas globais.



### B. A Sessão De Alinhamento &quot;Visibilidade Estratégica&quot;

* **Público-alvo**: partes interessadas de marketing de alto nível (liderança).

* **Objetivo**: redefinir a ansiedade de &quot;Simplificar primeiro&quot;.

* **A Mensagem**: &quot;Não precisamos de uma taxonomia perfeita para iniciar. Estamos usando o WFP como o ambiente para *compilar* a taxonomia perfeita.&quot;

* **Resultado**: aprovação para avançar com o WFP como mecanismo de reconciliação enquanto o Core permanecer em seu estado atual.



### C. A Exibição &quot;Spoke-to-Global&quot;

* **Público-alvo**: novas equipes explorando o WFP.

* **Objetivo**: reduzir a sensação de &quot;siloed&quot;.

* **A Mensagem**: &quot;Veja como o trabalho local da Equipe A alimenta automaticamente a Workspace primária designada? Você pode ter a mesma visibilidade para seu trabalho também.&quot;

* **Resultado**: aceitação de novos departamentos que veem o benefício de serem &quot;conectados&quot; sem perder sua independência local.



### D. Horário comercial do &quot;Suporte contínuo&quot;

* **Público-alvo**: todos os usuários do WFP (atuais e potenciais).

* **Meta**: fornecer um ambiente recorrente e de baixo risco para orientação tática e solução de problemas.

* **A Mensagem**: &quot;Não há perguntas erradas. Estamos aqui para ajudá-lo a resolver seus desafios específicos de planejamento em tempo real.&quot;

* **Resultado**: maior confiança do usuário, resolução mais rápida de atritos técnicos e identificação de novos padrões que possam justificar padronização global.



## &#x200B;9. Equipe de Escala: Funções e Responsabilidades

O sucesso em um modelo de dimensionamento gerenciado requer mais do que apenas a configuração da ferramenta; requer uma distribuição clara das funções entre as equipes Global e Spoke.



### A. O Arquiteto Corporativo (CDE Central/Operações de Marketing)

* **Foco**: integridade da empresa, desempenho do sistema e **taxonomia de dados unificados**.

* **Responsabilidades**:

   * Gerencia a **Workspace de Taxonomia Global**.

   * Facilita o **Caminho de maturidade do campo** (promovendo sucessos locais para padrões globais).

   * Mantém as exibições **Principais do Workspace** para relatórios executivos.

   * Lidera a **Auditoria Semântica** mensal entre espaços de trabalho.



### B. O Spoke Champion (Proprietário do Processo de Equipe)

* **Foco**: relevância da equipe e velocidade de adoção.

* **Responsabilidades**:

   * Atua como ponto único de contato da equipe funcional.

   * É o proprietário da estrutura do espaço de trabalho local e dos experimentos de campo personalizado.

   * Garante que a equipe use o **Gateway Controlado** (Forms) para entrada de dados.

   * Participa do **Handshake Colaborativo** durante a harmonização.



### C. O Patrocinador Executivo (Liderança de Marketing)

* **Foco**: alinhamento estratégico, visibilidade de OKR e **visualização de portfólio (por exemplo, Calendário global)**.

* **Responsabilidades**:

   * Define os **OKRs de marketing** da empresa no espaço de trabalho de Taxonomia global.

   * Defende o valor de &quot;Etapa de visibilidade 1&quot; para outros líderes.

   * Reforça a alocação de recursos 80/20 (Valor sobre limpeza).



### D. O líder de ativação (gerenciamento de alterações)

* **Foco**: mudança cultural e desenvolvimento de habilidades.

* **Responsabilidades**:

   * Hospeda recorrentes **Office Hours** e **Workshops de Descobertas**.

   * Mantém a exibição interna de &quot;História de sucesso&quot;.

   * Identifica pontos de atrito técnico que o Arquiteto Empresarial deve resolver.



## &#x200B;10. Lista de verificação para dimensionar a próxima equipe

* [ ] **Identifique o Campeão**: quem é o &quot;Proprietário do Processo&quot; ou o &quot;Campeão&quot; desta nova equipe?

* [ ] **Definir o &quot;Delta Local&quot;**: de quais 2 a 3 campos essa equipe precisa que o padrão Global não fornece atualmente?

* [ ] **Mapear para rotas globais**: quais campos globais existentes podem atender a 80% de suas necessidades?

* [ ] **Conceder Visibilidade Global**: Conceder a eles acesso Somente Leitura aos Espaços de Trabalho Primários relevantes e ao espaço de trabalho de Taxonomia Global no Dia 1.

* [ ] **Estabelecer a Transferência**: como seu trabalho &quot;alimenta&quot; os Espaços de Trabalho Principais relevantes? (por exemplo, por meio de um Tipo de registro global ou uma pesquisa específica).