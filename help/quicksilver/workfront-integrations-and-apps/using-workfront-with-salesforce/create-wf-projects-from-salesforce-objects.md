---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: Criar [!DNL Adobe Workfront] projetos de [!DNL Salesforce] objetos
description: Após instalar o [!DNL Adobe Workfront] for Salesforce, você poderá definir acionadores que criem [!DNL Workfront] projetos quando determinados critérios forem atendidos em [!DNL Salesforce] Oportunidades e Contas.
author: Becky
feature: Workfront Integrations and Apps
exl-id: b38c91ae-342b-4002-a947-7a0ab1aaca93
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '1573'
ht-degree: 3%

---

# Criar [!DNL Adobe Workfront] projetos a partir de [!DNL Salesforce] objetos

>[!IMPORTANT]
>
>Para fornecer integrações mais estáveis e escaláveis, estamos mudando para uma abordagem de integração moderna e flexível usando a Automação e Integração do Workfront (Fusion). Como parte desse processo de transição, a integração do Workfront para Salesforce não estará disponível após **28 de fevereiro de 2026**.
>
>Recomendamos usar a Automação e integração do Workfront para as necessidades de integração de sua organização com o Salesforce.
>
>Para obter uma visão geral da Automação e Integração do Workfront, consulte [Visão geral do Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obter informações sobre os recursos específicos dos módulos de Automação e Integração do Workfront para Salesforce, consulte [módulos do Salesforce](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

Depois de instalar o [!DNL Adobe Workfront] for Salesforce, você poderá definir acionadores que criam projetos [!DNL Workfront] quando determinados critérios forem atendidos em [!DNL Salesforce] [!UICONTROL Oportunidades] e [!UICONTROL Contas].

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <td> <p>Standard</p>
   <p>Plano</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Para enviar uma solicitação [!DNL Workfront] de uma [!DNL Salesforce] [!UICONTROL Oportunidade] ou Conta
verifique se você tem o seguinte no seu ambiente:

* O administrador do [!DNL Workfront] instalou o [!DNL Workfront for Salesforce].\
   Para obter mais informações sobre como instalar o [!DNL Workfront for Salesforce], consulte [Instalar [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* O administrador [!DNL Workfront] adicionou a seção [!DNL Workfront] à sua [!UICONTROL Oportunidade] e à Conta
layouts de página.\
   Para obter mais informações sobre como adicionar a seção [!DNL Workfront] a um layout de página, consulte [Configurar a [!DNL Adobe Workfront] seção para [!DNL Salesforce] usuários](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Você tem uma conta [!DNL Workfront] e pode fazer logon nela a partir da seção [!DNL Workfront] dentro da sua [!UICONTROL Oportunidade] ou Conta
.

## Configurando a criação de [!DNL Workfront] projetos a partir de [!DNL Salesforce]

* [Noções básicas sobre a criação automática de projetos](#understanding-the-automatic-creation-of-projects-understanding-the-automatic-creation-of-projects)
* [Configurar acionadores](#configuring-triggers-configuring-triggers)
* [Noções básicas sobre nomes de projeto](#understanding-project-names-understanding-project-names)

### Noções básicas sobre a criação automática de projetos {#understanding-the-automatic-creation-of-projects}

Como administrador do sistema [!DNL Salesforce], você pode definir acionadores que podem criar projetos automaticamente em [!DNL Workfront] quando as seguintes situações ocorrerem em [!DNL Salesforce]:

* O [!UICONTROL Estágio] de uma [!UICONTROL Oportunidade] foi atualizado.
* O [!UICONTROL Tipo] de uma Conta
foi atualizado.

Os acionadores só podem ser configurados após a instalação de [!DNL Workfront for Salesforce].  \
Para obter informações sobre como instalar o [!DNL Workfront for Salesforce], consulte [Instalar [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Considere o seguinte ao configurar acionadores para criar automaticamente [!DNL Workfront] projetos quando [!DNL Salesforce] itens forem criados ou atualizados:

* Você precisa ser um [!DNL Salesforce] e um administrador do sistema [!DNL Workfront] para configurar os acionadores.
* Após configurar os acionadores, qualquer pessoa que atualize o [!UICONTROL Estágio] de uma [!UICONTROL Oportunidade] ou o [!UICONTROL Tipo] de uma Conta
O pode acionar a criação de um projeto [!DNL Workfront]. Isso inclui [!DNL Salesforce] usuários que não têm uma conta [!DNL Workfront].
* Não há limite para o número de acionadores que você pode ter.
* Não é possível criar vários acionadores com base nas mesmas condições. Os acionadores são exclusivos por padrão.
* Depois que o projeto é criado, ele é vinculado automaticamente à oportunidade ou à conta em que foi gerado. Depois de estabelecido, esse link não pode ser interrompido.
* Uma oportunidade ou conta pode ser vinculada a vários projetos em [!DNL Workfront] quando uma condição acionada tiver sido atendida várias vezes na vida da oportunidade ou da conta.

  Por exemplo, se você definir mais de um [!UICONTROL Estágio] para uma [!UICONTROL Oportunidade] para acionar um Projeto, será criado um projeto para cada estágio definido que a oportunidade alcançar, durante a vida dessa oportunidade. Além disso, se você atualizar o [!UICONTROL Estágio] de uma [!UICONTROL Oportunidade] de um estágio definido para outro e depois atualizá-lo de volta para o estágio definido, um segundo projeto será criado pela segunda vez que você atualizar o campo [!UICONTROL Estágio] para o mesmo estágio definido.

* Um projeto em [!DNL Workfront] pode ser vinculado apenas a uma oportunidade ou a uma conta em [!DNL Salesforce] em um determinado momento, mas não a ambos ao mesmo tempo.

### Configurar acionadores {#configuring-triggers}

Depois de configurar os acionadores, o processo de criação de projetos [!DNL Workfront] será habilitado para as estruturas do [!UICONTROL Salesforce Classic] ou [!DNL Lightning Experience].

Para configurar acionadores em [!UICONTROL Salesforce]:

1. Faça logon em [!DNL Salesforce] como administrador do sistema.
1. (Condicional) Em [!DNL Salesforce Classic], clique em **[!UICONTROL Configuração]** e, na seção **[!UICONTROL Compilação]**, expanda **[!UICONTROL Raio]**.

   Ou

   Na Experiência do Lightning [!DNL Salesforce], clique no ícone **[!UICONTROL Instalação]**, depois em **[!UICONTROL Instalação]** e, em **[!UICONTROL FERRAMENTAS DA PLATAFORMA]**, expanda **[!UICONTROL Aplicativos]**.

1. Clique em **[!UICONTROL Pacotes Instalados]**.

   Observe que o pacote **[!DNL Workfront]** foi instalado.

1. Clique em **[!UICONTROL Configurar]** ao lado de **[!DNL Workfront]**.

1. Faça logon em [!DNL Workfront] como administrador do sistema.

   A página **[!UICONTROL Triggers]** é exibida.

   ![salesforce_triggers_page_empty.png](assets/salesforce-triggers-page-empty-350x134.png)

1. Clique em **[!UICONTROL Novo Gatilho]**.
1. No menu suspenso **[!UICONTROL [!DNL Salesforce]Objeto]**, selecione **[!UICONTROL Oportunidade]**.

   Este campo é obrigatório.

1. (Condicional) Especifique o seguinte:

   1. No menu suspenso **[!UICONTROL Estágio]**, selecione um **[!UICONTROL Estágio]**.\

      Quando uma oportunidade atinge o [!UICONTROL Estágio] especificado aqui, um projeto é criado em [!DNL Workfront]. Este campo é obrigatório.

   1. No campo **[!UICONTROL Portfolio ou Programa]**, comece digitando o nome de um Portfolio ou Programa no qual deseja que o projeto seja colocado em [!DNL Workfront], em seguida, selecione-o quando ele aparecer na lista.\

      Se você não especificar um Portfolio ou um Programa, o novo projeto será criado e adicionado à lista [!UICONTROL Projetos que possuo] do usuário que fez logon em [!DNL Workfront] ao configurar os acionadores. Esse usuário também é o Proprietário do novo projeto.

   1. Comece digitando o nome de um Modelo que você deseja associar ao novo projeto [!DNL Workfront] e selecione-o quando ele aparecer na lista.\

      Este campo é obrigatório.


      >[!NOTE]
      >
      >Se você tiver especificado um Proprietário do modelo no modelo que planeja usar para essa integração, ele se tornará o Proprietário do novo projeto. Os novos projetos aparecem na lista [!UICONTROL Projetos dos quais sou proprietário] do usuário proprietário do novo projeto, de acordo com o modelo.

   1. (Opcional) Selecione o campo **[!UICONTROL Criar um novo projeto para cada tipo de produto vendido]** se desejar criar um novo projeto para cada tipo de produto vendido em qualquer oportunidade.
   1. (Condicional) Selecione um **[!UICONTROL Produto]** no menu suspenso **[!UICONTROL Produto]**.

      Este campo é obrigatório.

   1. (Condicional) Comece digitando o nome de um **[!UICONTROL Modelo]** que você deseja associar ao novo projeto [!DNL Workfront] se o Produto especificado estiver na [!UICONTROL Oportunidade]. Selecione-o quando ele aparecer na lista.

      Este campo é obrigatório.

      O projeto criado quando um novo produto é adicionado à oportunidade [!DNL Salesforce] é colocado na mesma Portfolio ou Programa selecionado para a oportunidade.

      >[!IMPORTANT]
      >
      >O projeto é criado somente quando o Estágio é atualizado na [!UICONTROL Oportunidade]. Um projeto exclusivo é criado para cada produto especificado quando o campo Preparo é atualizado, e não conforme os produtos são adicionados a [!UICONTROL Oportunidades].

1. (Opcional) Clique em **[!UICONTROL Novo Acionador]**.
1. (Opcional) No menu suspenso **[!UICONTROL [!DNL Salesforce]Objeto]**, selecione **Conta
**.

   Este campo é obrigatório.
1. (Condicional) Especifique o seguinte:

   1. Selecione um **[!UICONTROL Tipo]** no menu suspenso **[!UICONTROL Tipo]**.

      Quando qualquer **Conta
** é designado como o **[!UICONTROL Tipo]** especificado aqui em [!DNL Salesforce], um **[!UICONTROL Projeto]** é criado em [!DNL Workfront].

      Este campo é obrigatório.

   1. (Opcional) Comece digitando o nome de um **[!UICONTROL Portfolio]** ou **[!UICONTROL Programa]** onde deseja colocar o projeto em [!DNL Workfront] no campo **[!UICONTROL Portfolio ou Programa]** e selecione-o quando ele aparecer na lista.

      Se você não especificar um Portfolio ou um Programa, o novo projeto será criado e adicionado à lista **[!UICONTROL Projetos que possuo]** do usuário que fez logon em [!DNL Workfront] pelo [!DNL Salesforce]. O usuário também é o Proprietário do novo projeto.

   1. Comece digitando o nome de um **[!UICONTROL Modelo]** que você deseja associar ao novo projeto [!DNL Workfront] e selecione-o quando ele aparecer na lista.

      Este campo é obrigatório.

      >[!NOTE]
      >
      >Se você tiver especificado um Proprietário do modelo no modelo que planeja usar para essa integração, ele se tornará o Proprietário do novo projeto. Os novos projetos aparecem na lista **[!UICONTROL Projetos dos quais sou proprietário]** do usuário proprietário do novo projeto, de acordo com o modelo.

   ![salesforce_triggers_page_with_clean_up_template_names.png](assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png)

1. Clique em **[!UICONTROL Salvar]**.

   [!DNL Workfront] projetos agora são gerados sempre que qualquer um dos acionadores é atendido.

### Noções básicas sobre nomes de projeto {#understanding-project-names}

Dependendo do acionador que gerou os projetos, os nomes dos projetos em [!DNL Workfront] podem seguir um destes padrões:

* Se o projeto for criado com base em uma oportunidade ou em um gatilho de conta, o nome do projeto será: *`<Salesforce object name>`: `<Project template name>` (via [!DNL Salesforce])*.
* Se o projeto for criado com base em um acionador de oportunidade que também inclua a adição de um novo Produto, o nome do projeto será: *`<Salesforce object name>`: `<Salesforce product name>` (via [!DNL Salesforce])*.

## Visualizar [!DNL Workfront] projetos

Se o administrador [!DNL Workfront] adicionou a seção [!DNL Workfront] à sua [!UICONTROL Oportunidade] ou Conta
layout de página, você pode ver os projetos criados automaticamente na guia [!UICONTROL Projetos] desta seção.\
Para obter mais informações sobre como adicionar a seção [!DNL Workfront] ao layout da página de uma [!UICONTROL Oportunidade] ou Conta
, consulte [Configurar a [!DNL Adobe Workfront] seção para [!DNL Salesforce] usuários](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

Você deve ter uma conta [!DNL Workfront] e estar conectado ao [!DNL Workfront] para exibir a guia [!UICONTROL Projetos].

Para exibir projetos criados a partir de uma [!UICONTROL Oportunidade] ou Conta
:

1. Ir para uma [!UICONTROL Oportunidade] ou Conta
.
1. Vá para a seção **[!DNL Workfront]**.

   >[!NOTE]
   >
   >Dependendo de como o administrador do [!DNL Workfront] configurou esta seção, ela pode ter um nome diferente.

1. Selecione a guia **[!UICONTROL Projetos]**.

   Todos os projetos criados por acionadores definidos são listados nesta guia. Qualquer usuário em [!DNL Salesforce] que também tenha uma conta [!DNL Workfront] e que possa ter permissões para ver esses projetos em [!DNL Workfront] também pode vê-los em [!DNL Salesforce] para a [!UICONTROL Oportunidade] ou a Conta
que os gerou.

   Você pode exibir as seguintes informações sobre os projetos criados pela integração:

   * Nome do Projeto
   * Número de referência
   * Data de Entrada
   * Nome do proprietário
   * Status
   * Condição
   * Data de conclusão planejada
   * Percentual concluído

     Quando essas informações forem atualizadas em [!DNL Workfront], você poderá ver os campos atualizados nessa lista.

1. (Opcional) Clique no nome de um projeto para abri-lo no Workfront.
1. (Opcional) Clique em [!UICONTROL **[!UICONTROL Ir para Salesforce]**] na área [!UICONTROL Detalhes do Projeto] ou no cabeçalho do projeto para acessar a [!UICONTROL Oportunidade] ou a Conta
onde o projeto se originou. O administrador do sistema ou do grupo deve adicionar o campo [!UICONTROL Integrações] ao modelo de layout para encontrá-lo no cabeçalho do projeto.

   >[!NOTE]
   >
   >O link [!UICONTROL Ir para o Salesforce] está visível para todos os usuários [!DNL Workfront] que podem ver o projeto. Você deve ter uma conta [!DNL Salesforce] para poder acessar a Oportunidade [!DNL Salesforce] ou a Conta de onde o projeto foi gerado.
