---
content-type: reference
product-area: reporting
keywords: auditoria,trilha,personalizado,campo
navigation-topic: calculate-custom-data-reports
title: "Exemplo de campo personalizado calculado: exibir o histórico de edição de um campo"
description: Se os usuários atualizarem campos personalizados regularmente e você quiser capturar um log de todas as alterações feitas em um campo, bem como uma data em que as alterações ocorram, você poderá capturar essas informações em um campo personalizado calculado.
author: Nolan
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 0%

---

# Exemplo de campo personalizado calculado: exibir o histórico de edição de um campo

Se os usuários atualizarem campos personalizados regularmente e você quiser capturar um log de todas as alterações feitas em um campo, bem como uma data em que as alterações ocorram, você poderá capturar essas informações em um campo personalizado calculado.

O exemplo a seguir mostra como criar o *Instruções Editar Histórico* campo calculado para capturar todas as alterações feitas em um campo de texto de linha única chamado *Instruções*.

>[!TIP]
>
>Você pode seguir este exemplo para todos os tipos de campos personalizados, não apenas para campos de texto de uma única linha.

Isso faz o seguinte: 

* Limita o *Instruções Editar Histórico* para os 2000 caracteres mais recentes para permanecer dentro do limite do banco de dados do Workfront.
* Verifica se o valor atual da variável *Instruções* corresponde à frente do campo *Instruções Editar Histórico* valor; parte do princípio que está em branco e, caso contrário, faz o seguinte: 

   * Se eles combinarem, deixará a variável *Instruções Editar Histórico* tal como se encontra;
   * Se não corresponderem, substituirá a variável *Instruções Editar Histórico* com o valor mais recente na *Instruções* , seguido pela data atual entre parênteses, uma barra vertical e a anterior *Instruções Editar Histórico*, que preserva os valores anteriores e a(s) data(s) de entrada.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Plano Adobe Workfront*</p> </td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td> <p>Licença da Workfront*</p> </td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Configurações de nível de acesso*</strong> </td> 
   <td> <p>Acesso administrativo ao Forms personalizado</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Permissões de objeto</strong> </p> </td> 
   <td> <p>Gerenciar permissões nos formulários personalizados </p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Compartilhar um formulário personalizado</a>.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## Pré-requisitos

Para adicionar um campo calculado que exibe o histórico de edição de um campo a um formulário personalizado, primeiro você deve:

* Criar o formulário personalizado
* Adicione o campo cujo histórico você deseja capturar no formulário personalizado

## Exibir o histórico de edição de um campo

1. Vá para um formulário personalizado onde deseja adicionar o campo calculado.

1. Para criar o campo personalizado de texto de linha única, por exemplo, faça o seguinte:

   1. Clique em **Campo de texto de linha única**.
   1. Especifique um **Rótulo** para o campo personalizado, como *Instruções*.
   1. Clique em **Appliance**.

1. Selecionar **Adicionar um campo**, em seguida selecione **Calculado** para adicionar um campo personalizado calculado ao formulário.
1. Especifique um **Rótulo** para o campo personalizado calculado, como *Instruções Editar Histórico*.

   Este é o campo que capturará todas as alterações feitas no primeiro campo criado (*Instruções*).

1. Clique em **Salvar + Fechar**.
1. Clique no nome do formulário, onde agora você adicionou dois campos para reabri-lo.
1. Clique no campo personalizado calculado *Instruções Editar Histórico,* em seguida, copie e cole o seguinte na caixa Cálculo :
1. No **Cálculo** , especifique o seguinte cálculo para o seu campo personalizado:

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (Recomendado) Cole o mesmo cálculo no **Instruções** no campo calculado do formulário.
1. Certifique-se de que  **Texto** é selecionado no **Formato** para formatar o campo personalizado calculado como texto.

   Este é o padrão.

1. Clique em **Salvar+Fechar**.

   Agora, ao anexar o formulário personalizado a um objeto e, em seguida, alguém altera as informações no *Instruções* , o campo *Instruções Editar Histórico&quot; exibe o valor mais recente, seguido da data atual entre parênteses e uma barra vertical. Se forem feitas outras alterações, elas serão adicionadas a essas informações da mesma forma.

   No cálculo acima, você pode substituir *Instruções* com o nome exato do campo de texto de linha única cujo histórico você deseja rastrear, e *Instruções Editar Histórico* com o nome exato do campo calculado.
