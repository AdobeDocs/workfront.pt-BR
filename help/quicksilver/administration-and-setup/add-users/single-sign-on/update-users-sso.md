---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
title: Atualizar usuários para logon único
description: Você pode atualizar usuários para logon único no Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0f9c543a-2ae2-4c2c-9c4d-647079263a7e
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 1%

---

# Atualizar usuários para logon único

{{important-admin-console-onboard}}

Quando o logon único (SSO) é ativado na sua instância do Adobe Workfront, você pode fazer logon no Workfront com suas credenciais de SSO.

Se você tiver um sistema existente que já esteja preenchido com usuários associados a credenciais de SSO, poderá importar as IDs dos usuários para o Workfront importando um arquivo CSV (valores separados por vírgula) para o Workfront.

Para obter mais informações sobre a integração do Workfront com um sistema SSO, consulte [Visão geral do logon único no Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).


## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Nomes de usuário SSO

Dependendo da solução de SSO usada, o nome de usuário no ambiente de SSO pode ser chamado de qualquer um dos seguintes:

* Usuário do SSO
* Federation ID
* Nome de Usuário da Federação

No Workfront, todos esses nomes são armazenados no campo Nome de usuário SSO , no objeto do usuário.

Para que seus usuários possam usar suas credenciais de SSO para fazer logon no Workfront, é necessário atualizar seu perfil para incluir seu nome de usuário de SSO, além do nome de usuário do Workfront.

Como administrador do Workfront, você pode atualizar o campo Nome de usuário SSO em massa para seus usuários do Workfront usando uma lista de nomes de usuário e importando-o no Workfront. Essa lista deve conter a ID de usuário do Workfront (GUID), bem como o nome de usuário SSO correspondente para cada usuário e deve ser salva como um arquivo CSV ou TSV. Esse processo atualiza nomes de usuário SSO existentes no Workfront ou adiciona um novo nome de usuário SSO, se estiver faltando um para os usuários.

## Preparar o arquivo de importação {#prepare-the-import-file}

Você pode começar a preparar seu arquivo de importação criando um relatório de todos os usuários no Workfront que devem ter seus campos de nome de usuário SSO atualizados.

1. Criar um relatório de usuário no Workfront.

   Para obter instruções sobre como criar relatórios do usuário no Workfront, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Selecione os seguintes campos em seu relatório:

   | Nome | O nome completo do usuário do Workfront. |
   |---|---|
   | ID | A ID é o GUID alfanumérico da Workfront. |
   | Usuário do SSO | Selecione o campo Nome de Usuário do SSO para garantir que não haja nomes de usuário que você esteja substituindo por sua importação. Esse campo deve estar em branco para todos os usuários, se eles ainda não tiverem sido atualizados para SSO. |

   ![](assets/users-with-sso-username-and-no-sso-access-only-field.png)

1. Salve o relatório.
1. Clique em **Exportar** na parte superior do relatório e exporte o relatório para o Excel.
1. Abra o arquivo Excel exportado e comece a adicionar seus nomes de usuário SSO para cada usuário no relatório na coluna Nome de usuário SSO .

   >[!IMPORTANT]
   >
   >Os nomes de usuário SSO fazem distinção entre maiúsculas e minúsculas.

1. Elimine todas as colunas no arquivo Excel, exceto o **ID** e **Nome de Usuário SSO** colunas.

1. Elimine os cabeçalhos de coluna e verifique se não há linhas em branco na parte superior do relatório.

   O arquivo que você está usando para atualizar seus usuários do Workfront com os nomes de usuário SSO deve conter apenas 2 colunas, nesta ordem:

   * A primeira coluna deve exibir a ID de usuário do Workfront (o GUID do usuário, como encontrado no Workfront).
   * A segunda coluna deve conter o nome de usuário SSO, como é exibido no sistema SSO.
   * As colunas não devem ter cabeçalhos e não deve haver linhas vazias na parte superior da lista de nomes.

      ![](assets/update-users-for-sso-csv-file-for-import.png)

1. Salve o relatório como um arquivo CSV ou TSV em seu computador.

## Atualize seus usuários para SSO {#update-your-users-for-sso}

O processo de atualização de usuários para SSO adiciona o campo Nome de usuário SSO aos usuários do Workfront se um não estiver presente ou atualiza o valor nesse campo se já houver um valor associado aos usuários.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema** then **Atualizar usuários para SSO**.

1. Clique em **Escolher arquivo** para procurar o arquivo que você preparou.

   Para obter mais informações sobre como preparar este arquivo, consulte [Preparar o arquivo de importação](#prepare-the-import-file).

1. Selecione o arquivo onde ele está salvo em seu computador e clique em **Abrir**.

   Isso permite que todos os usuários façam logon no Workfront usando suas credenciais de SSO.

   O **Permitir apenas `<SSO Configuration>` Autenticação** está ativada para todos os usuários incluídos no CSV.

## Verifique o SSO dos nomes de usuário do Workfront de seus usuários

Para obter instruções sobre como criar um relatório de usuário contendo informações do nome de usuário SSO, consulte [Preparar o arquivo de importação](#prepare-the-import-file).

1. Execute um relatório de usuário contendo informações do nome de usuário SSO.

   Observe que a coluna Nome de Usuário SSO é preenchida para cada usuário.

1. Certifique-se de que os valores da coluna Nome de Usuário SSO correspondam ao Nome de Usuário SSO no seu servidor SSO.
1. Se a coluna Nome de Usuário SSO estiver em branco, atualize os nomes de Usuário SSO de seus usuários.

   ![](assets/users-with-sso-field-updated.png)

   Para obter instruções sobre como atualizar seus usuários para SSO, consulte [Atualize seus usuários para SSO](#update-your-users-for-sso).
