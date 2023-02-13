---
product-area: projects
navigation-topic: business-case-and-scorecards
title: Criar e editar riscos em projetos
description: Os riscos são possíveis eventos ou fatores que impedem que um projeto termine a tempo ou dentro do orçamento. Os riscos podem ser registrados como parte da criação do Caso de negócios de um projeto ou usando a guia Riscos . Os riscos são criados apenas em um projeto. Não é possível associar riscos a tarefas ou problemas.
author: Alina
feature: Work Management
exl-id: 6125c477-c0d8-43b4-88d8-35b0c2412468
source-git-commit: 8611c7bf8be6405f8ec8462ff2fd0f5998e8a995
workflow-type: tm+mt
source-wordcount: '1083'
ht-degree: 0%

---

# Criar e editar riscos em projetos

Os riscos são possíveis eventos ou fatores que impedem que um projeto termine a tempo ou dentro do orçamento. Os riscos podem ser registrados como parte da criação do Caso de negócios de um projeto ou usando a guia Riscos . Os riscos são criados apenas em um projeto. Não é possível associar riscos a tarefas ou problemas.

Os riscos podem estar associados ao custo, mas o Custo de Risco Real não afeta o Custo Real do Projeto.

>[!NOTE]
>
>Este artigo define os riscos associados ao projeto conforme você os define no Caso de negócios do projeto ou como você os adiciona na guia Riscos do projeto. Para obter informações sobre o campo Risco que está disponível ao editar um projeto, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos e Dados Financeiros</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p> Gerencie permissões que incluem Gerenciar finanças no projeto para o qual deseja criar ou editar riscos </p> <p>Para obter mais informações sobre permissões de projeto, consulte o artigo <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Compartilhar um projeto no Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Criar e editar riscos no Caso de negócios

Você pode criar riscos como parte do planejamento do Caso de negócios de um projeto. Posteriormente, você pode editá-las no Caso de negócios, quando ocorrerem alterações em sua probabilidade, plano de mitigação ou custo, por exemplo. Para obter informações sobre como criar um Caso de Negócios, consulte [Criar um caso de negócios para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

O administrador do Workfront ou o administrador do grupo deve habilitar o **Riscos** na seção Caso de negócios na área Preferências do projeto antes de visualizá-la no nível do projeto na seção Caso de negócios . Para obter informações sobre como definir preferências de projeto, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Criar e editar riscos no Caso de negócios é idêntico.

Para criar ou editar um risco no Caso de negócios:

1. Vá para o projeto para o qual deseja criar riscos.
1. Clique em **Caso de negócios** no painel esquerdo.
1. No **Riscos** seção , clique em **Editar riscos**.
1. Insira ou edite as seguintes informações:

   * **Descrição:** descrever o risco.

   * **Custo potencial**: indicar o custo estimado se o risco deve ocorrer.

   * **Probabilidade**: indicar a probabilidade de o risco ocorrer como valor percentual.

   * **Tipo:** indicar a categoria em que o risco se insere.
   * **Plano de mitigação**: atualizar a descrição do plano para mitigar o risco.

   * **Custo da mitigação**: indicar o custo do plano de atenuação que deve ser criado para evitar que o risco ocorra.

   ![](assets/crp1-350x117.png)

1. (Opcional) Clique em **Adicionar Outro Risco** acrescentar riscos adicionais.
1. Clique em **Salvar**.

## Criar e editar riscos na área Riscos

Além de criar e editar riscos no Caso de negócios, você pode fazer isso usando o **Riscos** de um projeto.

* [Criar riscos na área Riscos](#create-risks-in-the-risks-area)
* [Editar riscos na área Riscos](#edit-risks-in-the-risks-area)

### Criar riscos na área Riscos {#create-risks-in-the-risks-area}

1. Vá para o projeto para o qual deseja criar riscos.
1. Clique em **Riscos** no painel esquerdo.

   ![Seção Riscos da tarefa](assets/risks-section-on-project-2022.png)

1. Clique em **Comece A Adicionar Riscos** e criar riscos editando suas informações em linha.

   Ou

   Clique em **Novo risco**. O **Novo risco** será aberta.

1. Insira as seguintes informações:

   * **Descrição**: descrever o risco.
   * **Tipo de risco**: indicar a categoria em que o risco se insere.\
      O administrador do Workfront define os Tipos de risco disponíveis no seu ambiente. Para obter informações sobre como definir Tipos de Risco, consulte o artigo [Editar e criar tipos de risco](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

   * **Probabilidade**: indicar a probabilidade de o risco ocorrer como valor percentual.
   * **Custo potencial**: indicar o custo estimado se o risco deve ocorrer.
   * **Custo da mitigação**: indicar o custo do plano de atenuação que deve ser criado para evitar que o risco ocorra.
   * **Custo real**: Indicar o custo real do risco em caso de ocorrência do risco.
   * **Plano de mitigação**: atualizar a descrição do plano para mitigar o risco.

1. (Condicional) Clique em **Enter** se você estiver criando o risco em linha.

   Ou

   Clique em **Salvar** se você estiver editando as informações no **Novo risco** caixa de diálogo.

1. (Opcional) Selecione um **Status** para o risco, na **Status** no menu suspenso, ao aplicar a variável **Padrão** exibir a lista de riscos.

   Por padrão, o Status de um risco é **Identificado**.

### Editar riscos na área Riscos {#edit-risks-in-the-risks-area}

É possível editar riscos durante a vida de um projeto, quando ocorrerem alterações em sua probabilidade, custo potencial ou status, por exemplo.

Você pode editar um risco por vez ou editar vários riscos em massa.

Para editar riscos:

1. Navegue até um projeto para o qual deseja editar os riscos existentes.
1. Clique em **Riscos** no painel esquerdo.
1. Comece a editar os campos dos riscos que você vê na lista para editar um risco de cada vez.

   Ou

   Selecione um ou vários riscos e clique em **Editar** para editar vários riscos ao mesmo tempo.

   >[!NOTE]
   >
   >Você está aplicando as mesmas informações a todos os riscos selecionados, ao editar vários riscos ao mesmo tempo. As informações associadas a cada risco antes de suas alterações são substituídas em uma edição em massa.

1. Se tiver clicado **Editar**, o **Editar risco** será aberta.

   Considere editar os seguintes campos:

   * **Descrição**: edite a descrição do risco.
   * **Tipo de risco**: indicar a categoria em que o risco se insere.
   * **Probabilidade**: indicar a probabilidade de o risco ocorrer como valor percentual.
   * **Custo potencial**: indicar o custo estimado se o risco deve ocorrer.
   * **Custo da mitigação**: indicar o custo do plano de atenuação que deve ser criado para evitar que o risco ocorra.
   * **Custo real**: Indicar o custo real do risco em caso de ocorrência do risco.
   * **Plano de mitigação**: atualizar a descrição do plano para mitigar o risco.

1. Clique em **Salvar alterações**.
1. (Opcional) Edite o **Status** para um risco, na **Status** no menu suspenso, ao aplicar a variável **Padrão** exibir a lista de riscos.

   >[!NOTE]
   >
   >Não é possível editar o **Status** dos riscos **Editar risco** caixa de diálogo. Isso só pode ser feito em uma edição em linha.
