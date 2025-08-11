---
title: Preencher automaticamente uma solicitação a partir de dados anteriores
content-type: reference
description: Você pode usar a IA para preencher automaticamente campos de solicitação usando dados de solicitações anteriores.
author: Becky
feature: Get Started with Workfront
source-git-commit: cf2ae77ed27b1dd30144f6de31bec474f53f1efb
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---

# Preencher automaticamente uma solicitação a partir de dados anteriores

>[!NOTE]
>
>* Essa funcionalidade estará disponível como um beta aberto no seguinte agendamento:
>
>   * Lançamento mensal: 11 de setembro de 2025
>   * Versão trimestral: 16 de outubro de 2025

A IA pode ajudar a preencher automaticamente os campos de solicitação com base em solicitações anteriores. Você pode aprovar ou rejeitar essas sugestões antes de enviar a solicitação.

O preenchimento automático não substitui nenhum campo já preenchido.

Os usuários não recebem sugestões de dados aos quais, de outra forma, não teriam acesso.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Novo: Colaborador ou superior</p>
   Ou
   <p>Atual: solicitação ou superior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a ocorrências</p>  </td> 
  </tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td><p>Acesso para adicionar solicitações a uma fila de solicitações</p> <p>Exibir permissões ou mais altas na solicitação existente</p> <p>Para obter informações sobre como configurar uma fila de solicitações, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Criar uma fila de solicitações</a>. </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Obter sugestões ao preencher o formulário

O preenchimento automático pode sugerir valores de campo enquanto você preenche o formulário. À medida que você informa valores nos campos de solicitação, o Workfront compara esses valores com solicitações anteriores. Se o valor inserido estiver estreitamente correlacionado com outros valores de campo em contextos semelhantes em solicitações anteriores, o Workfront sugere esses valores.

Por exemplo, se uma clínica sempre usar o mesmo código de faturamento, a Workfront sugerirá esse código de faturamento no campo apropriado quando o nome da clínica for inserido.

Para usar sugestões com base em solicitações anteriores:

1. Comece a criar uma solicitação.

   Para obter instruções, consulte [Criar e enviar solicitações](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Comece a preencher os campos.

   À medida que você preenche campos, outros campos podem mostrar sugestões.

1. Para cada sugestão de campo, selecione **Aceitar** ou **Rejeitar** para esse campo.

   ![Aceitar ou rejeitar sugestão](assets/accept-reject-suggestion.png)

   Ou

   Selecione **Aceitar tudo** ou **Rejeitar tudo** na parte superior da página para aceitar ou rejeitar todas as sugestões.

   >[!NOTE]
   >
   >Quaisquer sugestões não revisadas serão automaticamente aceitas quando você enviar a solicitação.
