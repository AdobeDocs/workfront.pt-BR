---
title: Visão geral do Assistente de IA
content-type: reference
description: Visão geral do Assistente de IA
author: Becky
feature: Get Started with Workfront
exl-id: e5f2408b-2c29-4257-8bdc-bf20880de265
source-git-commit: a4e403abadc0268b919ce8105989ef6c912f33a4
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 1%

---

# Visão geral do Assistente de IA

O Assistente de IA da Workfront ajuda você a realizar seu trabalho oferecendo informações e sugestões no aplicativo em uma conversa em idioma natural. O Assistente de IA pode lhe oferecer uma experiência de trabalho mais estável

* Resumindo itens de trabalho ou documentos
* Encontrar instruções ou material de referência para processos de trabalho
* Gerar ou verificar fórmulas para campos calculados

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td><p>Novo: Qualquer um</p>
       <p>ou</p>
       <p>Atual: não disponível</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p>
       <p>ou</p>
       <p>Atual: não disponível</p></td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Pré-requisitos para o Assistente de IA

Para habilitar o Assistente de IA para sua organização, **todos** dos itens a seguir devem ser aplicados:

* Sua organização deve ter migrado para o Adobe IMS (Identity Management System)
* A Experiência unificada do Adobe deve ser habilitada
* Sua organização deve ter um plano Select, Prime ou Ultimate Workfront
* A Adobe deve ter um contrato de geração de IA da Adobe assinado no arquivo

  Para obter mais informações sobre como assinar o contrato, consulte [Assinar o contrato de IA de Geração da Adobe](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) neste artigo.

## Considerações sobre o Assistente de IA

* O Assistente de IA é sensível ao contexto da página que você abriu. Por exemplo, inserir &quot;Resumir este projeto&quot; no Assistente de IA em uma página de projeto retorna um resumo desse projeto específico.
* O administrador do Workfront deve ativar o Assistente de IA para os usuários em sua organização. O Assistente de IA é ativado por meio de níveis de acesso.

  Para obter mais informações, consulte [Habilitar ou desabilitar o Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* O Assistente do Workfront Planning AI tem recursos diferentes do Assistente do Workfront AI.

  Para obter mais informações sobre o Assistente de IA no Workfront Planning, consulte [Visão geral do Assistente de IA do Adobe Workfront Planning](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

* No momento, o Assistente de IA está disponível somente em inglês.


## Funcionalidade disponível no Assistente de IA

Atualmente, o Assistente de IA oferece as seguintes funcionalidades:

* Resumo de projetos, tarefas, problemas ou documentos.

  Para obter mais informações, consulte [Resumir usando o Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

* Fornecer instruções ou informações de referência extraídas da documentação do Workfront na Adobe Experience League.

  Para obter mais informações, consulte [Obter ajuda do Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md).

* Localizar itens específicos no Workfront.

  Para obter mais informações, consulte [Usar o Assistente de IA para trabalhar com projetos, tarefas e problemas](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).

* Gerar ou refinar fórmulas para campos personalizados calculados.

  >[!NOTE]
  >
  >Essa funcionalidade está disponível somente para organizações nos planos do Prime ou do Ultimate Workfront.

  Para obter mais informações, consulte [Gerar ou revisar fórmulas de campo calculado com o Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md).

* Resumindo atualizações, documentos carregados e outras alterações importantes sobre seus projetos nos seguintes intervalos de tempo: 24 horas, 3 dias e 7 dias em Prioridades.

Para obter mais informações, consulte [Acompanhar o trabalho em Prioridades](/help/quicksilver/workfront-basics/priorities/catch-me-up.md).


## Tipos de objeto disponíveis para o Assistente de IA

O assistente de IA pode consultar dados associados aos seguintes tipos de objeto se o usuário tiver as permissões válidas no Workfront:

* Portfólios
* Programas
* Projetos
* Tarefas
* Problemas
* Formulários personalizados
* Usuários
* Registros do Workfront Planning


## Acessar o assistente do AI

1. Na parte superior de qualquer página do Workfront, clique no ícone do Assistente de IA ![ícone do Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Digite sua pergunta ou aviso no painel à direita da tela.

   Adobe Se não for possível digitar nesse painel, a organização não terá um contrato Gen AI assinado no arquivo.

1. Se o assistente de IA não fornecer a resposta necessária, refine seu prompt e tente novamente.

## Assinar o contrato de IA de geração da Adobe

Adobe Se a sua organização não tiver um contrato Gen AI assinado no arquivo, o Assistente AI não poderá ser ativado para a sua organização.

Se um usuário tentar usar o AI Assistant quando o contrato da Adobe Gen AI não tiver sido assinado, verá uma mensagem:

* Usuários: os usuários são informados de que o Assistente de IA não foi ativado para sua organização e que eles podem entrar em contato com o administrador do Workfront para solicitá-lo para sua organização.
* Administradores: os administradores são informados de que não há um contrato Adobe Gen AI assinado e podem solicitar que uma cópia do contrato seja enviada para assinatura.

Para solicitar o contrato da Adobe Gen AI:

1. Como um Administrador do Workfront, clique no ícone do Assistente do AI ![ícone do Assistente do AI](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Comece a digitar no painel Assistente de IA.
1. Quando a mensagem do contrato da Adobe Gen AI for exibida, clique em **Revisar contrato**.
1. Insira o nome e o endereço de email da pessoa da sua organização que assinará o contrato de IA de geração da Adobe.

   O contrato será enviado a este indivíduo para assinatura. Depois de assinado e devolvido, o contrato é revisado pela Adobe e o Assistente de IA é ativado para a sua organização.

## Dicas para criar prompts no Assistente de IA

Use as seguintes palavras-chave em seus prompts para fornecer contexto e ajudar a localizar as informações corretas. As palavras-chave não diferenciam maiúsculas de minúsculas.

Ao inserir seu prompt, inclua a frase `using (keyword)`.

| Palavra-chave | Efeito |
|---|---|
| `workfront` | Interage com o Workfront. |
| `planning ` | Interage com o Workfront Planning. |
| `help` | Retorna informações da documentação do Experience League. |
| `formula` | Verifica e retorna fórmulas para uso em formulários do Planning, de Configuração ou personalizados. |
| `health` | Verifica a integridade do projeto com o Supervisor de Integridade do Projeto. |
| `summarize` | Resume itens, como ao carregar um arquivo ou resumir um projeto. |

>[!NOTE]
>
> Nem todas as palavras-chave estão disponíveis em todas as áreas.
>
>* A palavra-chave `formula` está disponível apenas no Planning, na Instalação e no Construtor de formulários Personalizados.
>* A palavra-chave `planning` está disponível somente no Workfront Planning.





