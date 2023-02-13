---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: Editar configurações de prova
description: Você pode editar as configurações de prova a qualquer momento depois de criar uma prova.
author: Courtney
feature: Digital Content and Documents
exl-id: ee30ce2c-e3dc-4863-a69b-cbc1b8747362
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 7%

---

# Editar configurações de prova

Você pode editar as configurações de prova a qualquer momento depois de criar uma prova.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Plano atual: Pro ou superior</p> <p>ou</p> <p>Plano herdado: Premium</p> <p>Para obter mais informações sobre como revisar o acesso com os diferentes planos, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de prova no Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano atual: Trabalho ou Plano</p> <p>Plano herdado: Qualquer (É necessário ter a prova ativada para o usuário)</p> </td> 
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
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, função ou Perfil de permissão de prova você possui, entre em contato com o administrador da Workfront ou da Workfront Proof.

## Editar configurações de prova

Algumas configurações podem ser bloqueadas se o administrador do Workfront as tiver desativado no nível da conta.

1. Vá para o projeto, tarefa ou problema onde deseja obter a prova e clique no botão **Documentos** guia .
1. Passe o mouse sobre a prova e clique em **Detalhes do documento**.
1. No painel esquerdo, clique em **Configurações do visualizador de prova**.
1. Ajuste as seguintes configurações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Exigir login. Esta prova não pode ser compartilhada com usuários convidados</td> 
      <td> <p>Se você precisar de níveis mais altos de segurança para o seu processo de revisão e aprovação, poderá usar o logon obrigatório na prova. Isso significa que somente usuários do Workfront podem ser adicionados à prova. Eles devem digitar o email e a senha para poder acessá-los.</p> <p>Observação: <em style="font-style: normal;">Se o Logon necessário estiver ativado, as Assinaturas não poderão ser ativadas.</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Requer decisões assinadas eletronicamente</td> 
      <td> <p>Você pode exigir uma assinatura eletrônica de qualquer revisor que tome uma decisão sobre a prova. Quando um revisor toma uma decisão, um prompt é exibido, solicitando que ele insira seu email e senha e confirme sua decisão. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information, see 
          <a href="../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md" class="MCXref xref">Understanding electronic signatures in Workfront Proof</a>
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear a prova quando todas as decisões necessárias forem tomadas</td> 
      <td> <p>Você pode definir um estado de prova para bloquear quando o Aprovador final tomar sua decisão. Isso é útil se você quiser garantir que seus revisores não poderão voltar à prova e adicionar comentários adicionais ou alterar suas decisões.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir o download do arquivo original</td> 
      <td> <p>Você pode permitir que revisores em uma prova baixem o arquivo original do qual uma prova foi criada. Isso é ativado por padrão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir o compartilhamento da prova por meio de URL público ou código de inserção</td> 
      <td>Você pode permitir que os usuários compartilhem a prova com um URL público ou código incorporado. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir assinatura da prova por meio de URL público ou código de inserção</td> 
      <td> <p>Habilitar a assinatura na prova permite que as pessoas que não foram adicionadas explicitamente à prova se inscrevam na prova (ou seja, se adicionem à prova). Eles receberão a função e o alerta por email selecionados para eles nas configurações de Assinatura.</p> <p>Se a opção Subscription tiver sido ativada em uma prova, os campos abaixo se tornarão ativos:</p> 
       <ul> 
        <li><strong>Validação necessária do assinante</strong> - O assinante deve clicar em um link em um email para acessar uma prova<br>Selecionar essa opção significa que a pessoa que está assinando não terá acesso imediato à prova, mas obterá um link para a prova em um email. O objetivo da validação do assinante é garantir que a pessoa tenha inserido um endereço de email correto ao qual tenha acesso.</li> 
        <li><strong>Função padrão para novos assinantes -</strong> Essa é a função de prova padrão que será atribuída a todos os revisores que assinam a prova.</li> 
        <li><strong>Alerta por email padrão para novos assinantes</strong> - Esse é o alerta por email padrão que será atribuído a todos os revisores que assinam a prova.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.

 
