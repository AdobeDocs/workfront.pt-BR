---
title: Visão geral da versão 23.3
description: Visão geral da versão 23.3
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 441d84d6-6c40-4a03-967e-836cf78c8fc1
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '2799'
ht-degree: 0%

---

# Visão geral da versão 23.3

Esta página fornece informações sobre a funcionalidade incluída na versão 23.3 do. Essas melhorias foram disponibilizadas no ambiente de Produção com a versão 23.3 do em 20 e 21 de julho de 2023.

O webinário de lançamento do versão 23.3 do foi realizado em 29 de junho de 2023. Você pode [registrar-se no webinário para exibir uma gravação sob demanda aqui](https://webinars.on24.com/adobe_workfront/whatsnewin233?partnerref=exlreleaseoverview).

<span class="preview">Os recursos fora do ciclo (aqueles que foram lançados para produção antes da data de lançamento da versão 23.3) estão destacados em amarelo.</span>

>[!IMPORTANT]
>
>A versão 23.3 inclui a opção de mover sua organização para versões mensais. Portanto, a Workfront está alterando o esquema de numeração de versões para contabilizar as faixas de lançamento mensais e trimestrais.
>
>* Se você estiver na faixa de **lançamento rápido (mensal)**, o lançamento após a versão 23.3 será **23.8**, em 31 de agosto de 2023.
>* Se você estiver na faixa de lançamento **trimestral**, o lançamento após a versão 23.3 será **23.10**, na semana de 26 de outubro de 2023.
> 
> As versões trimestrais incluirão a funcionalidade de três versões mensais. Por exemplo, a versão trimestral 23.10 incluirá funcionalidades lançadas nas versões mensais 23.8, 23.9 e 23.10.
>
>Os lançamentos mensais e trimestrais estão planejados para estarem disponíveis na última quinta-feira do mês.
>
>| Lançamento mensal | Versão trimestral |
>|----|----|
>| <ul><li>23.8 (31 de agosto de 2023)</li><li>23.9 (28 de setembro de 2023)</li><li>23.10 (26 de outubro de 2023)</li></ul> | <ul><li>23.10 (Semana de 26 de outubro de 2023)</li></ul> |
>| <ul><li>Nenhuma versão (novembro de 2023)</li><li>Nenhuma versão (dezembro de 2023)</li><li>24.1 (janeiro de 2024)</li></ul> | <ul><li>24.1 (janeiro de 2024)</li></ul> |
>
>Para obter mais informações sobre o processo de lançamento rápido, consulte [Habilitar ou desabilitar o processo de lançamento rápido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Aprimoramentos do Adobe Workfront

* [Melhorias do administrador](#administrator-enhancements)
* [Aprimoramentos do Agile](#agile-enhancements)
* [Aprimoramentos do Financial Management](#financial-management-enhancements)
* [Aprimoramentos de integração](#integration-enhancements)
* [Aprimoramentos do projeto](#project-enhancements)
* [Melhorias na mobilidade](#mobile-enhancements)
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Habilitar ciclos de lançamento mais rápidos do Workfront</a></p>
                        <p>Para permitir que você receba novos recursos e atualizações de produtos da Workfront com mais rapidez, adicionamos a capacidade de ativar ciclos de lançamento mais rápidos. Agora, você pode optar por fazer com que sua organização receba versões do Workfront com mais frequência do que uma vez por trimestre. O ciclo de lançamento trimestral ainda estará disponível para organizações que preferem versões menos frequentes.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 22 de junho de 2023</p>
                            </li>
                            <li>
                                <p>Versão de produção: com a versão 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Controle em nível de grupo disponível para a preferência de horas e folha de horas "Onde os usuários podem registrar horas"</a></p>
                        <p>O administrador do sistema agora pode bloquear e desbloquear a planilha de horas e a preferência de horas "Onde os usuários podem registrar horas". Quando essa preferência estiver desbloqueada, os administradores de grupo poderão definir as configurações de "Onde os usuários podem registrar horas" separadamente para cada grupo.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 4 de maio de 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Versão de produção: 18 de maio de 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Exibir lógica e ignorar indicadores e regras de lógica exibidos no designer de formulário beta</a></p>
                        <p>O beta público do designer de formulário foi reativado na Pré-visualização e Produção em 21 de julho de 2023. Além disso, agora é possível visualizar as regras de lógica existentes criadas em formulários personalizados herdados no designer de formulários.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 21 de julho de 2023</p>
                            </li>
                            <li>
                                <p>Versão de produção: 21 de julho de 2023</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

### Aprimoramentos do Agile

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">A Exibição Agile de um projeto exibe um quadro kanban</a></p>
                        <p>A Exibição Agile de um projeto agora inclui funcionalidades adicionais para filtrar, agrupar e classificar trabalho em um quadro kanban. O novo design flexível da visualização inclui um recurso de pesquisa robusto e a capacidade de adicionar novas tarefas ao projeto diretamente do quadro.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 29 de junho de 2023</p>
                            </li>
                            <li>
                                <p>Versão de produção para todos os clientes: com a versão 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Classificar por colunas do quadro</a></p>
                        <p>Adicionamos a capacidade de classificar os cartões nas colunas em um quadro. Quando você seleciona uma opção para classificar por, todas as colunas são classificadas. Não é possível classificar uma única coluna, e a coluna de backlog ou de entrada não é classificada.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 22 de junho de 2023</p>
                            </li>
                            <li>
                                <p>Versão de produção para todos os clientes: com a versão 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>                             
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Modo escuro agora disponível em Adobe Workfront Boards</a></p>
                        <p>Agora é possível exibir todas as placas e fluxos de trabalho no modo escuro. A nova configuração está disponível por meio das preferências no painel Quadros.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de visualização: 22 de junho de 2023<span style="color: #ff0000;"> Esse recurso foi removido da Visualização e não será lançado com a versão 23.3.</span></p>
                            </li>
                            <li>
                                <p>Versão de produção para todos os clientes: N/D</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Metas disponíveis em iterações de fluxo de trabalho em painéis do Adobe Workfront</a></p>
                        <p>Adicionamos a capacidade de adicionar metas a uma iteração, sem precisar listar as metas em um cartão. As metas são adicionadas em um formato de lista de verificação e podem ser marcadas como concluídas. A área de métricas na parte superior direita da iteração mostra quantas metas existem e quantas foram concluídas.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de visualização: 22 de junho de 2023<span style="color: #ff0000;"> Esse recurso foi removido da Visualização e não será lançado com a versão 23.3.</span></p>
                            </li>
                            <li>
                                <p>Versão de produção para todos os clientes: N/D</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Adicionar comentários aos cartões nos quadros</a></p>
                        <p>Agora é possível adicionar comentários a cartões ad hoc e conectados em quadros e marcar outros usuários nos comentários. Os comentários estão disponíveis nos detalhes do cartão. O recurso de comentário para quadros usa a nova experiência de comentário do Adobe Workfront.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 15 de junho de 2023</p>
                            </li>
                            <li>
                                 <p>Versão de produção para aceitação antecipada: 22 de junho de 2023 <span style="color: #ff0000;"> Esse recurso está disponível na Produção nesta data somente por meio da aceitação antecipada de recursos para Workfront Boards.</span></p>
                                <p>Versão de produção para todos os clientes: com a versão 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Melhorias no gerenciador de tags do Boards</a></p>
                        <p>A interface do gerenciador de tags foi aprimorada, permitindo criar novas tags rapidamente e aplicá-las a cartões. Você também pode criar tags para fluxos de trabalho.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 19 de maio de 2023</p>
                            </li>
                            <li>
                                 <p><span class="preview">Versão de produção: 19 de maio de 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Filtros simples disponíveis nas colunas de entrada da placa</a></p>
                        <p>Filtros simplificados foram adicionados à configuração da coluna de entrada para permitir que você defina a coluna de entrada mais rapidamente. Os filtros disponíveis são projetos do Workfront e atribuições por equipe ou usuário. Você pode alternar para os filtros avançados, se preferir.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 10 de maio de 2023<br /></p>
                            </li>
                            <li>
                                 <p>Versão de produção para aceitação antecipada: 10 de maio de 2023 <span style="color: #ff0000;"> Esse recurso está disponível na Produção nesta data somente por meio da aceitação antecipada de recursos para Workfront Boards.</span></p>
                                <p>Versão de produção para todos os clientes: com a versão 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Filtros simples adicionados ao modelo de quadro dinâmico</a></p>
                        <p>Os filtros no modelo de quadro dinâmico foram simplificados para permitir que você crie um quadro mais rapidamente.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 27 de abril de 2023<br /></p>
                            </li>
                            <li>
                                 <p>Versão de produção para aceitação antecipada: 28 de abril de 2023 <span style="color: #ff0000;"> Esse recurso está disponível na Produção nesta data somente por meio da aceitação antecipada de recursos para Workfront Boards.</span></p>
                                <p>Versão de produção para todos os clientes: com a versão 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Modelo de quadro dinâmico</a></p>
                        <p>Um novo modelo, quadro dinâmico, agora está disponível para quadros independentes. Este template não está disponível para quadros dentro de um workflow.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 20 de abril de 2023<br /></p>
                            </li>
                            <li>
                                 <p>Versão de produção para aceitação antecipada: 28 de abril de 2023 <span style="color: #ff0000;"> Esse recurso está disponível na Produção nesta data somente por meio da aceitação antecipada de recursos para Workfront Boards.</span></p>
                                <p>Versão de produção para todos os clientes: com a versão 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Migrar cartões Kanban da Equipe Ágil para Quadros</a></p>
                        <p>Um novo botão <b>Adicionar aos quadros</b> em quadros Kanban de equipes ágeis permite adicionar todos os cartões do quadro Kanban a um quadro Workfront. Você pode optar por criar um novo quadro do Workfront ou adicionar os cartões a um quadro existente.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 20 de abril de 2023<br /></p>
                            </li>
                            <li>
                                 <s><p>Versão de produção para aceitação antecipada: 28 de abril de 2023 <span style="color: #ff0000;"> Esse recurso está disponível na Produção nesta data somente por meio da aceitação antecipada de recursos para Workfront Boards.</span></p></s>
                                 </li>
                                 <li>
                                <p><span class="preview">Versão de produção para todos os clientes: 18 de maio de 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Navegação à esquerda adicionada aos detalhes do cartão em Quadros</a></p>
                        <p>À medida que mais opções de campo são adicionadas aos cartões nas placas Workfront, os detalhes do cartão aumentam. Um novo painel de navegação à esquerda dos detalhes do cartão permite selecionar uma seção e mover-se automaticamente para esse grupo de campos.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 20 de abril de 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Versão de produção para todos os clientes: 27 de abril de 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Preferências e notificações por email dos painéis</a></p>
                        <p>As notificações por email agora estão disponíveis para painéis do Adobe Workfront. As notificações estão ativadas por padrão e você pode selecionar em suas preferências quais emails deseja receber. Você receberá um email quando for adicionado a um quadro e quando um cartão for atribuído a você.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 13 de abril de 2023<br /></p>
                            </li>
                            <li>
                                 <p>Versão de produção para aceitação antecipada: 13 de abril de 2023 <span style="color: #ff0000;"> Esse recurso está disponível na Produção nesta data somente através da aceitação antecipada de recursos para placas Workfront.</p>
                                <p>Versão de produção para todos os clientes: com a versão 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

### Aprimoramentos do Financial Management

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-finance-enhancements.md" class="MCXref xref" xrefformat="{para}">Taxas de custo efetivo e de cobrança</a> por data</p>
                        <p>As taxas de custo e cobrança com data efetiva estão agora disponíveis nos objetos de empresa, usuário e função de trabalho na Workfront. Quando taxas de efetivação de data são aplicadas a um projeto e horas são registradas em tarefas do projeto, os custos e a receita são calculados usando as taxas especificadas para cada período.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 29 de junho de 2023</p>
                            </li>
                            <li>
                                <p>Versão de produção para clientes da versão rápida: a ser anunciada, após a versão de produção 23.3</p>
                                <p>Versão de produção para todos os clientes: a ser anunciada<br>
                                O recurso de substituição de taxa de atribuição foi temporariamente desabilitado na Pré-visualização de 30 de junho a 13 de julho de 2023.</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Nova integração do Google Workspace já disponível</a></p> 
                        <p>Uma nova integração do Google Workspace agora está disponível no Google Marketplace. A nova integração é autenticada usando o OAuth2 e substitui a integração anterior.</p><p>A integração anterior do Google Workspace agora está obsoleta e será automaticamente desinstalada.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: N/D</p>
                            </li>
                            <li>
                                <p><span class="preview">Versão de produção: 27 de junho de 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">As integrações do Adobe Creative Cloud agora oferecem suporte a vários usuários atribuídos</a></p> 
                        <p>A integração do Adobe Creative Cloud agora oferece suporte à capacidade de escolher entre "Concluído com minha parte" e "Concluído" (ou "Resolvido") quando uma tarefa ou problema tiver vários usuários atribuídos.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: N/D</p>
                            </li>
                            <li>
                                <p><span class="preview">Versão de produção: 22 de junho de 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Exibir e gerenciar notificações do Workfront na Workfront para plug-ins do Creative Cloud</a></p> 
                        <p>Para facilitar o recebimento das notificações necessárias, possibilitamos a exibição e o gerenciamento das notificações do Workfront sem sair da Adobe Creative Cloud. Agora, você pode visualizar notificações e acessar os itens de trabalho e comentários relacionados a essas notificações diretamente da janela de plug-in do Workfront no aplicativo do Creative Cloud.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: N/D</p>
                            </li>
                            <li>
                                <p><span class="preview">Versão de produção: 22 de junho de 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
 <!--               <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Improved experience when moving a document to a linked folder with drag and drop</a></p> 
                        <p>We've added some transparency to the process of dragging and dropping a document into a linked folder. Now, the document that you moved to a linked folder remains in the document list until it has fully moved. The document options are disabled, but you can still open the document for view while it is moving. When the document has completed the transfer, it disappears from the document list, because it is now fully located in the linked folder. </p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release: June 7, 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Production release: June 15, 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>-->
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Criar automaticamente pastas vinculadas ao Adobe Experience Manager Assets ao criar um projeto</a></p>
                        <p>Com o novo fluxo de trabalho Criar pasta vinculada para a integração do Adobe Experience Manager, é possível configurar a integração com um caminho para uma pasta do Adobe Experience Manager Assets. Quando a integração é adicionada a um modelo de projeto, qualquer projeto criado a partir do modelo criará automaticamente uma subpasta vinculada no Experience Manager Assets na pasta especificada. </p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 11 de maio de 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Versão de produção: 24 de maio de 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Mapear valores de campo do Workfront para marcas na Experience Manager Assets</a></p>
                        <p>Agora, você pode categorizar e encontrar rapidamente ativos com base em dados da Workfront. Você pode mapear esses dados como parte da configuração de metadados na integração do Workfront para Experience Manager Assets.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 10 de maio de 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Versão de produção: 10 de maio de 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Mapear campos do Workfront para campos de metadados personalizados do Experience Manager Assets</a></p>
                        <p>Com a integração nativa, agora é possível mapear campos nativos e integrados do Workfront para campos de esquema de metadados personalizados no Experience Manager Assets as a Cloud Service.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 10 de maio de 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Versão de produção: 10 de maio de 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Ajuste as configurações do modelo de fluxo de trabalho de prova automática usando o Adobe Workfront para Creative Cloud</a></p>
                        <p>Agora você pode ajustar as configurações existentes do modelo de fluxo de trabalho automatizado diretamente no Creative Cloud.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 27 de abril de 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Versão de produção: 27 de abril de 2023</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Aprovações de novos documentos</a> </p>
                        <p>As aprovações de documentos estão sendo reprojetadas em uma implantação em fases que será disponibilizada para mais usuários com cada versão.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 31 de maio de 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Versão de produção: 14 de junho de 2023</span></p>
                            </li>
                        </ul>
                        <p><span style="color: #ff0000;">Esse recurso faz parte de uma versão em fases e está disponível no momento apenas para clientes específicos.</span></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Novo botão Compartilhar</a> </p>
                        <p>A opção Compartilhar foi retirada do menu Mais para projetos, tarefas e problemas, tornando o compartilhamento mais intuitivo.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 22 de junho de 2023<br /></p>
                            </li>
                            <li>
                                <p>Versão de produção: com a versão 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Melhorias na mobilidade

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-mobile-enhancements.md" class="MCXref xref" xrefformat="{para}">Nova funcionalidade de prova no aplicativo móvel do Workfront</a> </p>
                        <p>Com a descontinuação do aplicativo Workfront Proof independente na versão 23.10 (outubro de 2023), o aplicativo móvel Workfront principal teve recursos de comprovação adicionados para permitir que a comprovação em dispositivos móveis continue.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: N/D</p>
                            </li>
                            <li>
                                <p><span class="preview">Versão de produção: disponível na Apple App Store e na Google Play Store em 21 de junho de 2023</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Nova experiência na Página Inicial</a></p>
                        <p>Para capacitar melhor os usuários de todos os tipos a utilizar o Workfront para suas necessidades específicas, a Página inicial recebeu uma atualização importante! A nova experiência da Página inicial oferece personalização visual e de conteúdo para sua Página inicial, proporcionando flexibilidade para exibir somente as informações mais relevantes ao seu trabalho.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 23 de junho de 2023</p>
                            </li>
                            <li>
                                <p>Versão de produção: com a versão 23.3</p>
                            </li>
                        </ul>
                    </td>
                 </tr>                                 
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Nova experiência de comentários para objetos adicionais</a> </p>
                        <p>A nova experiência de comentários estará disponível para os seguintes objetos, logo após a versão 23.3 para produção: tarefas de modelo, modelos, folhas de horas, equipes, usuários, programas, portfólios.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: a ser anunciada, após a versão de produção 23.3</p>
                            </li>
                            <li>
                                <p>Versão de produção para clientes da versão rápida: a ser anunciada, após a versão de produção 23.3 </p>
                                <p>Versão de produção para todos os clientes: com a versão 23.10 (outubro de 2023)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>                
            <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Nova experiência de comentários do Beta para projetos, tarefas e documentos</a> </p>
                        <p>A nova experiência de comentários no Beta agora está disponível para projetos, tarefas e documentos. Antes desta atualização, a experiência de comentários no Beta estava disponível somente para problemas e metas.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 1 de junho de 2023<br /></p>
                            </li>
                            <li>
                                <p>Versão de produção: com a versão 23.3</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Perfis sem avatares agora exibem as iniciais de usuário</a></p>
                        <p>Para facilitar a localização de usuários específicos em listas grandes, os perfis sem avatares personalizados agora exibem as iniciais do usuário em um plano de fundo colorido em listas e relatórios herdados. Essa é uma pequena alteração cosmética e não se aplica se uma foto de avatar já estiver sendo usada ou se o usuário estiver desativado.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 20 de abril de 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Versão de produção: 4 de maio de 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md" class="MCXref xref" xrefformat="{para}">Novos aprimoramentos na experiência beta de comentários</a></p>
                        <p>As melhorias na seção Atualizações estão sendo disponibilizadas no período da versão 23.3 para a nova experiência de comentário beta. Esses aprimoramentos serão disponibilizados no ambiente de Produção com a versão 23.3, a menos que especificado de outra forma.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: ao longo do período da versão 23.3<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Versão de produção: com a versão 23.3 (salvo especificação em contrário)</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-release-activity.md" class="MCXref xref" xrefformat="{para}">Novos aprimoramentos na experiência do Painel da Tela</a></p>
                        <p>As melhorias no Painel de controle do Canvas estão sendo disponibilizadas no período da versão 23.3. Esses aprimoramentos serão disponibilizados no ambiente de Produção com a versão 23.3, a menos que especificado de outra forma. 
 </p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 5 de junho de 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Versão de produção: 5 de junho de 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Atualizações de aparência durante o período da versão 23.3</a></p>
                        <p>Pequenas atualizações na aparência de várias áreas do aplicativo Adobe Workfront estão sendo feitas dentro do período da versão 23.3. Essas melhorias serão disponibilizadas no ambiente de Produção no mínimo 2 semanas após o lançamento para Pré-visualização.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: ao longo do período da versão 23.3</p>
                            </li>
                            <li>
                                <p><span class="preview">Versão de produção: um mínimo de 2 semanas após o lançamento para Pré-visualização (a menos que especificado de outra forma)</span></p>
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

Novos recursos no Workfront Fusion estão disponíveis na Produção em uma cadência fora da programação de lançamento da versão 23.3. Para obter mais informações sobre os recursos mais recentes, consulte [atividade de versão do Adobe Workfront Fusion](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Aprimoramentos no Planejador de cenários do Workfront

Não há atualizações do Planejador de cenários neste momento na versão. Esta área será atualizada quando houver atualizações disponíveis.

### Aprimoramentos do Workfront Proof

Novos recursos chegando à versão do Workfront Proof dentro do período da versão 23.3. Para obter informações sobre esses novos recursos agora disponíveis na Pré-visualização, consulte [Adobe Workfront Proof com a versão 23.3](/help/quicksilver/product-announcements/product-releases/workfront-proof-release-activity/proof-23-3-release/proof-23-3-overview.md).

### Aprimoramentos das metas do Workfront

Novos recursos chegando à versão do Workfront Goals dentro do período da versão 23.3. Para obter informações sobre esses novos recursos agora disponíveis na Pré-visualização, consulte [Adobe Workfront Goals com a versão 23.3](/help/quicksilver/product-announcements/product-releases/goals-release-activity/goals-23-3-release/goals-23-3-release.md).

### API versão 16

Para a API versão 16, modificamos alguns recursos e endpoints. Algumas das alterações são compatíveis com a nova funcionalidade, enquanto outras facilitam o uso das informações disponíveis por meio da API.

Para obter informações sobre novidades e atualizações, consulte [Novidades na API versão 16](/help/quicksilver/wf-api/api/new-api-version-16.md).

Para obter informações sobre versões de API, consulte [Controle de versão de API e agendamento de suporte](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Atualizações de manutenção do Workfront 

Para obter informações sobre as atualizações de manutenção feitas durante a versão 22.3, consulte [Atualizações de manutenção do Workfront](https://experienceleague.adobe.com/pt-br/docs/workfront-known-issues/releases/current-updates).

### Atualizações de treinamento

Explore as atualizações mais recentes feitas em programas de aprendizado, caminhos de aprendizado, vídeos e guias para cada versão de produto do Adobe Workfront. Para obter mais informações, consulte a seção &quot;Novidades&quot; da [página Tutoriais do Workfront](https://experienceleague.adobe.com/pt-br/docs/workfront-learn/tutorials-workfront/home).

### Funcionalidade que será removida em breve do Workfront

A seguinte funcionalidade será removida do Workfront em breve:

#### Substituição do aplicativo móvel Proof com a versão 23.10 (outubro de 2023)

Descontinuaremos oficialmente o aplicativo móvel Proof com a versão 23.10 (outubro de 2023). O aplicativo móvel geral do Workfront foi aprimorado com a nova funcionalidade de comprovação (consulte a nota de versão em Aprimoramentos do Workfront Mobile para obter mais informações), e os usuários são aconselhados a começar a usá-lo para trabalhos de comprovação o mais rápido possível.

Observe que o aplicativo móvel Workfront requer um logon Workfront. Usuários externos e convidados podem continuar a usar o aplicativo Prova para trabalho de prova; no entanto, ele não é mais compatível e ficará indisponível na versão 23.10 (outubro de 2023).


<!-- HTML you might need

New table

### add product area name

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Feature</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Release dates</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="ADD LINK" class="MCXref xref" xrefformat="{para}">Title</a><span style="color: #ff0000;"> New in Preview!</span></p>
                        <p>Body</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release:<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Production release: </span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

New row for table 

<tr>
  <td>
    <a href="ADD%20LINK">Title</a> New in Preview!
    <p>Body</p>
  </td>
  <td>
    <p><strong>Available on these dates:</strong></p>
    <ul>
      <li>
        <p>Preview release:</p>
      </li>
      <li>
        <p>Production release:</p>
      </li>
    </ul>
  </td>
</tr>


New in preview, prod, and coming soon text

<span style="color: #ff0000;"> New in Preview!</span>
<span style="color: #ff0000;"> New in Production!</span>
<span style="color: #ff0000;"> Coming soon!</span>


Test for boards early access stuff

Production release for early opt-in: March 2, 2023 This feature is available in Production only through the early feature opt-in for Workfront Boards.

Production release for all customers: With the 23.2 release

-->
