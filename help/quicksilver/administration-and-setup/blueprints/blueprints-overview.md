---
user-type: administrator
content-type: overview
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Visão geral de blueprints
description: Os blueprints fornecem blocos de construção básicos para ajudá-lo a criar um sistema de gerenciamento de trabalho que cresce com você.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c487598-2066-4507-8dfe-1a54d38f5eea
source-git-commit: af869fc8f57458f0f006ab86d6c19fe07f3eb81b
workflow-type: tm+mt
source-wordcount: '816'
ht-degree: 0%

---

# Visão geral de blueprints

Blueprints são conjuntos de objetos do Workfront que abordam casos de uso comuns no Workfront. Você pode baixar e instalar um blueprint e, em seguida, configurar os objetos para seu caso de uso específico.

>[!INFO]
>
>Exemplos:
>
>* **Configuração da Organização de Recursos Humanos**
>
>   Este blueprint contém a configuração de estruturas organizacionais para expandir para um departamento de Recursos Humanos.
>
>* **Adicionar a lista de verificação de TI para novos funcionários**
>
>   Este blueprint contém um modelo para organizar novas atividades de integração de funcionários. A utilização desse modelo permite que as equipes de TI operem com eficiência, resultando em uma nova experiência de funcionário positiva e em um caminho mais rápido para a produtividade.
>
>* **Lista de verificação de noções básicas de instância herdada**
>
>    Este blueprint contém um modelo de projeto (ou lista de verificação) que pode ser revisado com uma pequena lista de perguntas, recursos e links para compreender claramente como a instância do Workfront foi configurada. Use-a quando tiver herdado recentemente uma instância do Workfront e precisar de orientação sobre onde começar.
>
>Para revisar os blueprints atuais, consulte [Lista de blueprints disponíveis](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md).


Os blueprints fornecem blocos de construção básicos para ajudá-lo a criar um sistema de gerenciamento de trabalho que cresce com você. Os administradores do sistema podem navegar pelo catálogo de blueprints e instalar modelos de projeto, painéis e estruturas organizacionais prontos para uso. Outros usuários podem navegar no catálogo e solicitar a instalação de um blueprint. Para obter mais informações, consulte [Navegar pelo catálogo de blueprints e solicitar a instalação de blueprints](../../administration-and-setup/blueprints/browse-catalog.md).

Cada blueprint destina-se a um departamento e a um nível de maturidade específico para ajudá-lo a implementar práticas recomendadas comprovadas em seu sistema com mais rapidez. Os níveis de maturidade detalhados abaixo são indicados no cartão de catálogo do blueprint e nos detalhes.

**[!UICONTROL Gerenciado]:** Os modelos de projeto gerenciados ajudam a apoiar a adoção de um novo processo de negócios antes que as atividades e os resultados sejam totalmente aceitos como um procedimento padrão. Eles contêm tarefas para garantir que cada etapa do novo processo seja seguida.

**[!UICONTROL Integrado]:** Os modelos de projeto integrados presumem que as funções empresariais sejam compatíveis por meio de um procedimento operacional padrão. Os colaboradores do processo conhecem as etapas e as tarefas necessárias para acompanhar o processo. Os modelos de projeto para dar suporte a esse processo contêm menos tarefas para rastrear apenas marcos e outros materiais de entrega importantes necessários para fins de relatório.

## Encontrar o blueprint correto

Você pode consultar blueprints por caso de uso, nível de maturidade, status de instalação e tipo com os filtros no lado direito do catálogo. Depois de encontrar um blueprint que lhe interessa, você pode visualizar os detalhes na página de detalhes.

### Tipos de blueprint

O tipo de blueprint mostra o que está incluído no blueprint. O tipo está listado na parte inferior do cartão de blueprint no catálogo. Observe que um blueprint pode ter mais de um tipo.

Os seguintes tipos de blueprints estão disponíveis:

* Modelos de projeto: inclui objetos padrão associados a um modelo de projeto (tarefas, problemas, funções e equipes) e algumas preferências relacionadas a esses objetos. Para obter mais informações, consulte [Configurar um blueprint](../../administration-and-setup/blueprints/configure-template-package.md).
* Estruturas organizacionais: inclui objetos associados à estrutura de uma organização (empresas, grupos, funções e equipes). Para obter mais informações, consulte [Configurar um blueprint](../../administration-and-setup/blueprints/configure-template-package.md).
* Painéis: inclui um ou mais painéis para um caso de uso específico, como serviços de implementação.
<!--
* Request queues: Includes one or more projects configured as request queues.
* Custom forms: Includes custom forms attached to another object type, such as a project or portfolio.
* Setup features: Includes one or more elements that are configured in the Setup area of Workfront, such as layout templates.
-->

Para revisar os blueprints atuais, consulte [Lista de blueprints disponíveis](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md).

### Exibir detalhes de 

Cada blueprint contém uma página de detalhes. Nessa página, é possível:

* Exibir um resumo do conteúdo do fluxo de trabalho
* Leia um breve resumo do blueprint
* Exibir histórico de instalação (clique em **[!UICONTROL Ver detalhes]** para ver a lista completa de objetos instalados com o blueprint)
* Consulte descrições de função, equipe, empresa e grupo
* Veja um exemplo visual do blueprint específico, como um modelo de projeto (você pode visualizar a imagem completa no navegador ou baixá-la)

![[!UICONTROL Detalhes do blueprint] página](assets/blueprint-details-page-2022.png)

## Instalar um blueprint

O administrador do sistema pode instalar diretamente no ambiente de produção ou em ambientes de sandbox. Para saber mais, consulte [Instalar um blueprint](../../administration-and-setup/blueprints/blueprints-install.md) ou [Configurar um blueprint](../../administration-and-setup/blueprints/configure-template-package.md).

Após a instalação, você pode não ter certeza sobre as melhores ações a serem executadas. Para obter informações, consulte [Ações a serem executadas após a instalação de um blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

## Observações adicionais sobre blueprints e modelos

Os blueprints não substituem a funcionalidade dos modelos de projeto no [!DNL Adobe Workfront]. Blueprints são uma maneira de criar novos modelos mais rapidamente para organizar mais do seu trabalho no [!DNL Workfront].

Não é possível copiar ou editar um blueprint. No entanto, após instalar a solução de um blueprint, você pode modificar o modelo do projeto, as funções de trabalho ou as equipes criadas a partir do blueprint da mesma forma que você normalmente atualiza esses registros no [!DNL Workfront] interface. Além disso, ao instalar um blueprint, o modelo é armazenado no [!UICONTROL Modelos] área de [!DNL Workfront] e o blueprint original permanece no [!UICONTROL Blueprints] área. Não é necessário fazer uma cópia do modelo antes de começar a personalizá-lo de acordo com as suas necessidades.

Os blueprints não removem nem substituem nada configurado em seu ambiente. Se você pretende substituir um modelo existente instalando um blueprint que cria um novo modelo, recomendamos desativar a versão anterior para evitar confusão entre os planejadores que criam projetos com base em modelos.
