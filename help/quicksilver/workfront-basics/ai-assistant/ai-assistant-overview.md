---
title: Assistente de IA no Workfront
content-type: reference
description: Saiba mais sobre o Assistente de IA no Adobe Workfront
author: Becky
feature: Get Started with Workfront
exl-id: e5f2408b-2c29-4257-8bdc-bf20880de265
source-git-commit: e8e10f02f77f6c1df9f0af380eb16cc6bbc3b5d1
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 100%

---

# Assistente de IA no Workfront

O Assistente de IA do Workfront ajuda você a realizar seu trabalho, oferecendo informações e sugestões no aplicativo em uma conversa em linguagem natural. O Assistente de IA pode proporcionar uma experiência de trabalho mais tranquila ao

* Resumir itens de trabalho ou documentos
* Encontrar instruções ou material de referência para processos de trabalho
* Gerar ou verificar fórmulas para campos calculados

## Requisitos de acesso

Você deve ter o seguinte acesso para realizar as etapas descritas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td><p>Novo: qualquer um</p>
       <p>ou</p>
       <p>Atual: não disponível</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: padrão</p>
       <p>ou</p>
       <p>Atual: não disponível</p></td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Pré-requisitos para o Assistente de IA

Para habilitar o Assistente de IA para sua organização, **todos** os seguintes requisitos devem ser atendidos:

* Sua organização deve ter migrado para o Adobe IMS (Sistema de Gerenciamento de Identidades)
* A Adobe Unified Experience deve estar habilitada
* Sua organização deve ter um plano Select, Prime ou Ultimate do Workfront
* A Adobe deve ter um contrato de IA generativa da Adobe assinado em arquivo

  Para obter mais informações sobre a assinatura do contrato, consulte [Assinar o contrato de IA generativa da Adobe](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) neste artigo.

## Considerações sobre o Assistente de IA

* O Assistente de IA é sensível ao contexto da página que você tem aberta. Por exemplo, ao inserir “Resumir este projeto” no Assistente de IA em uma página de projeto, um resumo desse projeto específico será exibido.
* O administrador do Workfront deve habilitar o Assistente de IA para os usuários da sua organização. O Assistente de IA é habilitado por meio de níveis de acesso.

  Para obter mais informações, consulte [Habilitar ou desabilitar o Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* O Assistente de IA do Workfront Planning tem funcionalidades diferentes do Assistente de IA do Workfront.

  Para obter mais informações sobre o Assistente de IA no Workfront Planning, consulte [Visão geral do Assistente de IA do Adobe Workfront Planning](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

* O Assistente de IA está disponível apenas em inglês no momento.


## Funcionalidade disponível no Assistente de IA

O Assistente de IA oferece atualmente as seguintes funcionalidades:

* Resumo de projetos, tarefas, problemas ou documentos.

  Para obter mais informações, consulte [Resumir usando o Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

* Fornecimento de instruções ou informações de referência extraídas da documentação do Workfront na Adobe Experience League.

  Para obter mais informações, consulte [Obter ajuda do Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md).

* Localizar itens específicos no Workfront.

  Para obter mais informações, consulte [Usar o Assistente de IA para trabalhar com projetos, tarefas e problemas](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).

* Gerar ou refinar fórmulas para campos personalizados calculados.

  >[!NOTE]
  >
  >Essa funcionalidade está disponível apenas para organizações nos planos Prime ou Ultimate do Workfront.

  Para obter mais informações, consulte [Gerar ou revisar fórmulas de campos calculados com o Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md).

* Resumir atualizações, documentos enviados e outras alterações importantes sobre seus projetos nos seguintes intervalos de tempo: 24 horas, 3 dias, 7 dias em Prioridades.

Para obter mais informações, consulte [Atualize-se sobre o trabalho em Prioridades](/help/quicksilver/workfront-basics/priorities/catch-me-up.md).


## Tipos de objetos disponíveis para o Assistente de IA

O Assistente de IA pode consultar dados associados aos seguintes tipos de objetos, caso o usuário tenha as permissões válidas no Workfront:

* Portfólios
* Programas
* Projetos
* Tarefas
* Problemas
* Formulários personalizados
* Usuários
* Registros do Workfront Planning


## Acessar o Assistente de IA

1. Na parte superior de qualquer página do Workfront, clique no ícone do Assistente de IA ![Ícone do Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Digite sua pergunta ou prompt no painel à direita da tela.

   Se você não conseguir digitar neste painel, sua organização não tem um contrato de IA generativa da Adobe assinado em arquivo.

1. Se o Assistente de IA não fornecer a resposta que você precisa, refine seu prompt e tente novamente.

## Assinar o contrato de IA generativa da Adobe

Se a sua organização não tiver um contrato de IA generativa da Adobe assinado em arquivo, o Assistente de IA não poderá ser habilitado para a sua organização.

Se um usuário tentar usar o Assistente de IA quando o contrato de IA generativa da Adobe não tiver sido assinado, ele verá uma mensagem:

* Usuários: os usuários são informados de que o Assistente de IA não foi habilitado para a organização e que podem entrar em contato com o administrador do Workfront para solicitá-lo para a organização.
* Administradores: os administradores são informados de que não há um contrato de IA generativa da Adobe assinado e podem solicitar o envio de uma cópia do contrato para assinatura.

Para solicitar o contrato de IA generativa da Adobe:

1. Como administrador do Workfront, clique no ícone do Assistente de IA ![Ícone do Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Comece a digitar no painel do Assistente de IA.
1. Quando a mensagem do contrato de IA generativa da Adobe for exibida, clique em **Revisar contrato**.
1. Insira o nome e o endereço de e-mail da pessoa da sua organização que assinará o contrato de IA generativa da Adobe.

   O contrato será enviado a essa pessoa para assinatura. Após ser assinado e devolvido, o contrato é revisado pela Adobe e, em seguida, o Assistente de IA é habilitado para a sua organização.

   >[!NOTE]
   >
   >Aguarde de 1 a 3 dias úteis após a assinatura e a devolução do contrato para que a Adobe revise e habilite o Assistente de IA.

## Dicas para criar prompts no Assistente de IA

Use as seguintes palavras-chave nos seus prompts para fornecer contexto e ajudar a localizar as informações corretas. As palavras-chave não diferenciam maiúsculas de minúsculas.

Ao inserir seu prompt, inclua a frase `using (keyword)`.

| Palavra-chave | Efeito |
| --- | --- | 
| `workfront` | Interagir com o Workfront. |
| `planning` | Interagir com o Workfront Planning. |
| `help` | Retorna informações da documentação do Experience League. |
| `formula` | Verifica e retorna fórmulas para uso no Planning, na Configuração ou em formulários personalizados. |
| `health` | Verifica a integridade do projeto com o Project Health Advisor. |
| `summarize` | Resume itens, como ao fazer upload de um arquivo ou resumir um projeto. |

>[!NOTE]
>
> Nem todas as palavras-chave estão disponíveis em todas as áreas.
>
>* A palavra-chave `formula` está disponível apenas no Planning, na Configuração e no construtor de formulários personalizados.
>* A palavra-chave `planning` está disponível apenas no Workfront Planning.





