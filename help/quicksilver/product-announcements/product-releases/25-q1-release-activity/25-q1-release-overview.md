---
title: Visão geral da versão do primeiro trimestre de 2025
description: Esta página fornece informações sobre as funcionalidades incluídas na versão do primeiro trimestre de 2025. Essas melhorias estão previstas para serem disponibilizadas no ambiente de produção ao longo do trimestre.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5bb898fa-d74e-4174-bc93-d8ffb8937680
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '2786'
ht-degree: 13%

---

# Visão geral da versão do primeiro trimestre de 2025

Esta página fornece informações sobre as funcionalidades incluídas na versão do primeiro trimestre de 2025. Essas melhorias estão previstas para serem disponibilizadas no ambiente de produção ao longo do trimestre.

<span class="preview">Os recursos fora do ciclo (aqueles que são lançados na produção antes da data de lançamento do primeiro trimestre de 2025) estão destacados em amarelo.</span>

>[!IMPORTANT]
>
>A versão 23.3 incluía a opção de mover sua organização para versões mensais. Portanto, a Workfront alterou o esquema de numeração de versões para contabilizar as faixas de lançamento mensais e trimestrais. O primeiro número designa o ano e o segundo número significa o mês do lançamento. Exemplo: a versão de abril de 2025 é 25.4.
>
>As versões mensais e trimestrais estão previstas para serem disponibilizadas na quinta-feira da segunda semana completa do mês, salvo indicação em contrário.
>
>| Versão mensal | Versão trimestral |
>|----|----|
>| <ul><li>24.11 (14 de novembro de 2024)</li><li>24.12 (12 de dezembro de 2024)</li><li>25.1 (15 de janeiro de 2025)</li></ul> | <ul><li>25.1 (16 de janeiro de 2025)</li></ul> |
>
>Observe que, para a versão final de cada trimestre (25.1 deste trimestre), os usuários que estiverem no cronograma de lançamento rápido receberão a versão um dia antes.
>
>Para obter mais informações sobre o processo de lançamento rápido, consulte [Habilitar ou desabilitar o processo de lançamento rápido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Aprimoramentos do Adobe Workfront

* [Aprimoramentos do administrador](#administrator-enhancements)
* [Melhorias nas placas](#boards-enhancements)
* [Aprimoramentos no gerenciamento de documentos](#document-management-enhancements)
* [Aprimoramentos de prioridades](#priorities-enhancements)
* [Aprimoramentos de projeto](#project-enhancements)
* [Aprimoramentos de provas](#proofing-enhancements)
* [Aprimoramentos de Relatório e Painel de Controle](#report-and-dashboard-enhancements)
* [Atualizar aprimoramentos de fluxo](#update-stream-enhancements)
* [Outros aprimoramentos](#other-enhancements)

### Aprimoramentos do administrador

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Recurso</span></p>
        </td>
        <td>
            <p><span class="bold">Datas de lançamento</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
           Regras de negócios agora são aceitas para mais objetos</a></p>
           [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Agora, você pode criar regras de negócios e aplicar a validação a esses objetos adicionais: Empresa, Iteração, Categoria de Recurso Não Mão-de-Obra, Função do Cargo, Usuário, Atribuição, Pool de Recursos, Folga, Documento e Hora.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: quarta-feira, 16 de janeiro de 2024</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
           Comparar objetos entre ambientes para promoção do ambiente</a></p>
           [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Para facilitar a determinação do objeto que deve ser incluído em um pacote de promoção de ambiente, adicionamos a capacidade de comparar objetos entre ambientes. Você pode então adicionar objetos a um pacote diretamente dessa comparação.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: 23 de outubro de 2025</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Mais objetos disponíveis para promoção de ambiente</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Para expandir os recursos da funcionalidade de promoção do ambiente, adicionamos mais objetos.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: 23 de outubro de 2025</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
        </td>
    </tr>  
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Impedir movimentação de tarefas quando há horas registradas</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Como a movimentação de tarefas ou problemas que registraram horas pode, às vezes, causar problemas de conformidade ou auditoria, adicionamos uma preferência na área Preferências de tarefas e problemas da Configuração que permite impedir que os usuários movam tarefas e problemas se houver horas registradas.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: sexta-feira, 19 de dezembro de 2024</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Preferência para usar projeto ou agendamento de usuário para tarefas de atribuição única</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Como administrador do sistema ou do grupo, agora você tem uma nova preferência para indicar se o Workfront deve usar a programação do projeto ou do usuário para calcular a linha do tempo do projeto quando você atribui um usuário a uma tarefa e o projeto e o usuário estão associados a uma programação.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: sexta-feira, 21 de novembro de 2024</li>
                <li>Produção para versão rápida: com a versão 24.12 (12 de dezembro de 2024)</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
        </td>
    </tr>     
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            As regras de negócios agora oferecem suporte a hiperlinks</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Agora é possível incluir hiperlinks na mensagem de erro personalizada de uma regra de negócios para orientar o usuário sobre como modificar sua ação dentro da restrição da regra. O URL estático pode ser vinculado à documentação ou a outras páginas que sejam úteis ao usuário.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: sexta-feira, 21 de novembro de 2024</li>
                <li>Produção para lançamento rápido: com o lançamento do 24.12 (12 de dezembro de 2024)</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
        </td>
    </tr>    
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            A filtragem em campos de digitação antecipada nativos agora está disponível</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Quando você adiciona uma referência de campo nativo a um formulário personalizado e ela faz referência a um campo de digitação antecipada (como Portfolio, Empresa ou Proprietário), uma opção de filtro está disponível. O filtro permite limitar os objetos que os usuários podem escolher quando estiverem usando o campo. Esse filtro personalizado funciona da mesma forma que um filtro em um campo de preenchimento personalizado, usando o Modo de texto para definir o filtro.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: sexta-feira, 21 de novembro de 2024</li>
                <li>Produção para versão rápida: com a versão 24.12 (12 de dezembro de 2024)</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Ícone "Mover para" adicionado a campos personalizados</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Quando um formulário personalizado contém várias seções com muitos campos, pode ser difícil mover um campo de uma seção para outra arrastando e soltando. Um ícone "mover para" foi adicionado a cada campo, permitindo selecionar a seção em que o campo é colocado.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: quarta-feira, 29 de outubro de 2024</li>
                <li>Produção para lançamento rápido: com o lançamento do 24.11 (14 de novembro de 2024)</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### Melhorias nas placas

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Recurso</span></p>
        </td>
        <td>
            <p><span class="bold">Datas de lançamento</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Alterar o proprietário de um quadro</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Por padrão, o criador de um quadro é o proprietário. O proprietário do painel é a única pessoa que pode excluir esse painel ou atualizar seus filtros no painel Configurar.</p>
            <p>Foi adicionada uma funcionalidade que permite aos administradores de sistema da Workfront alterar o proprietário de uma placa. O proprietário atual de um painel também pode alterar o proprietário desse painel específico. Essa funcionalidade está disponível nos quadros básico, retrospectivo e Kanban, mas não nos dinâmicos.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: quinta-feira, 18 de dezembro de 2024</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### Aprimoramentos no gerenciamento de documentos

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Recurso</span></p>
        </td>
        <td>
            <p><span class="bold">Datas de lançamento</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Editar vários documentos de uma só vez</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Agora é possível editar vários documentos de uma só vez. É possível editar as descrições e atualizar formulários personalizados.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: sexta-feira, 21 de novembro de 2024</li>
                <li>Produção para lançamento rápido: com o lançamento do 24.12 (12 de dezembro de 2024)</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
        </td>
    </tr>    
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Novo status Retirado disponível para aprovações de versão de documento</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Quando uma nova versão for adicionada a um documento com aprovações pendentes, a aprovação da versão anterior será exibida como "Retirado", indicando que o processo de aprovação anterior foi fechado devido à adição da nova versão.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: sexta-feira, 7 de novembro de 2024</li>
                <li>Produção para lançamento rápido: com o lançamento do 24.11 (14 de novembro de 2024)</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
            <p><i>Esse recurso faz parte de uma versão em fases e está disponível somente para clientes específicos.</i></p>
        </td>
    </tr>
</tbody>
</table>

### Aprimoramentos de prioridades

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Recurso</span></p>
        </td>
        <td>
            <p><span class="bold">Datas de lançamento</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Use filtros inteligentes para localizar seu trabalho em Prioridades</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Use linguagem natural para filtrar rapidamente o trabalho na lista de trabalho Prioridades. Você pode digitar coisas como </p>
            <ul>
                <li>Mostrar tarefas atrasadas</li>
                <li>Mostrar tarefas com vencimento nesta semana</li>
                <li>Mostrar as principais prioridades</li>
            </ul>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: sexta-feira, 9 de janeiro de 2025</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Recuperar o trabalho em Prioridades</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Você pode usar Capch me up para ajudar a reduzir a quantidade de tempo procurando informações sobre projetos ativos.</p>
            <p>Desenvolvido pelo Assistente de IA da Workfront, o recurso Catch me resume atualizações, documentos carregados e outras alterações importantes sobre seus projetos nos seguintes intervalos de tempo: 24 horas, 3 dias ou 7 dias.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: sábado, 20 de dezembro de 2024</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Veja as alterações em tempo real na página Detalhes em Prioridades</a></p>
            <p>Agora você pode exibir atualizações em tempo real na página Detalhes de uma tarefa ou ocorrência. Você também pode ver se outras pessoas estão visualizando a página ao mesmo tempo que você com indicadores de presença em tempo real.</p>
        </td>
        [!BADGE Na produção &#x200B;]{type=Informative}
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: sexta-feira, 19 de dezembro de 2024</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Fazer upload e exibir documentos e provas em Prioridades</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Agora você pode interagir com documentos e provas para tarefas e problemas na lista de trabalho e no calendário. Na nova guia Documentos, é possível</p>
            <ul>
                <li>Fazer upload de um documento</li>
                <li>Criar uma prova</li>
                <li>Iniciar o visualizador de provas</li>
                <li>E muito mais</li>
            </ul>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: sexta-feira, 19 de dezembro de 2024</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            A exibição Calendário agora está disponível em Prioridades</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Você pode acompanhar seu trabalho com um calendário mensal visual e claro. Com o calendário Prioridades, você pode</p>
            <ul>
                <li>Use filtros para encontrar seu trabalho</li>
                <li>Aplique campos personalizados como status e nível de foco para identificar trabalhos de alta prioridade</li>
                <li>Aplicar cores para organização rápida</li>
                <li>E muito mais</li>
            </ul>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: sexta-feira, 19 de dezembro de 2024</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Atualizações na lista de trabalho de prioridades</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Atualizamos a lista de trabalho de Prioridades para melhorar os recursos e alinhar com outras áreas do aplicativo.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: sexta-feira, 12 de dezembro de 2024</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Acesse a página Detalhes de um projeto em Prioridades</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Agora você pode navegar diretamente para um projeto no Workfront a partir da lista de trabalho Prioridades.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: sexta-feira, 5 de dezembro de 2024</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Opções atualizadas na coluna Meu foco em Prioridades</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Atualizamos as opções na coluna Meu foco para ajudá-lo a priorizar e classificar seu trabalho de uma maneira mais intuitiva. Os novos rótulos incluem</p>
            <ul>
                <li>Urgente</li>
                <li>Alta</li>
                <li>Normal</li>
                <li>Baixa</li>
            </ul>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: sexta-feira, 14 de novembro de 2024</li>
                <li><span class="preview">Versão de produção para todos os clientes: 14 de novembro de 2024</span></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Exibir detalhes do projeto em Prioridades</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Agora você pode ver os detalhes e comentários do projeto na lista de trabalho em Prioridades.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: quinta-feira, 6 de novembro de 2024</li>
                <li>Produção para lançamento rápido: com o lançamento do 24.11 (14 de novembro de 2024)</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### Aprimoramentos de projeto

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Recurso</span></p>
        </td>
        <td>
            <p><span class="bold">Datas de lançamento</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-project-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Atribuições mais relevantes removidas de Visualização e Produção para ambientes de Lançamento Rápido</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Uma funcionalidade que está no ambiente de Pré-visualização desde dezembro de 2023 e no ambiente de Produção de lançamento rápido desde março de 2024 foi removida. Os recursos adicionaram sugestões de atribuição inteligente mais relevantes ao atribuir tarefas.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: sexta-feira, 19 de dezembro de 2024</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### Aprimoramentos de provas

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
<tr>
        <td>
            <p><span class="bold">Recurso</span></p>
        </td>
        <td>
            <p><span class="bold">Datas de lançamento</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Atualização do Visualizador de provas de desktop</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Atualizamos o Desktop Viewer com a versão mais recente do Eletron 33.3.0 que usa Chromium 130.0.6723.152. </p>
            <p>Versão mais recente: 2.1.44 </p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: quarta-feira, 2 de janeiro de 2024</li>
                <li><span class="preview">Versão de produção para todos os clientes: 9 de janeiro de 2025</span></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><span class="bold">Recurso</span></p>
        </td>
        <td>
            <p><span class="bold">Datas de lançamento</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Nova extensão do navegador para revisão interativa disponível em beta</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Estamos introduzindo uma nova extensão de navegador, a ferramenta de revisão do Adobe Workfront, para substituir a extensão de navegador herdada para revisão de conteúdo ZIP interativo. A nova ferramenta de revisão do Adobe Workfront é compatível com a revisão de conteúdo ZIP em todos os navegadores comuns.</p>
            <p>A extensão do navegador herdado será removida em 28 de fevereiro de 2025.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: sexta-feira, 7 de novembro de 2024</li>
                <li><span class="preview">Versão de produção para todos os clientes: 7 de novembro de 2024</span></li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### Aprimoramentos de Relatório e Painel de Controle

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Recurso</span></p>
        </td>
        <td>
            <p><span class="bold">Datas de lançamento</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Novas entidades disponíveis na Conexão de dados</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Adicionamos suporte para várias novas entidades no Data Connect, incluindo algumas entidades específicas de agência.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: quinta-feira, 15 de janeiro de 2025</li>
                <li>Versão de produção para todos os clientes: 15 de janeiro de 2025</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Limite de 25 relatórios, páginas externas ou calendários nos painéis</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Para manter o desempenho do painel, implementamos um limite para o número total de relatórios, páginas externas ou calendários que podem ser colocados em um painel. Ao criar um novo painel, um máximo de 25 itens podem ser adicionados.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: terça-feira, 16 de dezembro de 2024</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Botão de criação de conta do leitor de primeira vez para Conexão de dados</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Os administradores que acessam o Data Connect pela primeira vez agora recebem a opção de criar uma nova conta do leitor de Snowflake clicando em um único botão. O processo leva alguns minutos para ser concluído, mas não requer nenhuma ação adicional.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: sexta-feira, 14 de novembro de 2024</li>
                <li><span class="preview">Versão de produção para todos os clientes: 14 de novembro de 2024</span></li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### Atualizar aprimoramentos de fluxo

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Recurso</span></p>
        </td>
        <td>
            <p><span class="bold">Datas de lançamento</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Experiência de comentário atualizada no widget Menções na área Página inicial e Minhas atualizações</a></p>
            <p>Estamos atualizando a experiência de comentários no widget Menções na Página inicial e na seção Menções na área Minhas atualizações. Agora, a mesma experiência na área Atualizações da maioria dos objetos do Workfront também está disponível no widget Menções e na seção Menções de Minhas atualizações.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: sexta-feira, 19 de dezembro de 2024</li>
                <li>Versão de produção para todos os clientes da Página inicial: a ser anunciada</li>
                <li>Versão de produção para todos os clientes de Minhas atualizações: 19 de junho de 2025</li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### Outros aprimoramentos

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Atualização sobre como os ativos movidos ou excluídos em pastas vinculadas são gerenciados</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Alteramos a maneira como os ativos movidos e excluídos são tratados ao usar a integração do Adobe Workfront com o Experience Manager Assets e o Assets Essentials:</p>
            <ul>
                <li>Ativos excluídos: quando um ativo é excluído dentro de uma pasta vinculada no Assets ou no Assets Essentials, o ativo excluído é retido na área Documentos do projeto.</li>
                <li>Ativos movidos: quando um ativo é movido para fora de uma pasta vinculada no Assets ou no Assets Essentials, o ativo movido é retido na área Documentos do projeto.</li>
            </ul>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: sexta-feira, 21 de novembro de 2024</li>
                <li><span class="preview">Versão de produção para todos os clientes: 5 de dezembro de 2024</span></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            As seções em um formulário personalizado agora podem ser recolhidas e expandidas</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Quando um formulário personalizado com várias seções é anexado a um objeto, agora é possível recolher e expandir todas as seções, exceto a seção padrão na parte superior do formulário. O administrador também pode visualizar essa funcionalidade ao visualizar o formulário no designer do formulário.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: terça-feira, 11 de novembro de 2024</li>
                <li>Produção para lançamento rápido: com o lançamento do 24.12 (12 de dezembro de 2024)</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            O Assistente de IA agora pode trabalhar com projetos, tarefas e problemas</a></p>
            [!BADGE Na produção &#x200B;]{type=Informative}
            <p>Para facilitar o gerenciamento de itens de trabalho no Workfront, atualizamos o Assistente de IA para trabalhar com projetos, tarefas e problemas. Agora, o AI Assistant pode localizar projetos, tarefas e problemas com base nos critérios especificados.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão preliminar: sexta-feira, 31 de outubro de 2024</li>
                <li>Produção para lançamento rápido: com o lançamento do 24.11 (14 de novembro de 2024)</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">
            Atualizações da aparência durante o primeiro trimestre de 2025</a></p>
            <p>Pequenas atualizações na aparência de várias áreas do aplicativo Adobe Workfront estão sendo feitas no primeiro trimestre de 2025. Revise as notas de versão individuais para datas de lançamento específicas.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão de pré-visualização: durante todo o período da versão do Primeiro trimestre de 2025</li>
                <li><span class="preview">Versão de produção: revise as notas de versão para datas específicas</span></li>
            </ul>
        </td>
    </tr>                            
</tbody>
</table>

<!--
### Functionality soon to be removed from Workfront

The following functionality is soon to be removed from Workfront:
-->

## Anúncios

### Aprimoramentos do Workfront Fusion

>[!IMPORTANT]
>
>A documentação do Workfront Fusion foi movida para um novo local. Para obter informações, instruções e versões do Fusion, visite a [documentação do Workfront Fusion](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/home).
>
>Cada artigo de documentação atual do Fusion contém um link para o artigo correspondente no novo local. Atualize seus marcadores.
>
>O conjunto atual de documentação do Fusion não está mais sendo atualizado e será removido em breve.

Novos recursos no Workfront Fusion estão disponíveis na produção em uma cadência fora da programação de lançamento do Primeiro trimestre de 2025. Para obter mais informações sobre os recursos mais recentes, consulte [Atividade de lançamento do Adobe Workfront Fusion](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Aprimoramentos do Workfront Planning

Novos recursos no Workfront Planning estão disponíveis em Produção. Para obter mais informações sobre os recursos mais recentes, consulte a [atividade da versão do Adobe Workfront Planning First Quarter 2025](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q1.md).

### Aprimoramentos no Planejador de cenários do Workfront

Não há atualizações do Planejador de cenários neste momento na versão. Esta área será atualizada quando houver atualizações disponíveis.

### Aprimoramentos do Workfront Proof

Não há atualizações do Workfront Proof neste momento na versão. Esta área será atualizada quando houver atualizações disponíveis.

### Aprimoramentos das metas do Workfront

Não há atualizações do Workfront Goals neste momento na versão. Esta área será atualizada quando houver atualizações disponíveis.

### API versão 19

Para a versão 19 da API, modificamos alguns recursos e pontos de acesso. Algumas das alterações oferecem suporte a novas funcionalidades, enquanto outras facilitam o uso das informações disponíveis por meio da API.

Para obter informações sobre as novidades e atualizações, consulte [Novidades na versão 19 da API](/help/quicksilver/wf-api/api/new-api-version-19.md).

Para obter informações sobre as versões da API, consulte [controle de versão da API e cronograma de suporte](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Atualizações de manutenção do Workfront

Para obter informações sobre as atualizações de manutenção feitas durante a versão do primeiro trimestre de 2025, consulte [Atualizações de manutenção do Workfront](https://experienceleague.adobe.com/pt-br/docs/workfront-known-issues/releases/current-updates).

### Atualizações de treinamento

Explore as últimas atualizações feitas nos programas de aprendizagem, caminhos de aprendizagem, vídeos e guias para cada versão do Adobe Workfront. Para obter mais informações, consulte a seção &quot;Novidades&quot; da [página de tutoriais do Workfront](https://experienceleague.adobe.com/pt-br/docs/workfront-learn/tutorials-workfront/home?lang=pt-BR).
