---
title: Visão geral da versão do quarto trimestre de 2024
description: This page provides information about functionality that is included in the Fourth Quarter 2024 release. Essas melhorias estão previstas para serem disponibilizadas no ambiente de produção ao longo do trimestre.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6cc67488-1ba9-4455-9152-366aaabf0939
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '2194'
ht-degree: 14%

---

# Visão geral da versão do quarto trimestre de 2024

Esta página fornece informações sobre as funcionalidades incluídas na versão do quarto trimestre de 2024. Essas melhorias estão previstas para serem disponibilizadas no ambiente de produção ao longo do trimestre.

<span class="preview">Os recursos fora do ciclo (aqueles que são lançados na produção antes da data de lançamento do quarto trimestre de 2024) estão destacados em amarelo.</span>

>[!IMPORTANT]
>
>A versão 23.3 incluía a opção de mover sua organização para versões mensais. Portanto, o Workfront alterou o esquema de numeração das versões para considerar as faixas de lançamento mensais e trimestrais. O primeiro número indica o ano, e o segundo número indica o mês do lançamento. Exemplo: a versão de abril de 2024 é 24.4.
>
>As versões mensais e trimestrais estão previstas para serem disponibilizadas na quinta-feira da segunda semana completa do mês, salvo indicação em contrário.
>
>| Versão mensal | Versão trimestral |
>|----|----|
>| <ul><li>24.8 (15 de agosto de 2024)</li><li>24.9 (September 12, 2024)</li><li>24.10 (October 17, 2024)</li></ul> | <ul><li>24.10 (October 17, 2024)</li></ul> |
>
>Note that for the final release of each quarter (24.10 this quarter), users on the fast release schedule will receive the release one day early.
>
>Para obter mais informações sobre o processo de lançamento rápido, consulte [Habilitar ou desabilitar o processo de lançamento rápido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Aprimoramentos do Adobe Workfront

* [Aprimoramentos do administrador](#administrator-enhancements)
* [Aprimoramentos no gerenciamento de documentos](#document-management-enhancements)
* [Aprimoramentos na página inicial](#home-enhancements)
* [Aprimoramentos de integração](#integration-enhancements)
* [Aprimoramentos de projeto](#project-enhancements)
* [Aprimoramentos na revisão](#proofing-enhancements)
* [Aprimoramentos no Painel e Relatório](#report-and-dashboard-enhancements)
* [Outros aprimoramentos](#other-enhancements)
* [Funcionalidade que será removida em breve do Workfront](#functionality-soon-to-be-removed-from-workfront)

### Aprimoramentos do administrador

<table>
    <col style="width: 50%;" />
    <col style="width: 50%;" />
        <tbody>
            <tr>
                <td>
                    <p><span class="bold">Recurso</span>
                    </p>
                </td>
                <td>
                    <p><span class="bold">Datas de lançamento</span>
                    </p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Nível de acesso agora disponível na promoção do ambiente</a></p>
                    [!BADGE Na produção &#x200B;]{type=Informative}
                    <p>Para expandir os recursos da funcionalidade de promoção de ambiente, adicionamos a capacidade de incluir níveis de acesso. Agora é possível configurar um nível de acesso em um ambiente de sandbox e promovê-lo ao ambiente de produção.</p>
                </td>
                <td><p><b>Disponível nas seguintes datas:</b></p>
                    <ul>
                        <li>
                            <p>Versão preliminar: sexta-feira, 17 de outubro de 2024</p>
                        </li>
                        <li>
                            <p>Versão de produção para todos os clientes: com a versão 24.10 (17 de outubro de 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Um contador em formulários personalizados mostra o número de campos</a></p>
                    [!BADGE Na produção &#x200B;]{type=Informative}
                    <p>Os formulários personalizados são limitados a 500 campos. Em um formulário longo, pode ser difícil saber quantos campos estão no formulário e se você está se aproximando do limite. Um contador foi adicionado aos formulários personalizados na parte inferior esquerda. O contador exibe quantos campos são usados no formulário e ele fica sempre visível à medida que você rola a tela dentro do designer do formulário.</p>
                </td>
                <td><p><b>Disponível nas seguintes datas:</b></p>
                    <ul>
                        <li>
                            <p>Versão preliminar: quarta-feira, 1 de outubro de 2024</p>
                        </li>
                        <li>
                            <p>Versão de produção para todos os clientes: com a versão 24.10 (17 de outubro de 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">A "Select all" option is now available in layout templates</a></p>
                    [!BADGE Na produção &#x200B;]{type=Informative}
                    <p>Para ajudá-lo a exibir e ocultar mais facilmente campos com modelos de layout, uma caixa de seleção “Selecionar tudo” foi adicionada às áreas Visão geral e Finanças da exibição Detalhes em um modelo de layout. Essa opção estará disponível quando você selecionar Projeto, Tarefa, Ocorrência, Portfolio ou Programa em “Personalizar o que os usuários veem”.</p>
                </td>
                <td><p><b>Disponível nas seguintes datas:</b></p>
                    <ul>
                        <li>
                            <p>Versão preliminar: sexta-feira, 29 de agosto de 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Versão de produção para todos os clientes: 29 de agosto de 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Reverter pacotes de promoção de ambiente</a></p>
                    [!BADGE Na produção &#x200B;]{type=Informative}
                    <p>Para tornar a promoção do ambiente mais flexível e fácil de usar, ativamos a funcionalidade de reversão. Agora, é possível reverter pacotes em 24 horas, permitindo restaurar com mais facilidade as configurações anteriores que foram afetadas por um pacote de promoção de ambiente.</p>
                </td>
                <td><p><b>Disponível nas seguintes datas:</b></p>
                    <ul>
                        <li>
                            <p>Versão preliminar: sexta-feira, 29 de agosto de 2024</p>
                        </li>
                        <li>
                            <p>Produção para lançamento rápido: com o lançamento 24.9 (12 de setembro de 2024)</p>
                        </li>
                        <li>
                            <p>Versão de produção para todos os clientes: com a versão 24.10 (17 de outubro de 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">O botão Layout no designer de formulário personalizado permite duas ou três colunas</a></p>
                    <p>Um botão "Layout" no designer de formulário personalizado permite escolher entre uma área de trabalho de duas ou três colunas. O designer do formulário original usa três colunas e as configurações de campo são exibidas na coluna mais à direita. Se você selecionar duas colunas, as configurações de campo serão exibidas ao lado da biblioteca de campos na coluna à esquerda.</p>
                </td>
                <td><p><b>Disponível nas seguintes datas:</b></p>
                    <ul>
                        <li>
                            <p><s>Versão preliminar: terça-feira, 12 de agosto de 2024</s></p>
                        </li>
                        <li>
                            <p>Produção para lançamento rápido: N/A</p>
                        </li>
                        <li>
                            <p>Versão de produção para todos os clientes: N/A</p>
                        </li>
                    </ul>
                    <p><i>Esse recurso foi removido da Visualização e não será lançado em versões futuras.</i></p>
                </td>
            </tr>
        </tbody>
</table>

### Aprimoramentos no gerenciamento de documentos

>[!IMPORTANT]
>
>Os recursos listados em **Aprimoramentos no gerenciamento de documentos** fazem parte de uma versão em fases e estão disponíveis apenas para clientes específicos.

<table>
    <col style="width: 50%;" />
    <col style="width: 50%;" />
        <tbody>
            <tr>
                <td>
                    <p><span class="bold">Recurso</span>
                    </p>
                </td>
                <td>
                    <p><span class="bold">Datas de lançamento</span>
                    </p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-document-mgmt-enhancements.md">Exibir o status de decisão do documento diretamente na lista de documentos</a></p>
                    <p>Agora você pode visualizar o status de decisão de um documento diretamente na lista de documentos.</p>
                </td>
                <td><p><b>Disponível nas seguintes datas:</b></p>
                    <ul>
                        <li>
                            <p><s>Versão preliminar: sexta-feira, 3 de outubro de 2024</s></p>
                        </li>
                        <li>
                            <p>Versão de produção para todos os clientes: com a versão 24.10 (17 de outubro de 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-document-mgmt-enhancements.md">Quickly add previous reviewers and approvers to new document versions</a></p>
                    [!BADGE Na produção &#x200B;]{type=Informative}
                    <p>Agora é possível adicionar rapidamente revisores e aprovadores de versões anteriores do documento.</p>
                </td>
                <td><p><b>Disponível nas seguintes datas:</b></p>
                    <ul>
                        <li>
                            <p>Versão preliminar: sexta-feira, 3 de outubro de 2024</p>
                        </li>
                        <li>
                            <p>Versão de produção para todos os clientes: com a versão 24.10 (17 de outubro de 2024)</p>
                        </li>
                    </ul>
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
                    <p><span class="bold">Recurso</span>
                    </p>
                </td>
                <td>
                    <p><span class="bold">Datas de lançamento</span>
                    </p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-home-enhancements.md">Atualizações para o widget Aguardando minha aprovação em uma nova página inicial</a></p>
                    [!BADGE Na produção &#x200B;]{type=Informative}
                    <p>Fizemos as seguintes alterações no widget Aguardando minha aprovação:</p>
                        <ul>
                            <li>O widget foi renomeado como: O nome desse widget agora é Minhas aprovações.</li>
                            <li>Adicionei as aprovações que enviei como uma opção de filtro: agora você pode visualizar as aprovações que enviou em uma nova página inicial com este widget.</li>
                            <li>Prazo: agora você pode ver o prazo da prova, se um tiver sido definido. Se um prazo não for definido, ele assumirá como padrão a data de criação.</li>
                        </ul>
                </td>
                <td><p><b>Disponível nas seguintes datas:</b></p>
                    <ul>
                        <li>
                            <p>Versão preliminar: sexta-feira, 10 de outubro de 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Versão de produção para todos os clientes: 10 de outubro de 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-home-enhancements.md">Apresentando Prioridades: uma experiência de Workfront mais simples, simplificada e intuitiva para proprietários de tarefas</a></p>
                    [!BADGE Na produção &#x200B;]{type=Informative}
                    <p>As prioridades aumentam o foco e a produtividade para ajudar os clientes a realizar mais em menos tempo.</p>
                    <p>Com as Prioridades, você pode aproveitar:</p>
                        <ul>
                            <li>Gerencie e priorize tarefas diárias: organize seu dia ou semana com a navegação consolidada para maior clareza.</li>
                            <li>Maior produtividade: acesse o contexto do projeto e execute tarefas com mais rapidez e menos cliques.</li>
                            <li>Recursos personalizados: aproveite os recursos criados exclusivamente para proprietários de tarefas.</li>
                        </ul>
                </td>
                <td><p><b>Disponível nas seguintes datas:</b></p>
                    <ul>
                        <li>
                            <p>Versão preliminar: sexta-feira, 3 de outubro de 2024</p>
                        </li>
                        <li>
                            <p>Versão de produção para todos os clientes: com a versão 24.10 (17 de outubro de 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
        </tbody>
</table>

### Aprimoramentos de integração

<table>
    <col style="width: 50%;" />
    <col style="width: 50%;" />
        <tbody>
            <tr>
                <td>
                    <p><span class="bold">Recurso</span>
                    </p>
                </td>
                <td>
                    <p><span class="bold">Datas de lançamento</span>
                    </p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Aprimoramentos na experiência de logon de integração com o Outlook</a></p>
                    [!BADGE Na produção &#x200B;]{type=Informative}
                    <p>A experiência de logon para integração com o Outlook foi simplificada para que todos os clientes vejam o mesmo botão para fazer logon no Workfront, independentemente de estarem habilitados para IMS. As etapas de logon subsequentes permanecem diferentes para instâncias IMS e não IMS, mas a página inicial é a mesma para todos os usuários.</p>
                </td>
                <td><p><b>Disponível nas seguintes datas:</b></p>
                    <ul>
                        <li>
                            <p>Versão preliminar: quarta-feira, 6 de agosto de 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Versão de produção para todos os clientes: 6 de agosto de 2024</span></p>
                        </li>
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
                    <p><span class="bold">Recurso</span>
                    </p>
                </td>
                <td>
                    <p><span class="bold">Datas de lançamento</span>
                    </p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Atribuições mais relevantes adicionadas ao fluxo de trabalho Nova Tarefa</a></p>
                    [!BADGE Na produção para a versão rápida &#x200B;]{type=Positive}
                    <p>Adicionamos a mesma funcionalidade para atribuições inteligentes mais relevantes ao campo Atribuições na caixa Nova tarefa ao adicionar uma tarefa a um projeto e em uma lista de tarefas de projeto.</p>
                </td>
                <td><p><b>Disponível nas seguintes datas:</b></p>
                    <ul>
                        <li>
                            <p>Versão preliminar: quarta-feira, 13 de fevereiro de 2024</p>
                        </li>
                        <li>
                            <p>Produção para lançamento rápido: com o lançamento 24.5 (16 de maio de 2024)</p>
                        </li>
                    </ul>
                <p><i>Esse recurso foi removido da Visualização e da Produção de versão rápida.</i></p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Mais atribuições inteligentes relevantes</a></p>
                    [!BADGE Em produção para versão rápida &#x200B;]{type=Positive}
                    <p>Alteramos o algoritmo que o Workfront usa para calcular e sugerir atribuições inteligentes para tarefas. O novo algoritmo se aplica às seguintes áreas no Workfront em que você atribui uma tarefa: listas de tarefas, a área Atribuições no cabeçalho da tarefa, Início e o painel Resumo.</p>
                </td>
                <td><p><b>Disponível nas seguintes datas:</b></p>
                    <ul>
                        <li>
                            <p>Versão preliminar: sexta-feira, 21 de dezembro de 2023</p>
                        </li>
                        <li>
                            <p>Produção para versão rápida: com a versão 24.5 (16 de maio de 2024)</p>
                        </li>
                    </ul>
                <p><i>Esse recurso foi removido da Visualização e da Produção de versão rápida.</i></p>
                </td>
            </tr>
        </tbody>
</table>

### Aprimoramentos na revisão

<table>
    <col style="width: 50%;" />
    <col style="width: 50%;" />
        <tbody>
            <tr>
                <td>
                    <p><span class="bold">Recurso</span>
                    </p>
                </td>
                <td>
                    <p><span class="bold">Datas de lançamento</span>
                    </p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Copy/paste issue fix for the Desktop Proofing Viewer</a></p>
                    [!BADGE Na produção &#x200B;]{type=Informative}
                    <p>Corrigimos um problema em que o conteúdo é colado incorretamente na seção Atualizações do Visualizador de provas de desktop.</p>
                    <p>Nova versão: 2.1.39</p>
                </td>
                <td><p><b>Disponível nas seguintes datas:</b></p>
                    <ul>
                        <li>
                            <p>Versão preliminar: quinta-feira, 2 de outubro de 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Versão de produção para todos os clientes: 2 de outubro de 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Correção de tela em branco para usuários do Windows do Desktop Proofing Viewer</a></p>
                    [!BADGE Na produção &#x200B;]{type=Informative}
                    <p>Corrigimos um problema na nova versão 2.1.36 do Desktop Proofing Viewer que fazia com que alguns usuários do Windows vissem uma tela em branco após abrirem o visualizador. </p>
                    <p>Nova versão para usuários do Windows: 2.1.37</p>
                </td>
                <td><p><b>Disponível nas seguintes datas:</b></p>
                    <ul>
                        <li>
                            <p>Versão preliminar: sábado, 30 de agosto de 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Versão de produção para todos os clientes: 30 de agosto de 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Atualização do Chromium para o Visualizador de Revisão de Texto de Área de Trabalho</a></p>
                    [!BADGE Na produção &#x200B;]{type=Informative}
                    <p>Estamos atualizando o Visualizador de revisão de desktop para oferecer suporte ao Chromium 126.0.6478.127, que resolverá problemas com elementos de interface em provas interativas.</p>
                </td>
                <td><p><b>Disponível nas seguintes datas:</b></p>
                    <ul>
                        <li>
                            <p>Versão preliminar: sexta-feira, 29 de agosto de 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Production release for all customers: August 29, 2024</span></p>
                        </li>
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
                    <p><span class="bold">Recurso</span>
                    </p>
                </td>
                <td>
                    <p><span class="bold">Datas de lançamento</span>
                    </p>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">Workfront Data Connect disponível para novos planos</a></p>
                    [!BADGE Na produção &#x200B;]{type=Informative}
                    <p>O Workfront Data Connect ficará disponível para organizações em um dos novos planos da Workfront. A Data Connect permite que as organizações acessem seus dados como um data lake seguro e escalável, que pode ser analisado e visualizado usando ferramentas de business intelligence ou armazenado externamente. Além disso, as organizações podem usar o Data Connect para exibir análises de dados que estavam indisponíveis anteriormente, como análise de tendências com base no tempo, mapeamento de variáveis e análise de dados de sistemas externos em combinação com dados do Workfront.</p>
                </td>
                <td><p><b>Disponível nas seguintes datas:</b></p>
                    <ul>
                        <li>
                            <p>Versão de produção para todos os clientes: com a versão 24.10 (17 de outubro de 2024)</p>
                        </li>
                    </ul>
                    <p><i>Disponível apenas para organizações em um dos novos planos da Adobe Workfront. O Data Connect está incluído no plano Ultimate e será disponibilizado para compra como um complemento dos planos Prime e Select no primeiro semestre de 2025.</i></p>
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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Resuma projetos ou atualizações com um clique</a></p>
                    [!BADGE Na produção &#x200B;]{type=Informative}
                    <p>Para facilitar a visualização rápida dos destaques de um projeto ou de uma sequência de atualizações, adicionamos botões Resumir a essas áreas do Workfront. Agora, você pode clicar no botão para gerar um resumo no Assistente do AI.</p><p>Anteriormente, os usuários podiam abrir o assistente do AI e digitar um prompt para criar um resumo do projeto ou atualizar o fluxo.</p>
                </td>
                <td><p><b>Disponível nas seguintes datas:</b></p>
                    <ul>
                        <li>
                            <p>Versão preliminar: sexta-feira, 3 de outubro de 2024</p>
                        </li>
                        <li>
                            <p>Versão de produção para todos os clientes: com a versão 24.10 (17 de outubro de 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-24-q4.md" class="MCXref xref" xrefformat="{para}">Disponibilidade geral do Adobe Workfront Planning</a></p>
                    [!BADGE Na produção &#x200B;]{type=Informative}
                    <p>O Workfront Planning está disponível para todos os clientes que compraram uma licença do Workfront Planning, além da licença do Workfront. Entre em contato com seu representante de conta para obter mais informações sobre o Workfront Planning.</p>
                    <p>Para obter as informações mais recentes da versão do Workfront Planning a cada trimestre, consulte a seção <a href="#workfront-planning-enhancements">Aprimoramentos do Workfront Planning</a> abaixo.</p>
                </td>
                <td><p><b>Disponível nas seguintes datas:</b></p>
                    <ul>
                        <li>
                            <p><span class="preview">Versão de produção para todos os clientes: 28 de agosto de 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Assistente do Adobe AI disponível no Workfront</a></p>
                    [!BADGE Na produção &#x200B;]{type=Informative}
                    <p>Para facilitar a realização do trabalho, adicionamos o Assistente de IA da Adobe à Workfront. AI Assistant can help you by:</p>
                    <ul>
                        <li>Resumir itens de trabalho e documentos, permitindo que você obtenha rapidamente uma compreensão geral de tarefas, projetos e ativos.</li>
                        <li>Fornecer informações da documentação do Experience League, trazer instruções e material de referência para o Workfront, ao mesmo tempo em que fornece um link para uma documentação mais detalhada.</li>
                        <li>Criar e refinar fórmulas para campos de formulário personalizados calculados, gerar fórmulas a partir de prompts de texto ou localizar erros em fórmulas existentes.</li>
                        </ul>
                        <p>O administrador do Workfront pode ativar ou desativar o Assistente de IA da organização. O Assistente do AI está disponível para instâncias com planos Select, Prime e Ultimate.</p>
                    </td>
                <td><p><b>Disponível nas seguintes datas:</b></p>
                    <ul>
                        <li>
                            <p>Versão preliminar: quinta-feira, 28 de agosto de 2024</p>
                        </li>
                        <li>
                            <p class="preview">Versão de produção: 28 de agosto de 2024</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Atualizações de aparência e funcionalidade durante o período do quarto trimestre de 2024</a></p>
                    <p>Pequenas atualizações na aparência de várias áreas do aplicativo Adobe Workfront estão sendo feitas dentro do período do quarto trimestre de 2024. Revise as notas de versão individuais para ver as datas de lançamento específicas.</p>
                </td>
                <td><p><b>Disponível nas seguintes datas:</b></p>
                    <ul>
                        <li>
                            <p>Preview release: Throughout the Fourth Quarter 2024 release timeframe</p>
                        </li>
                        <li>
                            <p><span class="preview">Versão de produção: revise as notas de versão para datas específicas</span></p>
                        </li>
                    </ul>
                </td>
            </tr>                            
        </tbody>
</table>

### Funcionalidade que será removida em breve do Workfront

A seguinte funcionalidade será removida do Workfront em breve:

#### Substituição da experiência inicial herdada com o 24.10

Descontinuaremos oficialmente a experiência herdada do Início com a versão 24.10. Os usuários são incentivados a começar a usar a nova Página inicial, que continuará a ser aprimorada com recursos adicionais antes da desativação.

## Anúncios

### Aprimoramentos do Workfront Fusion

Novos recursos do Workfront Fusion estão disponíveis na produção em uma cadência fora do cronograma de versões do quarto trimestre de 2024. Para obter mais informações sobre os recursos mais recentes, consulte [Atividade de lançamento do Adobe Workfront Fusion](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Aprimoramentos do Workfront Planning

Novos recursos no Workfront Planning estão disponíveis em Produção. Para obter mais informações sobre os recursos mais recentes, consulte [Atividade da versão do Adobe Workfront Planning do quarto trimestre de 2024](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-24-q4.md).

### Aprimoramentos do Planejador de Cenário do Workfront

Não há atualizações do Planejador de Cenários neste ponto da versão. Esta área será atualizada quando houver atualizações disponíveis.

### Aprimoramentos do Workfront Proof

Não há atualizações do Workfront Proof neste ponto da versão. Esta área será atualizada quando houver atualizações disponíveis.

### Aprimoramentos das metas do Workfront

Não há atualizações do Workfront Goals neste momento na versão. Esta área será atualizada quando houver atualizações disponíveis.

### API versão 19

Para a versão 19 da API, modificamos alguns recursos e pontos de acesso. Algumas das alterações oferecem suporte a novas funcionalidades, enquanto outras facilitam o uso das informações disponíveis por meio da API.

Para obter informações sobre as novidades e atualizações, consulte [Novidades na versão 19 da API](/help/quicksilver/wf-api/api/new-api-version-19.md).

Para obter informações sobre as versões da API, consulte [controle de versão da API e cronograma de suporte](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Atualizações de manutenção do Workfront

Para obter informações sobre as atualizações de manutenção feitas durante a versão do quarto trimestre de 2024, consulte [Atualizações de manutenção do Workfront](https://experienceleague.adobe.com/pt-br/docs/workfront-known-issues/releases/current-updates).

### Atualizações de treinamento

Explore as últimas atualizações feitas nos programas de aprendizagem, caminhos de aprendizagem, vídeos e guias para cada versão do Adobe Workfront. Para obter mais informações, consulte a seção &quot;Novidades&quot; da [página de tutoriais do Workfront](https://experienceleague.adobe.com/pt-br/docs/workfront-learn/tutorials-workfront/home?lang=pt-BR).
