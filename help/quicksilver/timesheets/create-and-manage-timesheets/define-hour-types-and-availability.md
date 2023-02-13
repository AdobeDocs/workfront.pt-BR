---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Definir os tipos de hora e a disponibilidade das folhas de horas
description: Um Tipo de hora é um rótulo que permite categorizar a entrada de tempo. Dependendo dos requisitos de relatório da sua organização para horas, isso pode ser uma parte essencial do tempo de registro.
author: Alina
feature: Timesheets
exl-id: 3c07a6b0-4751-4fce-ac28-6a83084025d4
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '920'
ht-degree: 0%

---

# Definir os tipos de hora e a disponibilidade das folhas de horas

Um Tipo de hora é um rótulo que permite categorizar a entrada de tempo. Dependendo dos requisitos de relatório da sua organização para horas, isso pode ser uma parte essencial do tempo de registro.

Há dois conjuntos de tipos de hora no Adobe Workfront:

* **Horas gerais:** Horas que não estão associadas a um projeto, como tempo de doença ou administração. Você pode registrar horas gerais somente na folha de horas.
* **Horas específicas do projeto:** Horas conectadas a projetos, tarefas e problemas. Você pode registrar horas específicas do projeto a partir de qualquer local em que possa registrar o tempo.

Ao fazer logon no Workfront, os tipos de hora específicos do projeto que estão disponíveis dependem das opções de configuração definidas nos níveis do sistema, do projeto e do usuário. (Os seguintes tipos de hora padrão específicos do projeto estão sempre disponíveis: Hora do projeto, Hora da tarefa e Hora da ocorrência.)

Os tipos de hora disponíveis para selecionar ao registrar o tempo (em projetos, tarefas e problemas) são determinados primeiro pelos tipos de hora disponibilizados em todo o sistema pelo administrador do sistema e, em seguida, pelos tipos de hora selecionados nos níveis do projeto e do usuário.

Após configurar os tipos de hora apropriados, você pode registrar o tempo de vários locais no Workfront, conforme descrito em [Tempo de registro](../../timesheets/create-and-manage-timesheets/log-time.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Planejar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso do administrador do sistema para definir tipos de hora em todo o sistema e editar todos os usuários</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>Gerenciar o acesso no projeto para definir tipos de hora em um projeto</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano ou tipo de licença você possui, entre em contato com o administrador da Workfront.

## Definir a disponibilidade no nível do sistema

O administrador do sistema determina quais tipos específicos de hora do projeto são disponibilizados em todo o sistema, conforme descrito na [Gerenciar tipos de hora](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md) seção em  [Gerenciar tipos de hora](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Definir a disponibilidade no nível do projeto {#define-availability-at-the-project-level}

O proprietário do projeto determina se todos os tipos de hora definidos no nível do sistema estão disponíveis no projeto (e tarefas e problemas no projeto) ou se apenas um subconjunto desses tipos de hora está disponível. 

1. Vá para o projeto onde deseja determinar a disponibilidade dos tipos de hora.
1. Clique no botão **Mais** ao lado do nome da tarefa, em seguida, clique em **Editar**.

1. Clique em **Editar projeto**.
1. No **Configurações** localize a **Filtrar tipos de horas** opção.

1. Selecionar **Não** para disponibilizar todos os tipos de hora específicos do projeto no projeto.

   Ou

   Selecionar **Sim** para disponibilizar apenas um subconjunto dos tipos de hora específicos do projeto no projeto, selecione os tipos de hora que deseja disponibilizar. (Mantenha pressionada a tecla Shift para selecionar vários tipos de hora.)

   Se você selecionar essa opção, somente os tipos de hora selecionados serão disponibilizados para selecionar ao registrar horas no projeto (ou em tarefas e problemas no projeto). Se você selecionar essa opção e não selecionar nenhum tipo de hora, o projeto exibirá apenas tipos de hora gerais.

   As mesmas seleções devem ser feitas no nível do usuário individual para que o usuário veja essas opções de tipo de hora no projeto.

1. Clique em **Salvar alterações**.

## Definir a disponibilidade no nível do usuário

Você pode registrar horas para um determinado tipo de hora em projetos, tarefas e problemas somente se esse tipo de hora tiver sido disponibilizado no nível do sistema, no nível do projeto e no nível do usuário.

Se você disponibilizar um tipo de hora no nível do usuário, conforme descrito nesta seção, mas não vir esse tipo de hora ao fazer logon em um projeto, tarefa ou problema, esse tipo de hora não foi disponibilizado no projeto (conforme descrito em [Definir a disponibilidade no nível do projeto](#define-availability-at-the-project-level)).

Para definir os tipos de hora que estão disponíveis para um usuário:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique no avatar do usuário no canto superior esquerdo.
1. Clique no botão **Mais** ao lado do nome do usuário e clique em **Editar**.

1. Somente um administrador de sistema pode editar outros usuários. Se você tiver uma licença do Plan , poderá editar os tipos de hora em seu próprio perfil.
1. No **Planejamento de recursos** na seção **Tipos de hora disponíveis** no menu suspenso, execute um dos procedimentos a seguir, dependendo dos tipos de hora que deseja disponibilizar ao fazer logon em um projeto, tarefa ou problema:

   * **Para disponibilizar todos os tipos de hora para o usuário:** Selecione todos os tipos de hora.\
      Se não selecionar todos os tipos de hora, tecnicamente é o mesmo que selecionar todos os tipos de hora. No entanto, nesse caso, todos os tipos de hora estão disponíveis para o usuário somente em projetos, tarefas e problemas em que **Não** é selecionado no **Filtrar tipos de horas** ao editar o projeto, conforme descrito em [Definir a disponibilidade no nível do projeto](#define-availability-at-the-project-level).
   * **Para disponibilizar apenas um subconjunto dos tipos de hora para o usuário:** Selecione apenas os tipos de hora que deseja disponibilizar.

      Para que os tipos de hora selecionados no nível do usuário estejam disponíveis em projetos, tarefas e problemas, esses mesmos tipos de hora também devem ser selecionados na variável **Filtrar tipos de horas** ao editar o projeto, conforme descrito em [Definir a disponibilidade no nível do projeto](#define-availability-at-the-project-level).

1. Clique em **Salvar alterações**.

   Agora, ao registrar horas em um projeto, tarefa ou problema, os tipos de hora selecionados estarão disponíveis se esses mesmos tipos de hora tiverem sido disponibilizados no nível do projeto.
