---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Definir tipos de horas e disponibilidade
description: Um Tipo de Hora é um rótulo que permite categorizar a entrada de tempo. Dependendo dos requisitos de horas de relatório da sua organização, essa pode ser uma parte essencial do tempo de registro.
author: Alina
feature: Timesheets
exl-id: 3c07a6b0-4751-4fce-ac28-6a83084025d4
source-git-commit: bfaf566e556882078875649549c0dfadacd800b8
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 0%

---

# Definir tipos de horas e disponibilidade

Um Tipo de Hora é um rótulo que permite categorizar a entrada de tempo. Dependendo dos requisitos de horas de relatório da sua organização, essa pode ser uma parte essencial do tempo de registro.

Há dois conjuntos de tipos de horas no Adobe Workfront:

* **Horas gerais:** horas que não estão associadas a um projeto, como um período de licença médica ou administração. Você pode registrar horas gerais somente na folha de horas.
* **Horas específicas do projeto:** horas registradas em projetos, tarefas e problemas. Você pode registrar horas específicas do projeto de qualquer local em que possa registrar horas.

Ao registrar o tempo no Workfront, os tipos de horas específicos do projeto que estão disponíveis dependem das opções de configuração definidas nos níveis do sistema, do projeto e do usuário. (Os seguintes tipos de horas específicos do projeto padrão estão sempre disponíveis: Hora do projeto, Hora da tarefa e Hora do problema.)

Os tipos de horas disponíveis para seleção ao registrar horas (em projetos, tarefas e problemas) são determinados primeiro pelos tipos de horas disponibilizados em todo o sistema pelo administrador do sistema e, em seguida, pelos tipos de horas selecionados nos níveis de projeto e usuário.

Após a configuração dos tipos de horas apropriados, você poderá registrar horas de vários locais no Workfront, conforme descrito em [Registrar horas](../../timesheets/create-and-manage-timesheets/log-time.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso de administrador do sistema para definir tipos de horas em todo o sistema e editar todos os usuários</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>Gerenciar o acesso no projeto para definir tipos de horas em um projeto</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber que tipo de plano ou licença você tem, contate o administrador do Workfront.

+++

## Definir disponibilidade no nível do sistema

O administrador do sistema determina quais tipos de horas específicos do projeto são disponibilizados em todo o sistema, conforme descrito em [Gerenciar tipos de horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Definir disponibilidade no nível do projeto {#define-availability-at-the-project-level}

O proprietário do projeto determina se todos os tipos de horas definidos no nível do sistema estão disponíveis no projeto (e tarefas e problemas dentro do projeto) ou se apenas um subconjunto desses tipos de horas está disponível.

1. Vá para o projeto em que deseja determinar a disponibilidade dos tipos de horas.
1. Clique no menu **Mais** ao lado do nome da tarefa e clique em **Editar**.

1. Clique em **Editar projeto**.
1. Na seção **Configurações**, localize a opção **Filtrar Tipos de Hora**.

1. Selecione **Não** para disponibilizar todos os tipos de horas específicos do projeto.

   Ou

   Selecione **Sim** para disponibilizar no projeto apenas um subconjunto dos tipos de horas específicos do projeto e, em seguida, selecione os tipos de horas que deseja disponibilizar. (Mantenha pressionada a tecla Shift para selecionar vários tipos de horas.)

   Se você selecionar essa opção, somente os tipos de horas selecionados serão disponibilizados para seleção ao registrar horas no projeto (ou em tarefas e problemas no projeto). Se você selecionar essa opção e não selecionar nenhum tipo de hora, o projeto exibirá somente tipos de hora gerais.

   As mesmas seleções devem ser feitas no nível do usuário individual para que o usuário veja essas opções de tipo de hora no projeto.

   Quando o tipo de hora padrão do usuário e um tipo de hora filtrado do projeto são correspondentes, esse tipo de hora é selecionado por padrão ao registrar o tempo.

1. Clique em **Salvar alterações**.

## Definir disponibilidade no nível do usuário

Você pode registrar horas para um determinado tipo de hora em projetos, tarefas e problemas somente se esse tipo de hora tiver sido disponibilizado no nível do sistema, do projeto e do usuário.

Se você disponibilizar um tipo de hora no nível do usuário conforme descrito nesta seção, mas não o vir ao registrar horas em um projeto, tarefa ou problema, esse tipo de hora não será disponibilizado no projeto (conforme descrito em [Definir disponibilidade no nível do projeto](#define-availability-at-the-project-level)).

Para definir os tipos de horas disponíveis para um usuário:

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu principal**, no canto superior direito do Adobe Workfront.

1. Clique no avatar do usuário no canto superior esquerdo.
1. Clique no menu **Mais** ao lado do nome de usuário e clique em **Editar**.

1. Somente um administrador do sistema pode editar outros usuários. Se você tiver uma licença de Plano, poderá editar os tipos de horas em seu próprio perfil.
1. Na seção **Planejamento de Recursos**, no menu suspenso **Tipos de Horas Disponíveis**, siga um destes procedimentos, dependendo de quais tipos de horas você deseja disponibilizar ao registrar horas em um projeto, tarefa ou problema:

   * **Para disponibilizar todos os tipos de horas para o usuário:** Selecione todos os tipos de horas.\
     Se você deixar todos os tipos de horas desmarcados, tecnicamente será o mesmo que selecionar todos os tipos de horas. No entanto, nesse caso, todos os tipos de horas estão disponíveis para o usuário somente em projetos, tarefas e problemas em que **Não** está selecionado na opção **Filtrar Tipos de Horas** ao editar o projeto, conforme descrito em [Definir disponibilidade no nível do projeto](#define-availability-at-the-project-level).
   * **Para disponibilizar ao usuário apenas um subconjunto dos tipos de horas:** Selecione apenas os tipos de horas que deseja disponibilizar.

     Para que os tipos de horas selecionados no nível do usuário estejam disponíveis em projetos, tarefas e problemas, esses mesmos tipos de horas também devem ser selecionados na opção **Filtrar Tipos de Horas** ao editar o projeto, conforme descrito em [Definir disponibilidade no nível do projeto](#define-availability-at-the-project-level).

1. (Opcional) No menu suspenso **Tipo de hora padrão**, selecione um tipo de hora.

   Quando o tipo de hora padrão do usuário e um tipo de hora filtrado do projeto são correspondentes, esse tipo de hora é selecionado por padrão ao registrar o tempo.

1. Clique em **Salvar alterações**.

   Agora, quando você registra horas em um projeto, tarefa ou problema, os tipos de horas selecionados ficam disponíveis se esses mesmos tipos de horas tiverem sido disponibilizados no nível do projeto.


## Como os tipos de hora no nível do usuário e no nível do projeto funcionam juntos

A lista a seguir descreve quais tipos de horas são exibidos em um objeto após você ter personalizado e filtrado os tipos de horas no nível do usuário e no nível do projeto ao registrar horas no objeto:

* Depois de personalizar o Tipo de hora padrão para o usuário e os Tipos de hora do projeto filtrados, o menu suspenso Tipo de hora exibe um dos seguintes tipos de hora:

   * Quando o usuário tem um Tipo de hora padrão em seu perfil e o projeto tem o mesmo Tipo de hora filtrado, esse Tipo de hora é exibido como o padrão selecionado ao registrar o tempo; o Tempo do projeto, da tarefa ou do problema é exibido como opções adicionais.

   * Quando o usuário não tem um Tipo de Hora Padrão e o Projeto tem Tipos de Hora Filtrados, o Tipo de Hora padrão ao registrar o tempo é Projeto, Tarefa ou Tempo de Problema, mas os Tipos de Hora filtrados do projeto também são exibidos como opções adicionais.

   * Quando o usuário não tem um Tipo de Hora Padrão e o projeto não tem Tipos de Hora Filtrados, somente os tipos de hora Projeto, Tarefa ou Problema são exibidos como padrão, dependendo do objeto no qual você está registrando o tempo.

   * Quando o usuário tem um Tipo de Hora Padrão e o projeto não tem Tipos de Hora Filtrados, o Projeto, Tarefa ou Tempo de Problema é exibido como padrão ao registrar o tempo nos objetos e nenhum outro Tipo de Hora está disponível como opções, incluindo o Tipo de Hora Padrão do usuário.

* Depois de personalizar os Tipos de horas e definir os Tipos de horas disponíveis para o seu usuário ou filtrar os Tipos de horas para um projeto, existem os seguintes cenários:

   * Quando você selecionou todos os tipos de horas para o campo Tipo de hora disponível no perfil do usuário e os Tipos de hora do projeto não estão filtrados, você verá todos os tipos de horas disponíveis ao registrar horas.
   * Quando você selecionou apenas um subconjunto de tipos de hora para o campo Tipo de hora disponível no perfil do usuário e os Tipos de hora do projeto não estão filtrados, você verá apenas os tipos de hora do usuário ao registrar horas.
   * Quando você selecionou todos os tipos de hora para o campo Tipo de hora disponível no perfil do usuário e os Tipos de hora do projeto estão filtrados, você verá apenas os tipos de hora do projeto e os tipos de hora padrão como Tempo do projeto, Tempo da tarefa, Tempo do problema, dependendo do objeto.
   * Quando você selecionou apenas um subconjunto de tipos de hora para o campo Tipo de hora disponível no perfil do usuário e os Tipos de hora do projeto estão filtrados, você verá apenas os tipos de hora que são comuns ao usuário e ao projeto. Se nenhum tipo de hora for comum ao usuário e ao projeto, somente os tipos de hora padrão serão exibidos (Hora do projeto, Hora da tarefa, Hora do problema).

>[!TIP]
>
>   Se você selecionar um tipo de hora diferente em vez do tipo de hora padrão para um objeto, o tipo de hora se tornará fixo. Na próxima vez que você fizer logon no mesmo objeto, o Tipo de hora assumirá automaticamente como padrão o tipo selecionado pela última vez.

