---
title: Configurar Regras de Negócios do Tipo de Registro
description: Você pode configurar regras de negócios do tipo registro que possam impor determinadas ações nos registros de acordo com os valores do campo.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: cafe52c228520becb66e2fa9d8121127223a8f71
workflow-type: tm+mt
source-wordcount: '1094'
ht-degree: 2%

---


# Configurar regras de negócios do tipo de registro

{{planning-important-intro}}

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Após o lançamento para Pré-visualização, os mesmos recursos também estarão disponíveis mensalmente no ambiente de Produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Você pode configurar regras de negócios para tipos de registro do Adobe Workfront Planning para indicar que determinados campos são obrigatórios antes que uma ação em um registro desse tipo seja permitida ou impedida.

Dependendo de como a regra é formulada, você poderá permitir as seguintes ações nos registros se as regras de negócios definidas forem atendidas:

* Editar ou não editar um registro
* Excluir ou não excluir um registro

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso para executar as etapas deste artigo:  

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Qualquer Workfront ou Fluxo de trabalho com um pacote do Planning</p></li>
Ou
<li><p>Qualquer pacote do Planning quando adquirido como um produto independente</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Workflow Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>licença do Adobe Planning</p></td> 
   <td><p>Planejamento padrão</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Você deve adicionar um Workflow e um tipo de licença do Planning ao nível de acesso quando tiver um Workflow e um pacote do Planning</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para um espaço de trabalho e um tipo de registro</p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações ao configurar regras de negócios

* Regras de negócios anexam uma condição a uma alteração de campo ou exclusão de registro. A regra só entra em ação em um momento específico e deliberado: quando um campo está prestes a ser alterado para um valor de campo configurado na regra.

* Uma regra se parece com isso em linguagem simples: &quot;Antes de editar esse registro, o campo Campaign summary deve ter um valor&quot;.

  Se o campo estiver vazio, a edição de registro será bloqueada e o usuário receberá uma mensagem clara explicando o que precisa abordar antes de seguir em frente. Depois que eles atualizam o campo obrigatório e tentam novamente, a alteração é permitida.

* As regras não bloqueiam a criação de registros. Os usuários ainda podem criar registros, mas devem garantir que os campos obrigatórios não estejam vazios ou contenham o valor especificado.
* As regras não editam ou excluem registros automaticamente. A alteração deve ser deliberada e acionada por um usuário.
* As regras não são aplicadas retroativamente: os registros antigos não são afetados. A verificação de regra só é executada na próxima vez que alguém tentar editar ou excluir um registro.
* Não é possível adicionar regras de negócios a tipos de registros globais nos espaços de trabalho principal ou secundário.
* É possível criar uma condição para a regra de negócios que faça referência a todos os tipos de campo, exceto para o seguinte:
  * Campos de fórmula
  * Campos de pesquisa
  * Campos de referência
* As regras se aplicam a todos que podem editar ou excluir registros.
* Você pode ter mais de uma regra de negócios para um tipo de registro.  <!--Syuzanna is checking this because it should be just ONE rule per action: one per edit and one per delete - see this: https://workfront.slack.com/archives/C0BHWEUSJCU/p1788281638322049?thread_ts=1787924876.280359&cid=C0BHWEUSJCU; I also logged a bug for this because it released with more than one per action - https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/6a99add600001e9aa90435ec181dec3e/overview-->

  Todas as regras são verificadas juntas ao mesmo tempo. <!-- I have asked Syuzanna and Norayr multiple times HOW are the rules run/ prioritized and I got no answers; when I know, I will update here-->

## Configurar regras de negócios

1. Ir para uma página de tipo de registro.
1. Em qualquer exibição, clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do tipo de registro e clique em **Regras de negócio**.

   A página da tabela Regras de negócio é aberta.
1. Clique em **Nova regra de negócio**.
1. Na caixa de regra **Nova empresa**, adicione um nome para a regra de negócios no primeiro campo disponível. Este campo é obrigatório
1. (Opcional) Adicione uma descrição para definir a regra de negócios e clique em **Salvar**.

   O formulário Configuração de regra de negócios é aberto.

   ![Formulário de configuração de regra de negócios](assets/business-rule-setup-form.png)

1. Na seção **Se** do formulário de configuração de regra de negócios, escolha quais ações você deseja restringir ou permitir com base em uma regra específica. Escolha entre os seguintes: <!--check UI text-->
   * **Edição de registro**: os usuários poderão editar ou não o registro, se a condição definida nesta regra for atendida.
   * **Exclusão de registro**: os usuários poderão excluir ou não o registro, se a condição definida nesta regra for atendida.
     <!--add screen shot when UI text is final-->
1. No **campo de Fórmula**, adicione a regra de negócios. Escolha um operador para a regra na seção **Expressões de fórmula** do painel direito.

   Por exemplo, você pode escolher **IF** na seção de campos **Outros** ou começar a digitar &quot;IF&quot; e depois clicar nele quando ele for exibido na lista de sugestões.

   >[!TIP]
   >
   >É recomendável selecionar os campos e operadores da lista de sugestões para manter a sintaxe da regra correta.
1. Escolha e o campo que você deseja tornar obrigatório para permitir que os registros desse tipo de registro sejam editados ou excluídos.

   Por exemplo, você pode digitar a seguinte instrução para tornar obrigatório o campo **Resumo da campanha**:

   ```
      IF(ISBLANK({Campaign summary}),"Campaign summary is a required field. You cannot edit this record without a value for the Campaign summary field.")
   ```

   >[!IMPORTANT]
   >
   >É altamente recomendável incluir na fórmula de regra as seguintes informações para facilitar a compreensão dos usuários quando uma ação que eles estão tentando executar em um registro não for permitida:
   >
   >* Os campos exatos para os quais a regra está configurada.
   >* A consequência exata se a regra não for atendida.

   Há indicadores no campo **Fórmula** quando um campo ou uma expressão está errada.  <!--add screen shot?-->

   Na seção **Then** da regra de negócios, você pode ver uma explicação do que a regra faz.

1. Clique em **Ativar** para tornar a regra ativa para este tipo de registro e em **Salvar**.

   As regras são aplicadas imediatamente após serem ativadas e todos os usuários com permissões para editar ou excluir registros no tipo de registro selecionado devem segui-las.
1. (Opcional e recomendado) Clique na seta para trás à esquerda das **Regras de negócio** no cabeçalho da página para exibir a página de tipo de registro e ir para uma exibição de tabela ou abrir a página de um registro e, em seguida, tente editar ou excluir um registro para testar a regra que acabou de criar.

## Gerenciar regras de negócios

É possível editar, excluir ou desativar as regras de negócios existentes.

A edição de uma regra existente não altera os registros existentes. A regra editada se aplica somente aos registros existentes quando alguém tenta editá-los ou excluí-los.

1. Retorne à página da tabela **Regras de negócio** para o tipo de registro.
1. Localize a regra que deseja alterar.
1. Passe o mouse sobre o nome da regra, em seguida, clique no menu **Mais** ![Mais menu](assets/more-menu.png) e, em seguida, em uma das seguintes opções:

   * **Editar**: isso abre a página de configuração da regra de negócios e permite editar informações sobre a regra de negócios.
   * **Desativar**: <!--check this in the UI: right now, it says Disable--> Isso impede que a regra seja acionada, mas preserva para o futuro, pois é necessário.
   * **Excluir**: todas as informações sobre a regra são excluídas. As regras excluídas não podem ser recuperadas.

   As regras editadas ou a desativação de regras se aplicam somente a registros futuros e não são aplicadas retroativamente.

   <!--add NEW screen shot below if UI is fixed with Deactivate at release; it was fixed in devTest-->

   <!--![Business rule more menu expanded](assets/business-rule-more-menu-in-table-expanded.png)-->

<!--

***********FROM CLAUDE - BELOW - MUST EDIT*******************


### What business rules actually do

Business rules attach a condition to a **status change**. Instead of enforcing complete data the moment someone creates a record (which would slow everyone down), the rule only kicks in at one specific, deliberate moment: when a status is about to change to a status you've configured.

A rule looks like this in plain language:

> "Before a record can move to **Ready for Execution**, the field **Brand** must have a value."

If the field is empty, the status change is blocked and the person gets a clear message telling them what to fix. Once they fill it in and try again, the change goes through.

A few important things this is *not*:

* **It doesn't block record creation.** People can still create a new record instantly and fill it in over time, exactly like today. 
* **It doesn't auto-fill anything or auto-change statuses.** A person always has to make the status change themselves.
* **It doesn't retroactively flag old records.** Records that are already sitting in the target status aren't affected — the check only runs the next time someone tries to move a record *into* that status.

### Step 1: Open the business rules configuration area

Business rules live alongside your other admin setup — you won't need to hunt for a separate "Planning" panel. From your workflow setup area:

1. Go to the main **workflow setup / admin configuration** area for your workspace.
2. Look for the **business rules** section for the record type you want to configure (for example, "Materials" or "Campaigns").


### Step 2: Choose the record type

Rules are configured per record type, so pick the one you want to add a rule to. For example, if you want to make sure every Materials record has key fields filled in before execution, select **Materials**.

### Step 3: Create a new rule

For each rule, you'll specify three things:

| What you set | Example |
|---|---|
| **Record type** | Materials |
| **Target status** | Ready for Execution |
| **Required field** | Brand |

In other words: "When a Materials record's status is changed to **Ready for Execution**, the field **Brand** must have a value."

You can add more than one rule for the same status. For example, you might require Brand, Therapeutic Area, Indication, and Estimated Launch Date all to be filled in before a record can move to "Ready for Execution" — each is its own rule, and all of them are checked together.

**What fields can you require?**

* Connected record fields (e.g., a linked Brand or Indication record) — the rule passes as soon as at least one record is linked.
* Standard text fields (single-line or paragraph) — the rule passes once there's any value.
* Date fields — the rule passes once a date is set.

**What you can't use yet:** formula fields and lookup fields aren't supported as rule targets in this release, since they're calculated in the background rather than filled in directly by a person.

### Step 4: Write the message people will see

When you create a rule, you'll also provide the message that shows up if someone tries to make the change without the field filled in. Keep it specific and actionable — something like:

> "Brand is required."

You don't need to worry about formatting a whole error banner — the system handles combining messages if multiple rules are violated at once (see below).

### Step 5: Save the rule

Once saved, the rule takes effect **immediately** for everyone in the workspace — no need to log out, refresh, or wait for a deployment. The very next time anyone tries to move a record into that status, the rule is checked.

### What your team will actually experience

Here's what changes for the people using Planning day to day, once a rule is live.

#### If a required field is empty

1. A planner opens a record and changes the status to the gated status (say, "Ready for Execution").
2. The system checks all rules tied to that status.
3. If a required field is empty, the change is **rejected** — the status reverts back to what it was.
4. A toast message appears, naming exactly which field(s) are missing:
   > *"Status change blocked: 'Brand' and 'Estimated Launch Date' must be populated before moving to 'Ready for Execution.'"*
5. The planner fills in the missing field(s) and tries the status change again.
6. This time, the rule passes, and the status updates normally.

#### If everything is already filled in

Nothing changes. The status updates instantly, with no extra steps or popups. Business rules are invisible until they're actually needed.

#### If several fields are missing at once

All the violated rules are checked together, and the message lists every missing field in one go — planners don't have to fix one field, try again, get told about the next one, and repeat.

### Step 6: Edit or remove a rule later

Rules aren't set in stone. To make changes:

1. Go back to the business rules configuration area for the record type.
2. Find the rule you want to change.
3. Edit the required field, target status, or message — or delete the rule entirely.
4. Save. The change applies immediately to future status changes.

Keep in mind: editing or deleting a rule **only affects transitions going forward.** Records that already made it into the target status before the change aren't reevaluated.
3## A few things worth knowing

* **This is separate from locking records after a status change.** Business rules (as described here) only check field completeness *before* a status change goes through. A different, related feature governs whether a record becomes fully locked from edits/deletion once it reaches a certain status — that's not what's covered here.
* **Bulk status changes** (changing status on many records at once) aren't fully defined yet for how they interact with business rules — if your team relies heavily on bulk actions, check with your Adobe contact on current behavior.
* **If a rule can't be evaluated** due to a system error, the transition is blocked rather than silently allowed through — you'll never end up with an incomplete record slipping past a rule because of a backend hiccup.
* **Turning the feature off** doesn't delete your configured rules — they're just paused. Turning it back on restores them exactly as they were, no reconfiguration needed.

### Quick reference: setting up your first rule

1. Confirm the feature is enabled for your tenant.
2. Go to workflow setup → business rules for your record type.
3. Choose the record type (e.g., Materials).
4. Create a rule: target status + required field.
5. Write a clear, specific error message.
6. Save — it's live immediately.
7. Repeat for each field you want to require.
8. Test it yourself: try changing a record's status with the field empty, confirm you see the expected message, fill in the field, and confirm the status change now goes through.

That's it — from here on, anyone converting a record forward will get a clear nudge if something's missing, instead of a downstream project quietly showing up incomplete.

-->