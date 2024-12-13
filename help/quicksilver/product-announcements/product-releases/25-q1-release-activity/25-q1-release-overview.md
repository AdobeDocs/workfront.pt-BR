---
title: Visão geral da versão do primeiro trimestre de 2025
description: Esta página fornece informações sobre a funcionalidade incluída na versão do Primeiro trimestre de 2025. Essas melhorias estão planejadas para serem disponibilizadas no ambiente de produção durante todo o trimestre.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5bb898fa-d74e-4174-bc93-d8ffb8937680
source-git-commit: 8b0c40d6fa5898581c50d6257bc2b2f2a4838b06
workflow-type: tm+mt
source-wordcount: '1728'
ht-degree: 0%

---

# Visão geral da versão do primeiro trimestre de 2025

Esta página fornece informações sobre a funcionalidade incluída na versão do Primeiro trimestre de 2025. Essas melhorias estão planejadas para serem disponibilizadas no ambiente de produção durante todo o trimestre.

<span class="preview">Os recursos fora do ciclo (aqueles que foram lançados para produção antes da data de lançamento do Primeiro trimestre de 2025) estão destacados em amarelo.</span>

>[!IMPORTANT]
>
>A versão 23.3 incluía a opção de mover sua organização para versões mensais. Portanto, a Workfront alterou o esquema de numeração de versões para contabilizar as faixas de lançamento mensais e trimestrais. O primeiro número designa o ano e o segundo número significa o mês do lançamento. Exemplo: a versão de abril de 2025 é 25.4.
>
>Os lançamentos mensais e trimestrais devem estar disponíveis na quinta-feira da segunda semana completa do mês, a menos que especificado de outra forma.
>
>| Lançamento mensal | Versão trimestral |
>|----|----|
>| <ul><li>24.11 (14 de novembro de 2024)</li><li>24.12 (12 de dezembro de 2024)</li><li>25.1 (15 de janeiro de 2025)</li></ul> | <ul><li>25.1 (16 de janeiro de 2025)</li></ul> |
>
>Observe que, para a versão final de cada trimestre (25.1 neste trimestre), os usuários na programação de lançamento rápido receberão o lançamento um dia antes.
>
>Para obter mais informações sobre o processo de lançamento rápido, consulte [Habilitar ou desabilitar o processo de lançamento rápido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Aprimoramentos do Adobe Workfront

* [Aprimoramentos do administrador](#administrator-enhancements)<!--* [Boards enhancements](#boards-enhancements)-->
* [Aprimoramentos no gerenciamento de documentos](#document-management-enhancements)
* [Aprimoramentos na página inicial](#home-enhancements)
* [Aprimoramentos de provas](#proofing-enhancements)
* [Aprimoramentos de Relatório e Painel de Controle](#report-and-dashboard-enhancements)
* [Outras melhorias](#other-enhancements)

### Melhorias do administrador

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
            Preferência para usar projeto ou agendamento de usuário para tarefas de atribuição única</a></p>
            [!BADGE Na produção para a versão rápida ]{type=Positive}
            <p>Como administrador de sistema ou de grupo, agora você tem uma nova preferência para indicar se o Workfront deve usar o cronograma do projeto ou do usuário para calcular a linha do tempo do projeto ao atribuir um usuário a uma tarefa e se o projeto e o usuário estão associados a um cronograma.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão de pré-visualização: 21 de novembro de 2024</li>
                <li>Produção para lançamento rápido: com o lançamento do 24.12 (12 de dezembro de 2024)</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (janeiro de 2025)</li>
            </ul>
        </td>
    </tr>     
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Agora as regras de negócios oferecem suporte a hiperlinks</a></p>
            [!BADGE Na produção para a versão rápida ]{type=Positive}
            <p>Agora é possível incluir hiperlinks na mensagem de erro personalizada de uma regra de negócios para orientar o usuário sobre como modificar sua ação dentro da restrição da regra. O URL estático pode vincular à documentação ou outras páginas que seriam úteis para o usuário.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão de pré-visualização: 21 de novembro de 2024</li>
                <li>Produção para lançamento rápido: com o lançamento do 24.12 (12 de dezembro de 2024)</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (janeiro de 2025)</li>
            </ul>
        </td>
    </tr>    
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            A filtragem em campos de digitação antecipada nativos agora está disponível</a></p>
            <p>Quando você adiciona uma referência de campo nativo a um formulário personalizado e ela faz referência a um campo de digitação antecipada (como Portfolio, Empresa ou Proprietário), uma opção de filtro está disponível. O filtro permite limitar os objetos que os usuários podem escolher quando estão usando o campo. Esse filtro personalizado funciona da mesma forma que um filtro em um campo de digitação antecipada personalizado, usando o Modo de texto para definir o filtro.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão de pré-visualização: 21 de novembro de 2024</li>
                <li>Produção para lançamento rápido: com o lançamento do 24.12 (12 de dezembro de 2024)</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Ícone "Mover para" adicionado a campos personalizados</a></p>
            [!BADGE Na produção para a versão rápida ]{type=Positive}
            <p>Quando um formulário personalizado contém várias seções com muitos campos, pode ser difícil mover um campo de uma seção para outra arrastando e soltando. Um ícone "mover para" foi adicionado a cada campo, permitindo selecionar a seção em que o campo é colocado.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão de pré-visualização: 29 de outubro de 2024</li>
                <li>Produção para lançamento rápido: com o lançamento do 24.11 (14 de novembro de 2024)</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

<!--### Boards enhancements

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Feature</span></p>
        </td>
        <td>
            <p><span class="bold">Release dates</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Change the owner of a board</a></p>
            <p>The creator of a board is the owner by default. The board owner is the only person who can delete that board or update its filters in the Configure panel. Functionality has been added to allow Workfront system administrators to change the owner of a board. The current owner of a board can also change the owner of that specific board.</p>
        </td>
        <td>
            <p><b>Available on these dates:</b></p>
            <ul>
                <li>Preview release: October 31, 2024</li>
                <li>Production for fast release: With the 24.11 release (November 14, 2024)</li>
                <li>Production release for all customers: With the 25.1 release (January 2025)</li>
            </ul>
        </td>
    </tr>
</tbody>
</table>-->

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
            [!BADGE Na produção para a versão rápida ]{type=Positive}
            <p>Agora é possível editar vários documentos de uma só vez. É possível editar as descrições e atualizar formulários personalizados.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão de pré-visualização: 21 de novembro de 2024</li>
                <li>Produção para lançamento rápido: com o lançamento do 24.12 (12 de dezembro de 2024)</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (janeiro de 2025)</li>
            </ul>
        </td>
    </tr>    
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Novo status Retirado disponível para aprovações de versão de documento</a></p>
            [!BADGE Na produção para a versão rápida ]{type=Positive}
            <p>Quando uma nova versão for adicionada a um documento com aprovações pendentes, a aprovação da versão anterior será exibida como "Retirado", indicando que o processo de aprovação anterior foi fechado devido à adição da nova versão.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão de pré-visualização: 7 de novembro de 2024</li>
                <li>Produção para lançamento rápido: com o lançamento do 24.11 (14 de novembro de 2024)</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (janeiro de 2025)</li>
            </ul>
            <p><i>Esse recurso faz parte de uma versão em fases e está disponível somente para clientes específicos.</i></p>
        </td>
    </tr>
</tbody>
</table>

### Aprimoramentos na página inicial

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
            Atualizações na lista de trabalho de prioridades</a></p>
            [!BADGE New in Preview ]{type=Negative}
            <p>Atualizamos a lista de trabalho de Prioridades para melhorar os recursos e alinhar com outras áreas do aplicativo.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão de pré-visualização: 12 de dezembro de 2024</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Acesse a página Detalhes de um projeto em Prioridades</a></p>
            <p>Agora você pode navegar diretamente para um projeto no Workfront a partir da lista de trabalho Prioridades.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão de pré-visualização: 5 de dezembro de 2024</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Opções atualizadas na coluna Meu foco em Prioridades</a></p>
            [!BADGE Na produção ]{type=Informative}
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
                <li>Versão de pré-visualização: 14 de novembro de 2024</li>
                <li><span class="preview">Versão de produção para todos os clientes: 14 de novembro de 2024</span></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Exibir detalhes do projeto em Prioridades</a></p>
            [!BADGE Na produção para a versão rápida ]{type=Positive}
            <p>Agora é possível exibir detalhes e comentários do projeto na lista de trabalho em Prioridades.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão de pré-visualização: 6 de novembro de 2024</li>
                <li>Produção para lançamento rápido: com o lançamento do 24.11 (14 de novembro de 2024)</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

## Aprimoramentos de provas

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
            Nova extensão do navegador para revisão interativa disponível em beta</a></p>
            [!BADGE Na produção ]{type=Informative}
            <p>Estamos introduzindo uma nova extensão de navegador, a ferramenta de revisão do Adobe Workfront, para substituir a extensão de navegador herdada para revisão de conteúdo ZIP interativo. A nova ferramenta de revisão do Adobe Workfront é compatível com a revisão de conteúdo ZIP em todos os navegadores comuns.</p>
            <p>A extensão do navegador herdado será removida em 28 de fevereiro de 2025.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão de pré-visualização: 7 de novembro de 2024</li>
                <li><span class="preview">Versão de produção para todos os clientes: 7 de novembro de 2024</span></li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

## Aprimoramentos de Relatório e Painel de Controle

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
            Botão de criação de conta do leitor de primeira vez para Conexão de dados</a></p>
            [!BADGE Na produção ]{type=Informative}
            <p>Os administradores que acessam o Data Connect pela primeira vez agora têm a opção de criar uma nova conta do leitor de Snowflake clicando em um único botão. O processo leva alguns minutos para ser concluído, mas não requer mais nenhuma ação.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão de pré-visualização: 14 de novembro de 2024</li>
                <li><span class="preview">Versão de produção para todos os clientes: 14 de novembro de 2024</span></li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### Outras melhorias

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Atualização sobre como os ativos movidos ou excluídos em pastas vinculadas são gerenciados</a></p>
            [!BADGE Na produção ]{type=Informative}
            <p>Alteramos a maneira como os ativos movidos e excluídos são tratados ao usar a integração do Adobe Workfront com o Experience Manager Assets e o Assets Essentials:</p>
            <ul>
                <li>Ativos excluídos: quando um ativo é excluído dentro de uma pasta vinculada no Assets ou Assets Essentials, o ativo excluído é retido na área Documentos do projeto.</li>
                <li>Ativos movidos: quando um ativo é movido para fora de uma pasta vinculada no Assets ou no Assets Essentials, o ativo movido é retido na área Documentos do projeto.</li>
            </ul>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão de pré-visualização: 21 de novembro de 2024</li>
                <li><span class="preview">Versão de produção para todos os clientes: 5 de dezembro de 2024</span></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            As seções em um formulário personalizado agora podem ser recolhidas e expandidas</a></p>
            [!BADGE Na produção para a versão rápida ]{type=Positive}
            <p>Quando um formulário personalizado com várias seções é anexado a um objeto, agora é possível recolher e expandir todas as seções, exceto a seção padrão na parte superior do formulário. O administrador também pode visualizar essa funcionalidade ao visualizar o formulário no designer do formulário.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão de pré-visualização: 11 de novembro de 2024</li>
                <li>Produção para lançamento rápido: com o lançamento do 24.12 (12 de dezembro de 2024)</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (janeiro de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            O Assistente de IA agora pode trabalhar com projetos, tarefas e problemas</a></p>
            [!BADGE Na produção para a versão rápida ]{type=Positive}
            <p>Para facilitar o gerenciamento de itens de trabalho no Workfront, atualizamos o Assistente de IA para trabalhar com projetos, tarefas e problemas. Agora, o AI Assistant pode localizar projetos, tarefas e problemas com base nos critérios especificados.</p>
        </td>
        <td>
            <p><b>Disponível nas seguintes datas:</b></p>
            <ul>
                <li>Versão de pré-visualização: 31 de outubro de 2024</li>
                <li>Produção para lançamento rápido: com o lançamento do 24.11 (14 de novembro de 2024)</li>
                <li>Versão de produção para todos os clientes: com a versão 25.1 (janeiro de 2025)</li>
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

Novos recursos no Workfront Fusion estão disponíveis na produção em uma cadência fora da programação de lançamento do Primeiro trimestre de 2025. Para obter mais informações sobre os recursos mais recentes, consulte [atividade de versão do Adobe Workfront Fusion](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Melhorias no planejamento do Workfront

Novos recursos no Workfront Planning estão disponíveis na Produção. Para obter mais informações sobre os recursos mais recentes, consulte a [atividade da versão do Adobe Workfront Planning First Quarter 2025](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q1.md).

### Aprimoramentos no Planejador de cenários do Workfront

Não há atualizações do Planejador de cenários neste momento na versão. Esta área será atualizada quando houver atualizações disponíveis.

### Aprimoramentos do Workfront Proof

Não há atualizações do Workfront Proof neste momento na versão. Esta área será atualizada quando houver atualizações disponíveis.

### Aprimoramentos das metas do Workfront

Não há atualizações do Workfront Goals neste momento na versão. Esta área será atualizada quando houver atualizações disponíveis.

### API versão 19

Para a API versão 19, modificamos alguns recursos e endpoints. Algumas das alterações são compatíveis com a nova funcionalidade, enquanto outras facilitam o uso das informações disponíveis por meio da API.

Para obter informações sobre novidades e atualizações, consulte [Novidades na API versão 19](/help/quicksilver/wf-api/api/new-api-version-19.md).

Para obter informações sobre versões de API, consulte [Controle de versão de API e agendamento de suporte](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Atualizações de manutenção do Workfront 

Para obter informações sobre as atualizações de manutenção feitas durante a versão do Primeiro trimestre de 2025, consulte [Atualizações de manutenção do Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Atualizações de treinamento

Explore as atualizações mais recentes feitas em programas de aprendizado, caminhos de aprendizado, vídeos e guias para cada versão de produto do Adobe Workfront. Para obter mais informações, consulte a seção &quot;Novidades&quot; da [página Tutorials do Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=pt-BR).
