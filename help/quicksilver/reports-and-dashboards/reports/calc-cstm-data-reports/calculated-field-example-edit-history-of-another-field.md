---
content-type: reference
product-area: reporting
keywords: auditoria,trilha,personalizado,campo
navigation-topic: calculate-custom-data-reports
title: "Exemplo de campo personalizado calculado: exibir um histórico de edição do campo"
description: Se os usuários atualizarem campos personalizados regularmente e você quiser capturar um log de todas as alterações feitas em um campo, bem como uma data quando as alterações ocorrerem, será possível capturar essas informações em um campo personalizado calculado.
author: Nolan
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 0%

---

# Exemplo de campo personalizado calculado: exibir um histórico de edição do campo

Se os usuários atualizarem campos personalizados regularmente e você quiser capturar um log de todas as alterações feitas em um campo, bem como uma data quando as alterações ocorrerem, será possível capturar essas informações em um campo personalizado calculado.

O exemplo a seguir mostra como criar o campo calculado *Histórico de Edição de Instruções* para capturar todas as alterações feitas em um campo de texto de linha única chamado *Instruções*.

>[!TIP]
>
>Você pode seguir esse exemplo para todos os tipos de campos personalizados, não apenas campos de texto de linha única.

Isso faz o seguinte: 

* Limita o campo *Histórico de Edição de Instruções* aos 2000 caracteres mais recentes para permanecer dentro do limite do banco de dados do Workfront.
* Verifica se o valor atual do campo *Instruções* corresponde à parte frontal do valor de *Histórico de Edição de Instruções*; presume que está em branco e, se não estiver, faz o seguinte: 

   * Se houver correspondência, o *Histórico de Edição de Instruções* permanecerá inalterado;
   * Se não corresponderem, substituirá o *Histórico de Edição de Instruções* pelo último valor no campo *Instruções*, seguido da data atual entre parênteses, uma barra vertical e o *Histórico de Edição de Instruções* anterior, que preserva o(s) valor(es) anterior(es) e a(s) data(s) quando foram inseridos.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>plano do Adobe Workfront*</p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td> <p>Licença da Workfront*</p> </td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Configurações de nível de acesso*</strong> </td> 
   <td> <p>Acesso administrativo ao Forms personalizado</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Permissões de objeto</strong> </p> </td> 
   <td> <p>Gerenciar permissões nos formulários personalizados </p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Compartilhar um formulário personalizado</a>.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## Pré-requisitos

Para adicionar um campo calculado que exibe o histórico de edição de um campo a um formulário personalizado, primeiro é necessário:

* Criar o formulário personalizado
* Adicione o campo cujo histórico você deseja capturar ao formulário personalizado

## Exibir um histórico de edição do campo

1. Vá para um formulário personalizado em que deseja adicionar o campo calculado.

1. Para criar o campo personalizado de texto de linha única, por exemplo, faça o seguinte:

   1. Clique em **Campo de Texto de Linha Única**.
   1. Especifique um **rótulo** para o campo personalizado, como *instruções*.
   1. Clique em **Aplicar**.

1. Selecione **Adicionar um campo** e **Calculado** para adicionar um campo personalizado calculado ao formulário.
1. Especifique um **Rótulo** para o campo personalizado calculado, como *Histórico de Edição de Instruções*.

   Este campo capturará todas as alterações feitas no primeiro campo criado por você (*Instruções*).

1. Clique em **Salvar + Fechar**.
1. Clique no nome do formulário ao qual você adicionou dois campos para reabri-lo.
1. Clique no campo personalizado calculado *Instruções Editar histórico* e, em seguida, copie e cole o seguinte na caixa Cálculo:
1. No campo **Cálculo**, especifique o seguinte cálculo para seu campo personalizado:

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (Recomendado) Cole o mesmo cálculo no campo **Instruções** no campo calculado do formulário.
1. Verifique se  **O texto** está selecionado no campo **Formatar** para formatar o campo personalizado calculado como texto.

   Este é o padrão.

1. Clique em **Salvar+Fechar**.

   Agora, quando você anexa o formulário personalizado a um objeto e alguém altera as informações no campo *Instruções*, o campo *Instruções Editar histórico&quot; exibe o valor mais recente, seguido da data atual entre parênteses e uma barra vertical. Se forem feitas mais alterações, elas serão adicionadas a essas informações da mesma forma.

   No cálculo acima, você pode substituir *Instruções* pelo nome exato do campo de texto de linha única cujo histórico deseja rastrear e *Instruções Editar Histórico* pelo nome exato do campo calculado.
