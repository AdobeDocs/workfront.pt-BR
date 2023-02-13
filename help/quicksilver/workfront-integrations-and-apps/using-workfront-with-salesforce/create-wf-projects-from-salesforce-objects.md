---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: Criar [!DNL Adobe Workfront] projetos de [!DNL Salesforce] objetos
description: Depois de instalar [!DNL Adobe Workfront] para o Salesforce, você pode definir acionadores que criam [!DNL Workfront] projetos em que determinados critérios sejam cumpridos [!DNL Salesforce] Oportunidades e Contas.
author: Becky
feature: Workfront Integrations and Apps
exl-id: b38c91ae-342b-4002-a947-7a0ab1aaca93
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '1507'
ht-degree: 3%

---

# Criar [!DNL Adobe Workfront] projetos de [!DNL Salesforce] objetos

Depois de instalar [!DNL Adobe Workfront] para o Salesforce, você pode definir acionadores que criam [!DNL Workfront] projetos em que determinados critérios sejam cumpridos [!DNL Salesforce] [!UICONTROL Oportunidades] e [!UICONTROL Contas].

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade descrita neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Pré-requisitos

Para enviar uma [!DNL Workfront] de um [!DNL Salesforce] [!UICONTROL Oportunidade] ou Conta certifique-se de ter as seguintes informações em seu ambiente:

* Seu [!DNL Workfront] administrador instalado [!DNL Workfront for Salesforce].\
   Para obter mais informações sobre a instalação [!DNL Workfront for Salesforce], consulte [Instalar [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* Seu [!DNL Workfront] o administrador adicionou o [!DNL Workfront] seção à sua [!UICONTROL Oportunidade] e layouts de página de conta.\
   Para obter mais informações sobre como adicionar o [!DNL Workfront] para um layout de página, consulte [Configure o [!DNL Adobe Workfront] seção para [!DNL Salesforce] usuários](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Você tem um [!DNL Workfront] e você pode fazer logon nela pelo [!DNL Workfront] seção dentro de sua [!UICONTROL Oportunidade] ou Conta .

## Configurar a criação de [!DNL Workfront] Projetos de [!DNL Salesforce]

* [Noções básicas sobre a criação automática de projetos](#understanding-the-automatic-creation-of-projects-understanding-the-automatic-creation-of-projects)
* [Configuração de acionadores](#configuring-triggers-configuring-triggers)
* [Noções básicas sobre nomes de projetos](#understanding-project-names-understanding-project-names)

### Noções básicas sobre a criação automática de projetos {#understanding-the-automatic-creation-of-projects}

Como [!DNL Salesforce] administrador do sistema, você pode definir acionadores que podem criar projetos automaticamente em [!DNL Workfront] quando as seguintes coisas acontecem em [!DNL Salesforce]:

* O [!UICONTROL Fase] de um [!UICONTROL Oportunidade] é atualizado.
* O [!UICONTROL Tipo] de uma Conta é atualizada.

Os acionadores só poderão ser configurados depois que você tiver instalado [!DNL Workfront for Salesforce].  \
Para obter informações sobre a instalação [!DNL Workfront for Salesforce], consulte [Instalar [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Considere o seguinte ao configurar acionadores para criar automaticamente [!DNL Workfront] projetos quando [!DNL Salesforce] Os itens são criados ou atualizados:

* Você deve ser um [!DNL Salesforce] e [!DNL Workfront] administrador do sistema para configurar acionadores.
* Depois de configurar os acionadores, qualquer pessoa que atualize o [!UICONTROL Fase] de um [!UICONTROL Oportunidade] ou [!UICONTROL Tipo] de uma Conta pode acionar a criação de um [!DNL Workfront] projeto. Isso inclui [!DNL Salesforce] usuários que não têm um [!DNL Workfront] conta.
* Não há limite para quantos acionadores você pode ter.
* Não é possível criar vários acionadores com base nas mesmas condições. Os acionadores são exclusivos por padrão.
* Depois que o projeto é criado, ele é vinculado automaticamente à oportunidade ou à conta em que foi gerado. Depois de estabelecido, esse link não pode ser interrompido.
* Uma oportunidade ou conta pode ser vinculada a vários projetos em [!DNL Workfront] quando uma condição acionada tiver sido cumprida várias vezes durante a vida da oportunidade ou da conta.

   Por exemplo, se você definir mais de um [!UICONTROL Fase] para um [!UICONTROL Oportunidade] para acionar um projeto, um projeto é criado para cada estágio definido que a oportunidade atinge, pela vida dessa oportunidade. Além disso, se você atualizar o [!UICONTROL Fase] de um [!UICONTROL Oportunidade] de um estágio definido para outro e, em seguida, atualizá-lo de volta ao estágio definido, um segundo projeto será criado pela segunda vez que você atualizar o [!UICONTROL Fase] para o mesmo estágio definido.

* Um projeto em [!DNL Workfront] pode ser vinculado somente a uma oportunidade ou uma conta em [!DNL Salesforce] em qualquer momento, mas não para ambos ao mesmo tempo.

### Configuração de acionadores {#configuring-triggers}

Depois de configurar os acionadores, o processo de criação [!DNL Workfront] projetos estão habilitados para ambos [!UICONTROL Salesforce Classic] ou [!DNL Lightning Experience] quadros.

Para configurar acionadores em [!UICONTROL Salesforce]:

1. Faça logon em [!DNL Salesforce] como administrador do sistema.
1. (Condicional) Em [!DNL Salesforce Classic], clique em **[!UICONTROL Configuração]** e sob o **[!UICONTROL Criar]** seção, expandir **[!UICONTROL Relâmpago]**.

   Ou

   Em [!DNL Salesforce] Experiência do Lightning, clique no botão **[!UICONTROL Configuração] ícone**, em seguida **[!UICONTROL Configuração]** e sob **[!UICONTROL FERRAMENTAS DA PLATAFORMA]** expandir **[!UICONTROL Aplicativos]**.

1. Clique em **[!UICONTROL Pacotes instalados]**.

   Observe que a variável **[!DNL Workfront]** pacote foi instalado.

1. Clique em **[!UICONTROL Configurar]** ao lado de **[!DNL Workfront]**.

1. Faça logon em [!DNL Workfront] como administrador do sistema.

   O **[!UICONTROL Triggers]** será exibida.

   ![salesforce_triggers_page_empty.png](assets/salesforce-triggers-page-empty-350x134.png)

1. Clique em **[!UICONTROL Novo acionador]**.
1. No **[!UICONTROL [!DNL Salesforce]Objeto]** , selecione **[!UICONTROL Oportunidade]**.

   Este campo é obrigatório.

1. (Condicional) Especifique o seguinte:

   1. No **[!UICONTROL Fase]** selecione um **[!UICONTROL Fase]**.\

      Quando uma oportunidade atinge o [!UICONTROL Fase] especificado aqui, um projeto é criado em [!DNL Workfront]. Este campo é obrigatório.

   1. No **[!UICONTROL Portfolio ou Programa]** , comece digitando o nome de um Portfolio ou Programa no qual você deseja colocar o projeto [!DNL Workfront], em seguida, selecione-o quando aparecer na lista.\

      Se você não especificar um Portfolio ou um Programa, o novo projeto será criado e adicionado ao [!UICONTROL Projetos que possuo] lista de usuários conectados ao [!DNL Workfront] ao configurar os acionadores. Esse usuário também é o Proprietário do projeto do novo projeto.

   1. Comece a digitar o nome de um Modelo que deseja associar ao novo [!DNL Workfront] , selecione-o quando aparecer na lista.\

      Este campo é obrigatório.


      >[!NOTE]
      >
      >Se você tiver especificado um Proprietário de modelo no modelo que pretende usar para essa integração, ele se tornará o Proprietário do projeto do novo projeto. Os novos projetos aparecem no [!UICONTROL Projetos que possuo] lista do usuário que é o proprietário do novo projeto, de acordo com o modelo.

   1. (Opcional) Selecione o **[!UICONTROL Criar um novo projeto para cada tipo de produto vendido] campo**, caso deseje criar um novo projeto para cada tipo de produto vendido em uma oportunidade única.
   1. (Condicional) Selecione um **[!UICONTROL Produto]** no **[!UICONTROL Produto]** menu suspenso.

      Este campo é obrigatório.

   1. (Condicional) Comece a digitar o nome de um **[!UICONTROL Modelo]** que você deseja associar ao novo [!DNL Workfront] projeto se o Produto especificado estiver no [!UICONTROL Oportunidade]. Selecione-o quando aparecer na lista.

      Este campo é obrigatório.

      O projeto criado quando um novo produto é adicionado ao [!DNL Salesforce] é colocada no mesmo Portfolio ou Programa selecionado para a oportunidade.

      >[!IMPORTANT]
      >
      >O projeto é criado somente quando o Estágio é atualizado no [!UICONTROL Oportunidade]. Um projeto exclusivo é criado para cada produto especificado quando o campo Estágio é atualizado, e não como os produtos são adicionados a [!UICONTROL Oportunidades].

1. (Opcional) Clique em **[!UICONTROL Novo acionador]**.
1. (Opcional) Na **[!UICONTROL [!DNL Salesforce]Objeto]** selecione **Conta **.

   Este campo é obrigatório.
1. (Condicional) Especifique o seguinte:

   1. Selecione um **[!UICONTROL Tipo]** do **[!UICONTROL Tipo]** menu suspenso.

      Quando qualquer **Conta ** é designada como **[!UICONTROL Tipo]** especificado aqui em [!DNL Salesforce], a **[!UICONTROL Projeto]** é criado em [!DNL Workfront].

      Este campo é obrigatório.

   1. (Opcional) Comece a digitar o nome de um **[!UICONTROL Portfolio]** ou **[!UICONTROL Programa]** onde deseja colocar o projeto [!DNL Workfront] no **[!UICONTROL Portfolio ou Programa]** e selecione-o quando aparecer na lista.

      Se você não especificar um Portfolio ou um Programa, o novo projeto será criado e adicionado ao **[!UICONTROL Projetos que possuo]** lista de usuários conectados ao [!DNL Workfront] from [!DNL Salesforce]. O usuário também é o Proprietário do projeto do novo projeto.

   1. Comece a digitar o nome de um **[!UICONTROL Modelo]** que você deseja associar ao novo [!DNL Workfront] , selecione-o quando aparecer na lista.

      Este campo é obrigatório.

      >[!NOTE]
      >
      >Se você tiver especificado um Proprietário de modelo no modelo que pretende usar para essa integração, ele se tornará o Proprietário do projeto do novo projeto. Os novos projetos aparecem no **[!UICONTROL Projetos que possuo]** lista do usuário que é o proprietário do novo projeto, de acordo com o modelo.
   ![salesforce_triggers_page_with_clean_up_template_names.png](assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png)

1. Clique em **[!UICONTROL Salvar]**.

   [!DNL Workfront] agora os projetos são gerados toda vez que qualquer um dos acionadores é atendido.

### Noções básicas sobre nomes de projetos {#understanding-project-names}

Dependendo de qual acionador gerou os projetos, os nomes dos projetos em [!DNL Workfront] pode seguir um destes padrões:

* Se o projeto for criado com base em uma oportunidade ou acionador de conta, o nome do projeto será: *`<Salesforce object name>`: `<Project template name>` (via [!DNL Salesforce])*.
* Se o projeto for criado com base em um acionador de oportunidade que também inclua a adição de um novo Produto, o nome do projeto será: *`<Salesforce object name>`: `<Salesforce product name>` (via [!DNL Salesforce])*.

## Exibir [!DNL Workfront] projetos

Se o seu [!DNL Workfront] o administrador adicionou o [!DNL Workfront] seção à sua [!UICONTROL Oportunidade] Para o layout da página Conta, é possível ver os projetos criados automaticamente no [!UICONTROL Projetos] desta seção.\
Para obter mais informações sobre como adicionar o [!DNL Workfront] para o layout de página de um [!UICONTROL Oportunidade] ou Conta , consulte [Configure o [!DNL Adobe Workfront] seção para [!DNL Salesforce] usuários](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

Você deve ter um [!DNL Workfront] e estar conectado a [!DNL Workfront] para visualizar o [!UICONTROL Projetos] guia .

Para visualizar projetos criados a partir de um [!UICONTROL Oportunidade] ou Conta :

1. Ir para um [!UICONTROL Oportunidade] ou Conta .
1. Vá para o **[!DNL Workfront]** seção.

   >[!NOTE]
   >
   >Dependendo de como o [!DNL Workfront] O administrador configurou esta seção e pode ter um nome diferente.

1. Selecione o **[!UICONTROL Projetos]** guia .

   Todos os projetos criados por acionadores definidos são listados nesta guia. Qualquer usuário em [!DNL Salesforce] que também tem uma [!DNL Workfront] e quem pode ter permissões para ver esses projetos em [!DNL Workfront] também pode visualizá-los em [!DNL Salesforce] para [!UICONTROL Oportunidade] ou a Conta que os gerou.

   ![[!DNL salesforce_projects_tab_with_projects_listed].png](assets/salesforce-projects-tab-with-projects-listed-350x150.png)

   Você pode exibir as seguintes informações sobre os projetos criados pela integração:

   * Nome do Projeto
   * Número de Referência
   * Data de Entrada
   * Nome do Proprietário
   * Status
   * Condição
   * Data de conclusão planejada
   * Percentual concluído

      Quando essas informações são atualizadas em [!DNL Workfront], você pode ver os campos atualizados nesta lista.

1. (Opcional) Clique no nome de um projeto para abri-lo no Workfront.
1. (Opcional) Clique em [!UICONTROL **[!UICONTROL Ir para o Salesforce]**] no [!UICONTROL Detalhes do projeto] ou o cabeçalho do projeto para acessar a variável [!UICONTROL Oportunidade] ou a Conta de origem do projeto. O administrador do sistema ou do grupo deve adicionar a variável [!UICONTROL Integrações] para o modelo de layout e localizá-lo no cabeçalho do projeto.

   >[!NOTE]
   >
   >O [!UICONTROL Ir para o Salesforce] link é visível para todos [!DNL Workfront] usuários que podem visualizar o projeto. Você deve ter um [!DNL Salesforce] para poder acessar a [!DNL Salesforce] Oportunidade ou Conta de onde o projeto foi gerado.
