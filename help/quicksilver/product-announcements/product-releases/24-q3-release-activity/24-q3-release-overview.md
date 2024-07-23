---
title: Visão geral da versão do terceiro trimestre de 2024
description: Esta página fornece informações sobre a funcionalidade incluída na versão do terceiro trimestre de 2024. Essas melhorias estão planejadas para serem disponibilizadas no ambiente de produção durante todo o trimestre.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 372aa2c2-5deb-49da-aadc-6e870bbd083a
source-git-commit: 76b44f3d5ff7d7747da801a051a457157e08ea4a
workflow-type: tm+mt
source-wordcount: '1849'
ht-degree: 0%

---

# Visão geral da versão do terceiro trimestre de 2024

Esta página fornece informações sobre a funcionalidade incluída na versão do terceiro trimestre de 2024. Essas melhorias estão planejadas para serem disponibilizadas no ambiente de produção durante todo o trimestre.

O webinário de versão 24.7 ao vivo foi cancelado, mas você ainda pode [assistir a uma demonstração em vídeo dos recursos 24.7 aqui](https://video.tv.adobe.com/v/3430532/%20).

<span class="preview">Os recursos fora do ciclo (aqueles que foram lançados para produção antes da data de lançamento do terceiro trimestre de 2024) estão destacados em amarelo.</span>

>[!IMPORTANT]
>
>A versão 23.3 incluía a opção de mover sua organização para versões mensais. Portanto, a Workfront alterou o esquema de numeração de versões para contabilizar as faixas de lançamento mensais e trimestrais. O primeiro número designa o ano e o segundo número significa o mês do lançamento. Exemplo: a versão de abril de 2024 é 24.4.
>
>Os lançamentos mensais e trimestrais devem estar disponíveis na quinta-feira da segunda semana completa do mês, a menos que especificado de outra forma.
>
>| Lançamento mensal | Versão trimestral |
>|----|----|
>| <ul><li>24.5 (16 de maio de 2024)</li><li>24.6 (13 de junho de 2024)</li><li>24.7 (18 de julho de 2024)</li></ul> | <ul><li>24.7 (18 de julho de 2024)</li></ul> |
>
>Para obter mais informações sobre o processo de lançamento rápido, consulte [Habilitar ou desabilitar o processo de lançamento rápido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Aprimoramentos do Adobe Workfront

* [Melhorias do administrador](#administrator-enhancements)
* [Melhorias no gerenciamento financeiro](#financial-management-enhancements)
* [Aprimoramentos de integração](#integration-enhancements)
* [Aprimoramentos do projeto](#project-enhancements)
* [Aprimoramentos de provas](#proofing-enhancements)
* [Melhorias no gerenciamento de recursos](#resource-management-enhancements)
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Regras de negócio agora estão disponíveis</a></p>
                        [!BADGE Na produção ]{type=Informative}
                        <p>Agora, os administradores podem adicionar regras de negócios na área Configuração do Workfront.</p>
                        <p>Uma regra de negócios permite aplicar validação a objetos do Workfront e impede que os usuários criem, editem ou excluam um objeto quando determinadas condições forem atendidas. As regras são criadas usando uma fórmula semelhante aos campos calculados em formulários personalizados.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 4 de julho de 2024</p>
                            </li>
                            <li>
                                <p>Versão de produção para todos os clientes: com a versão 24.7 (18 de julho de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Designer de formulários personalizados geralmente disponível no Adobe Workfront</a></p>
                        [!BADGE Na produção ]{type=Informative}
                        <p>Com a versão 24.7, o designer do formulário estará disponível para o público em geral e se tornará a experiência padrão para criar e editar formulários personalizados no Adobe Workfront. Ao criar um novo formulário personalizado ou abrir um formulário existente, você verá o espaço de trabalho de estilo da tela do designer de formulário.</p>
                        <p>Depois dessa versão, você não terá mais a opção de reverter para o construtor de formulários herdado.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 19 de junho de 2024</p>
                            </li>
                            <li>
                                <p>Versão de produção para todos os clientes: com a versão 24.7 (18 de julho de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Mover objetos entre ambientes Workfront com promoção de ambiente</a></p>
                        [!BADGE Na produção ]{type=Informative}
                        <p>A promoção de ambientes permite mover objetos de um ambiente do Workfront para outro, como de um ambiente de sandbox para um ambiente de produção. Você pode configurar e testar objetos sem qualquer risco para os dados e registros de sua organização. Você pode então mover esses objetos para produção sem precisar reconfigurá-los, economizando tempo e esforço.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de produção para todos os clientes: com a versão 24.6 (13 de junho de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Compartilhar formulários personalizados e campos personalizados no designer de formulários personalizado</a></p>
                        [!BADGE Na produção ]{type=Informative}
                        <p>Agora é possível compartilhar formulários personalizados e campos personalizados com o novo designer de formulário. Isso permite maior colaboração entre usuários em formulários personalizados.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 6 de junho de 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Versão de produção para todos os clientes: 13 de junho</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Adicionar um novo campo personalizado da área Campos</a></p>
                        [!BADGE Na produção ]{type=Informative}
                        <p>Agora é possível adicionar um novo campo ou widget personalizado diretamente na área Campos do Workfront, sem precisar abrir um formulário personalizado para criar o campo. Isso permite criar rapidamente campos personalizados reutilizáveis.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 6 de junho de 2024</p>
                            </li>
                            <li>
                                <p>Versão de produção para todos os clientes: com a versão 24.7 (18 de julho de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Tipo de campo suspenso de seleção múltipla disponível no designer de formulário</a></p>
                        [!BADGE Na produção ]{type=Informative}
                        <p>Para ajudá-lo a definir campos suspensos com mais facilidade, adicionamos o campo suspenso de seleção múltipla ao designer de formulário personalizado. Esse tipo de campo permite que os usuários escolham mais de uma opção em uma lista suspensa.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 4 de junho de 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produção para todos os clientes: 4 de junho de 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Melhorias no gerenciamento financeiro

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Campos de despesas faturáveis e não faturáveis disponíveis para projetos e tarefas</a></p>
                        [!BADGE Na produção ]{type=Informative}
                        <p>Para facilitar a visualização dos tipos de despesas, as despesas foram separadas em despesas faturáveis e não faturáveis em projetos e tarefas. Os seguintes campos estão disponíveis para adição em exibições e relatórios:</p>
                        <ul>
                            <li><p>Custo da despesa planejada e faturável</p></li>
                            <li><p>Custo de Despesas Não Faturáveis Planejadas</p></li>
                            <li><p>Custo Efetivo de Despesas Não Faturáveis</p></li>
                            <li><p>Custo Efetivo de Despesas Não Faturáveis</p></li>
                        </ul>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 10 de maio de 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produção para todos os clientes: 10 de maio de 2024</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Workfront para Experience Manager Assets e melhorias no Assets Essentials</a></p>
                        [!BADGE Na produção ]{type=Informative}
                        <p>Fizemos as seguintes melhorias nas integrações do Workfront para Experience Manager Assets e Assets Essentials:</p>
                        <ul>
                            <li><p>A integração agora é compatível com o GCP como provedor de serviços na nuvem. O AWS e o Azure eram suportados anteriormente.</p></li>
                            <li><p>O limite de tamanho para arquivos enviados para o Experience Manager por meio da integração aumentou para 30 GB. Anteriormente, o limite era de 5 GB.</p></li>
                        </ul>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 27 de junho de 2024</p>
                            </li>
                            <li>
                                <p>Produção para todos os clientes: com a versão 24.7 (18 de julho de 2024)</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Edite a Data de Confirmação e a Condição da tarefa e do problema na seção de cabeçalho ou Detalhes</a></p>
                        [!BADGE Na produção ]{type=Informative}
                        <p>Para facilitar a atualização de tarefas e problemas, adicionamos os campos Data de confirmação e Condição como opções para adicionar à seção Cabeçalhos de tarefas e problemas e Detalhes em um modelo de layout. Os usuários agora podem atualizar esses campos a partir da seção de cabeçalho ou Detalhes de uma página, quando são atribuídos ao modelo de layout modificado.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 30 de maio de 2024</p>
                            </li>
                            <li>
                                <p>Produção para lançamento rápido: com o lançamento do 24.6 (13 de junho de 2024)</p>
                            </li>
                            <li>
                                <p>Versão de produção para todos os clientes: com a versão 24.7 (18 de julho de 2024)</p>
                            </li>
                        </ul>
                        <p><span class="preview">Esse recurso foi removido temporariamente da Produção para clientes que não estão na programação de lançamento rápido.</span></p>
                    </td>
                 </tr>
                   <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Mais atribuições relevantes adicionadas ao fluxo de trabalho Nova Tarefa</a></p>
                        [!BADGE Na produção ]{type=Informative}
                        <p>Adicionamos a mesma funcionalidade para atribuições inteligentes mais relevantes ao campo Atribuições na caixa Nova tarefa ao adicionar uma tarefa a um projeto e em uma lista de tarefas de projeto.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 13 de fevereiro de 2024</p>
                            </li>
                            <li>
                                <p>Produção para lançamento rápido: com o lançamento 24.5 (16 de maio de 2024)</p>
                            </li>
                            <li>
                                <p>Versão de produção para todos os clientes: com a versão 24.7 (18 de julho de 2024)</p>
                            </li>
                        </ul>
                        <p><span class="preview">Este recurso foi removido temporariamente da Produção para clientes que não estão no cronograma de lançamento rápido.</span>&lt;/
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Mais atribuições inteligentes relevantes</a></p>
                        [!BADGE Na produção ]{type=Informative}
                        <p>Alteramos o algoritmo que o Workfront usa para calcular e sugerir atribuições inteligentes para tarefas. O novo algoritmo se aplica às seguintes áreas no Workfront em que você atribui uma tarefa: listas de tarefas, a área Atribuições no cabeçalho da tarefa, Início e o painel Resumo.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 21 de dezembro de 2023</p>
                            </li>
                            <li>
                                <p>Produção para lançamento rápido: com o lançamento 24.5 (16 de maio de 2024)</p>
                            </li>
                            <li>
                                <p>Versão de produção para todos os clientes: com a versão 24.7 (18 de julho de 2024)</p>
                            </li>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Atualizações de segurança para o Visualizador de Revisão de Texto de Área de Trabalho</a></p>
                        [!BADGE Na produção ]{type=Informative}
                        <p>A atualização de segurança do Workfront Proof Desktop Proofing Viewer 2.1.35 fornece correções de bugs de segurança para vulnerabilidades identificadas em versões anteriores.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 4 de julho de 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produção para todos os clientes: 4 de julho de 2024</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-resource-mgmt-enhancements.md">Folga refletida no Balanceador de carga de trabalho</a></p>
                        [!BADGE Na produção ]{type=Informative}
                        <p>Para ajustar facilmente o trabalho quando o destinatário principal em uma tarefa tiver um tempo de folga agendado, o Balanceador de carga de trabalho agora realoca horas para os usuários principal e secundário quando a linha do tempo do projeto é recalculada.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 6 de junho de 2024</p>
                            </li>
                            <li>
                                <p>Versão de produção para todos os clientes: com a versão 24.7 (18 de julho de 2024)</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Alteração de backend para guias no produto</a></p>
                        <p>Estamos implementando uma mudança de tecnologia para nossos guias no produto nas próximas semanas. Embora tenhamos tentado minimizar o impacto dessa transição, alguns usuários podem encontrar guias que já viram.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Produção para todos os clientes: incrementalmente até meados de agosto de 2024</p>
                            </li>
                         </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Experiência unificada de Adobe agora disponível para mais organizações da Workfront</a></p>
                        [!BADGE Na produção ]{type=Informative}
                        <p>Para permitir que as organizações acessem os benefícios da Experiência unificada do Adobe, começamos a disponibilizá-la para os clientes existentes do Workfront. </p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 20 de junho de 2024</p>
                            </li>
                            <li>
                                <p>Produção para clientes especificados: com a versão 24.7 (18 de julho de 2024)</p>
                            </li>
                         </ul>
                         <span style="color: #ff0000;">O Adobe Unified Shell está sendo disponibilizado em uma implantação em fases. Outras organizações serão integradas ao Adobe Unified Shell com as versões 24.10 e 25.1. </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Botão Ajuda removido da barra de navegação principal</a></p>
                        [!BADGE Na produção ]{type=Informative}
                        <p>Para unificar a experiência para usuários que não estão no Unified Shell, o botão Ajuda na barra de navegação principal foi removido. Esse botão, que não está presente para usuários no Unified Shell, vinculava-se à documentação do Workfront e era redundante com um botão de Ajuda semelhante disponível para todos os usuários no Menu principal.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 6 de junho de 2024</p>
                            </li>
                            <li>
                                <p>Versão de produção para todos os clientes: com a versão 24.7 (18 de julho de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Experiência de interface aprimorada para usuários com acesso limitado a objetos</a></p>
                        [!BADGE Na produção ]{type=Informative}
                        <p>Quando um usuário não tem acesso a um objeto, ele verá "Sem acesso" em qualquer lugar que o nome do objeto seja exibido no Workfront. Essa experiência aprimorada também se aplica à API do Workfront.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: 27 de março de 2024</p>
                            </li>
                            <li>
                                <p>Produção para lançamento rápido: com o lançamento 24.5 (16 de maio de 2024)</p>
                            </li>
                            <li>
                                <p>Produção para lançamento trimestral: com a versão 24.7 (18 de julho de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Atualizações de aparência durante o terceiro trimestre de 2024</a></p>
                        <p>Pequenas atualizações na aparência de várias áreas do aplicativo Adobe Workfront estão sendo feitas no período do terceiro trimestre de 2024. Revise as notas de versão individuais para datas de lançamento específicas.</p>
                    </td>
                    <td><p><b>Disponível nas seguintes datas:</b></p>
                        <ul>
                            <li>
                                <p>Versão de pré-visualização: durante todo o período da versão do terceiro trimestre de 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Versão de produção: revise as notas de versão para datas específicas</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
           </tbody>
        </table>

## Anúncios

### Aprimoramentos do Workfront Fusion

Novos recursos do Workfront Fusion estão disponíveis na produção em uma cadência fora da programação de lançamento do terceiro trimestre de 2024. Para obter mais informações sobre os recursos mais recentes, consulte [atividade de versão do Adobe Workfront Fusion](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Aprimoramentos no Planejador de cenários do Workfront

Não há atualizações do Planejador de cenários neste momento na versão. Esta área será atualizada quando houver atualizações disponíveis.

### Aprimoramentos do Workfront Proof

Não há atualizações do Workfront Proof neste momento na versão. Esta área será atualizada quando houver atualizações disponíveis.

### Aprimoramentos das metas do Workfront

Não há atualizações do Workfront Goals neste momento na versão. Esta área será atualizada quando houver atualizações disponíveis.

### API versão 18

Para a API versão 18, modificamos alguns recursos e endpoints. Algumas das alterações são compatíveis com a nova funcionalidade, enquanto outras facilitam o uso das informações disponíveis por meio da API.

Para obter informações sobre novidades e atualizações, consulte [Novidades na API versão 18](/help/quicksilver/wf-api/api/new-api-version-18.md).

Para obter informações sobre versões de API, consulte [Controle de versão de API e agendamento de suporte](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Atualizações de manutenção do Workfront 

Para obter informações sobre as atualizações de manutenção feitas durante a versão do terceiro trimestre de 2024, consulte [Atualizações de manutenção do Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Atualizações de treinamento

Explore as atualizações mais recentes feitas em programas de aprendizado, caminhos de aprendizado, vídeos e guias para cada versão de produto do Adobe Workfront. Para obter mais informações, consulte a seção &quot;Novidades&quot; da [página Tutorials do Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=pt-BR).
