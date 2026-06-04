---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: Editar configurações de prova
description: É possível editar configurações de prova a qualquer momento após criar uma prova.
author: Courtney
feature: Digital Content and Documents
exl-id: ee30ce2c-e3dc-4863-a69b-cbc1b8747362
TQID: https://experienceleague.adobe.com/8ZOLF6hwAvWlLyMPtt1Ad8ZAfHCjKg-annlGGv5Qz3g
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 532
ht-degree: 15%

---

# Editar configurações de prova

É possível editar configurações de prova a qualquer momento após criar uma prova.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Padrão</p>
   <p>Trabalho ou Plano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de Permissões de Prova </td> 
   <td>Gerente ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Função de prova</td> 
   <td>Autor ou moderador</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a documentos</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Editar configurações de prova

Algumas configurações podem ser bloqueadas se o administrador do Workfront as desabilitar no nível da conta.

1. Vá para o projeto, tarefa ou problema em que deseja a prova e clique na guia **Documentos**.
1. Passe o mouse sobre a prova, em seguida clique em **Detalhes do documento**.
1. No painel esquerdo, clique em **Configurações do visualizador de provas**.
1. Ajuste as seguintes configurações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Exigir logon. Esta prova não pode ser compartilhada com usuários convidados</td> 
      <td> <p>Se você precisar de níveis mais altos de segurança para o processo de revisão e aprovação, poderá usar exigir logon na prova. Isso significa que somente os usuários do Workfront podem ser adicionados à prova. Eles devem inserir seu email e senha antes de acessá-los.</p> <p>Observação: <em style="font-style: normal;">Se o Logon necessário estiver habilitado, as Assinaturas não poderão ser habilitadas.</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Requer decisões assinadas eletronicamente</td> 
      <td> <p>Você pode exigir uma assinatura eletrônica de qualquer revisor que tome uma decisão sobre a prova. Quando um revisor toma uma decisão, é exibido um prompt solicitando que ele insira seu email e senha e confirme sua decisão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear prova quando todas as decisões necessárias forem tomadas</td> 
      <td> <p>Você pode definir um estado de prova para bloquear quando o Aprovador final tomar a decisão. Isso é útil se você quiser garantir que os revisores não possam voltar para a prova e adicionar comentários adicionais ou alterar suas decisões.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir o download do arquivo original</td> 
      <td> <p>É possível permitir que os revisores em uma prova baixem o arquivo original do qual uma prova foi criada. Isso é ativado por padrão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir o compartilhamento da prova por meio de URL público ou código de inserção</td> 
      <td>Você pode permitir que os usuários compartilhem a prova com um URL público ou código de inserção. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir assinatura da prova por meio de URL público ou código de inserção</td> 
      <td> <p>Ativar a assinatura na prova permite que as pessoas que não foram adicionadas explicitamente à prova assinem a prova (ou seja, se adicionem à prova). Eles receberão a função e o alerta por email que você selecionar para eles nas Configurações de assinatura.</p> <p>Se a Assinatura tiver sido habilitada em uma prova, os campos abaixo ficarão ativos:</p> 
       <ul> 
        <li><strong>Validação de assinante necessária</strong> - O assinante deve clicar em um link em um email para acessar uma prova<br>Selecionar essa opção significa que a pessoa que está assinando não terá acesso imediato à prova, mas receberá um link para a prova em um email. O objetivo da validação do assinante é garantir que a pessoa tenha inserido um endereço de email correto ao qual tem acesso.</li> 
        <li><strong>Função padrão para novos assinantes -</strong> Esta é a função de prova padrão que será atribuída a todos os revisores que se subscreverem à prova.</li> 
        <li><strong>Alerta de email padrão para novos assinantes</strong> - É o alerta de email padrão que será atribuído a todos os revisores que assinarem a prova.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.

 
