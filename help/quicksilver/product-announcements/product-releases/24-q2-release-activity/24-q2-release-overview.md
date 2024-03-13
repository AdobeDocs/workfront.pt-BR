---
title: Visão geral da versão do segundo trimestre de 2024
description: Esta página fornece informações sobre a funcionalidade incluída na versão do segundo trimestre de 2024. Essas melhorias estão planejadas para serem disponibilizadas no ambiente de produção durante todo o trimestre.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 1e103c41d225c3bcc2699da24b0c6733c09b6637
workflow-type: tm+mt
source-wordcount: '1584'
ht-degree: 0%

---

# Visão geral da versão do segundo trimestre de 2024

Esta página fornece informações sobre a funcionalidade incluída na versão do segundo trimestre de 2024. Essas melhorias estão planejadas para serem disponibilizadas no ambiente de produção durante todo o trimestre.

<!--The 24.1 release webinar was on January 11, 2024. You can [register for the webinar to view an on-demand recording here](https://webinars.on24.com/adobe_workfront/whatsnewin241?partnerref=releaseoverview). -->

<span class="preview">Os recursos fora do ciclo (aqueles que foram lançados para produção antes da data de lançamento do Segundo trimestre de 2024) estão destacados em amarelo.</span>

>[!IMPORTANT]
>
>A versão 23.3 incluía a opção de mover sua organização para versões mensais. Portanto, a Workfront alterou o esquema de numeração de versões para contabilizar as faixas de lançamento mensais e trimestrais. O primeiro número designa o ano e o segundo número significa o mês do lançamento. Exemplo: a versão de abril de 2024 é 24.4.
>
>Os lançamentos mensais e trimestrais devem estar disponíveis na quinta-feira da segunda semana completa do mês, a menos que especificado de outra forma.
>
>| Lançamento mensal | Versão trimestral |
>|----|----|
>| <ul><li>24.2 (15 de fevereiro de 2024)</li><li>24.3 (14 de março de 2024)</li><li>24.4 (11 de abril de 2024)</li></ul> | <ul><li>24.4 (abril de 2024)</li></ul> |
>
>Para obter mais informações sobre o processo de lançamento rápido, consulte [Ativar ou desativar o processo de lançamento rápido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Aprimoramentos do Adobe Workfront

* [Melhorias do administrador](#administrator-enhancements)
* [Aprimoramentos na página inicial](#home-enhancements)
* [Aprimoramentos do projeto](#project-enhancements)
* [Melhorias no gerenciamento de recursos](#resource-management-enhancements)
* [Melhorias no fluxo de atualização e na notificação](#update-stream-and-notification-enhancements)
* [Outras melhorias](#other-enhancements)

### Melhorias do administrador

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">A integração JumpSeat agora está disponível para novos tipos de pacote</a></p>
                        <p>A integração do JumpSeat existente agora está disponível para contas que usam um dos novos tipos de pacote (ou seja, Select, Prime ou Ultimate). Você ainda deve ter uma assinatura ativa do JumpSeat para habilitar a integração.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 26 de fevereiro de 2024</p>
                            </li>
                            <li>
                                <p>Produção para lançamento rápido: com o lançamento do 24.3 (14 de março de 2024)</p>
                            </li>
                            <li>
                                <p>Produção para versão trimestral: com a versão 24.4 (abril de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Os campos nativos do Workfront estão disponíveis no designer de formulário beta</a></p>
                        <p>Os campos nativos do Workfront agora estão disponíveis para você adicionar aos seus formulários personalizados. Esse novo tipo de campo permite organizar e apresentar dados aos usuários de forma lógica, sem precisar recriar dados existentes em campos personalizados.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 29 de fevereiro de 2024</p>
                            </li>
                            <li>
                                <p>Produção para lançamento rápido: com o lançamento do 24.3 (14 de março de 2024)</p>
                            </li>
                            <li>
                                <p>Produção para versão trimestral: com a versão 24.4 (abril de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">O mapeamento de atributos agora está disponível para organizações que migraram para o Adobe IMS</a></p>
                        <p>[!BADGE Na produção ]{type=Informative}</p><p>Os administradores de sistema do Workfront agora podem configurar o mapeamento de atributos do usuário para organizações que migraram para o Adobe IMS. Isso permite que as informações do usuário sejam passadas para o Workfront pelo provedor de SSO (Logon único) da organização, para que os dados do usuário não precisem ser inseridos no Workfront e no provedor de SSO.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 22 de fevereiro de 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Versão de produção para todos os clientes: 22 de fevereiro de 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">A lógica de salto e a lógica de exibição agora estão disponíveis no designer de formulário beta</a></p><p>[!BADGE Na produção para a versão rápida ]{type=Positive}</p>
                        <p>Agora é possível editar a exibição existente, ignorar a lógica e adicionar uma nova lógica aos formulários personalizados no designer de formulário beta. Um construtor de lógica fácil de usar ajuda a definir quais campos exibir ou ignorar com base nas seleções no formulário.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 8 de fevereiro de 2024</p>
                            </li>
                            <li>
                                <p>Produção para lançamento rápido: com o lançamento do 24.2 (15 de fevereiro de 2024)</p>
                            </li>
                            <li>
                                <p>Produção para lançamento trimestral: a ser definido</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Opções de coluna adicionadas aos controles do Administrador para a nova Página inicial usando modelos de layout</a></p><p>[!BADGE Na produção para a versão rápida ]{type=Positive}</p><p>Os administradores agora podem personalizar quais colunas estão disponíveis para usuários em novos widgets da Página inicial específicos usando modelos de layout. As opções incluem ocultar ou exibir colunas padrão e adicionar campos existentes como novas colunas.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 2 de janeiro de 2024</p>
                            </li>
                            <li>
                                <p>Produção para lançamento rápido: com o lançamento do 24.2 (15 de fevereiro de 2024)</p>
                            </li>
                            <li>
                                <p>Produção para versão trimestral: com a versão 24.4 (abril de 2024)</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Melhorias no fluxo de trabalho de criação automatizada de pastas na integração do Adobe Experience Manager</a></p><p>[!BADGE Na produção ]{type=Informative}</p><p>Para garantir que suas pastas do Adobe Experience Manager reflitam com mais precisão suas necessidades, adicionamos árvores de pastas aninhadas ao fluxo de trabalho de pastas vinculadas do Adobe Experience Manager.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 11 de março de 2024</p>
                            </li>
                             <li> <p><span class="preview">Versão de produção para todos os clientes: 14 de março de 2024</span></p>
                             </li>
                        </ul>
                    </td>
                 </tr>          
            </tbody>
</table>

### Aprimoramentos do projeto

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Atribuições mais relevantes adicionadas ao fluxo de trabalho Nova tarefa</a></p><p>Adicionamos a mesma funcionalidade para atribuições inteligentes mais relevantes ao campo Atribuições na caixa Nova tarefa ao adicionar uma tarefa a um projeto e em uma lista de tarefas de projeto.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 13 de fevereiro de 2024</p>
                            </li>
                            <li>
                                <p>Produção para lançamento rápido: com o lançamento do 24.3 (14 de março de 2024)</p>
                            </li>
                            <li>
                                <p>Produção para versão trimestral: com a versão 24.4 (abril de 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Atribuições inteligentes mais relevantes</a></p><p>Alteramos o algoritmo que o Workfront usa para calcular e sugerir atribuições inteligentes para tarefas. O novo algoritmo se aplica às seguintes áreas no Workfront em que você atribui uma tarefa: listas de tarefas, a área Atribuições no cabeçalho da tarefa, Início e o painel Resumo.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 21 de dezembro de 2023</p>
                            </li>
                            <li>
                                <p>Produção para lançamento rápido: com o lançamento do 24.3 (14 de março de 2024)</p>
                            </li>
                            <li>
                                <p>Produção para versão trimestral: com a versão 24.4 (abril de 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
           </tbody>
        </table>

### Melhorias no gerenciamento de recursos

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-resource-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Indicador de alocações ajustadas manualmente no Balanceador de carga de trabalho</a></p><p>[!BADGE Na produção para a versão rápida ]{type=Positive}</p><p>Para fornecer mais clareza sobre ajustes manuais ou contorno no Balanceador de carga de trabalho, as alocações por hora ajustadas manualmente agora mostram um ícone de lápis.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 12 de outubro de 2024</p>
                            </li>
                            <li>
                                <p>Produção para lançamento rápido: com o lançamento do 24.2 (15 de fevereiro de 2024)</p>
                            </li>
                            <li>
                                <p>Produção para versão trimestral: com a versão 24.4 (abril de 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
           </tbody>
        </table>

### Melhorias no fluxo de atualização e na notificação

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">O novo fluxo de comentários agora está disponível em ações rápidas para novos widgets da Página inicial</a></p>
                        <p>Agora adicionamos a nova funcionalidade de comentários ao botão de ação rápida "Adicionar nova atualização" nos widgets Meu trabalho, Meus projetos, Minhas tarefas e Meus problemas na nova página inicial.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 1 de março de 2024</p>
                            </li>
                            <li>
                                <p>Produção para lançamento rápido: com o lançamento do 24.3 (14 de março de 2024)</p>
                            </li>
                            <li>
                                <p>Produção para versão trimestral: com a versão 24.4 (abril de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>  
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">Informações adicionais do comentador disponíveis na nova experiência de comentários</a></p><p>Fizemos os seguintes aprimoramentos na nova experiência de comentários:</p>
                        <ul>
                            <li>
                                <p>Você pode clicar no nome de um comentarista para ver seu nome, função e endereço de email em uma caixa de informações. Essas informações podem ajudar a identificar o usuário correto, se você tiver mais de um usuário com o mesmo nome. Ao clicar no nome do comentarista na caixa de informações, o perfil do usuário é aberto.</p>
                            </li>
                            <li>
                                <p>Seu nome de usuário é destacado nos comentários nos quais você está marcado, quando mencionado no texto do comentário.</p>
                            </li>
                        </ul>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 29 de fevereiro de 2024</p>
                            </li>
                            <li>
                                <p>Produção para lançamento rápido: com o lançamento do 24.3 (14 de março de 2024)</p>
                            </li>
                            <li>
                                <p>Produção para versão trimestral: com a versão 24.4 (abril de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>  
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">A guia Atividade do sistema na nova experiência de comentários aceita comentários somente leitura</a></p><p>Os comentários feitos nos registros de atividade do sistema na experiência de comentários herdada agora são preenchidos na guia Atividade do sistema na nova experiência de comentários como somente leitura. Não é possível responder aos registros de atividade do sistema na nova experiência de comentários.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 22 de fevereiro de 2024</p>
                            </li>
                            <li>
                                <p>Produção para lançamento rápido: com o lançamento do 24.3 (14 de março de 2024)</p>
                            </li>
                            <li>
                                <p>Produção para versão trimestral: com a versão 24.4 (abril de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr> 
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">Nova guia de fluxo de atualização para capturar comentários e entradas de atividade do sistema</a></p><p>Para fornecer uma exibição cronologicamente coesa de comentários e logs de atividades do sistema, estamos introduzindo uma terceira guia à área Atualizações de todos os objetos. A guia "Todos" captura os comentários do usuário e os comentários da atividade do sistema em um fluxo coeso.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 22 de fevereiro de 2024</p>
                            </li>
                            <li>
                                <p>Produção para lançamento rápido: com o lançamento do 24.3 (14 de março de 2024)</p>
                            </li>
                            <li>
                                <p>Produção para versão trimestral: com a versão 24.4 (abril de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">Novo fluxo de comentários agora disponível no painel Resumo</a></p><p>Agora adicionamos a nova funcionalidade de comentários ao painel Resumo para listas de tarefas e problemas.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 22 de fevereiro de 2024</p>
                            </li>
                            <li>
                                <p>Produção para lançamento rápido: com o lançamento do 24.3 (14 de março de 2024)</p>
                            </li>
                            <li>
                                <p>Produção para versão trimestral: com a versão 24.4 (abril de 2024)</p>
                            </li>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Atualizações de aparência durante o segundo trimestre de 2024</a></p><p>Pequenas atualizações na aparência de várias áreas do aplicativo Adobe Workfront estão sendo feitas no período do Segundo trimestre de 2024. Revise as notas de versão individuais para datas de lançamento específicas.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: durante todo o período da versão do segundo trimestre de 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Versão de produção: revise as notas de versão para datas específicas</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
           </tbody>
        </table>   
           </tbody>
        </table>

## Anúncios

### Aprimoramentos do Workfront Fusion

Novos recursos no Workfront Fusion estão disponíveis na produção em uma cadência fora da programação de lançamento do Primeiro trimestre de 2023. Para obter mais informações sobre os recursos mais recentes, consulte [Atividade de lançamento do Adobe Workfront Fusion](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Aprimoramentos no Planejador de cenários do Workfront

Não há atualizações do Planejador de cenários neste momento na versão. Esta área será atualizada quando houver atualizações disponíveis.

### Aprimoramentos de prova do Workfront

Não há atualizações do Workfront Proof neste momento na versão. Esta área será atualizada quando houver atualizações disponíveis.

### Aprimoramentos das metas do Workfront

Não há atualizações do Workfront Goals neste momento na versão. Esta área será atualizada quando houver atualizações disponíveis.

### API versão 16

Para a API versão 16, modificamos alguns recursos e endpoints. Algumas das alterações são compatíveis com a nova funcionalidade, enquanto outras facilitam o uso das informações disponíveis por meio da API.

Para obter informações sobre novidades e atualizações, consulte [Novidades da API versão 16](/help/quicksilver/wf-api/api/new-api-version-16.md).

Para obter informações sobre versões da API, consulte [Controle de versão da API e programação de suporte](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Atualizações de manutenção do Workfront 

Para obter informações sobre as atualizações de manutenção feitas durante a versão 22.3, consulte [Atualizações de manutenção do Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Atualizações de treinamento

Explore as atualizações mais recentes feitas em programas de aprendizado, caminhos de aprendizado, vídeos e guias para cada versão de produto do Adobe Workfront. Para obter mais informações, consulte a seção &quot;Novidades&quot; do [Página do Workfront Tutorials](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=pt-BR).
