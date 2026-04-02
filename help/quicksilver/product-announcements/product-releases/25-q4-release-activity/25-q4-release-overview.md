---
title: Visão geral da versão do quarto trimestre de 2025
description: Esta página fornece informações sobre a funcionalidade incluída na versão do Quarto trimestre de 2025. Essas melhorias estão previstas para serem disponibilizadas no ambiente de produção ao longo do trimestre.
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 298473d4-7d7d-4401-80bf-899a01f570a6
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '2245'
ht-degree: 39%

---

# Visão geral da versão do quarto trimestre de 2025

Esta página fornece informações sobre a funcionalidade incluída na versão do Quarto trimestre de 2025 programada para outubro de 2025.

As melhorias nesta página estão disponíveis no ambiente de pré-visualização. Esta página será atualizada com melhorias adicionais à medida que a versão do Quarto trimestre de 2025 se aproximar da versão de produção planejada.


<!--
 Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>.
-->

>[!IMPORTANT]
>
>
>As versões mensais e trimestrais estão previstas para serem disponibilizadas na quinta-feira da segunda semana completa do mês, salvo indicação em contrário.
>
>| Versão mensal | Versão trimestral |
>|----|----|
>| <ul><li>25.8 (14 de agosto de 2025)</li><li>25.9 (11 de setembro de 2025)</li><li>25.10 (16 de outubro de 2025)</li></ul> | <ul><li>25.10 (16 de outubro de 2025)</li></ul> |
>
>Observe que, para a versão final de cada trimestre (25.10 neste trimestre), os usuários no cronograma de lançamento rápido receberão a versão um dia antes (quinta-feira, 15 de outubro de 2025).
>
>Para obter mais informações sobre o processo de lançamento rápido, consulte [Habilitar ou desabilitar o processo de lançamento rápido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Aprimoramentos do Adobe Workfront

* [Aprimoramentos do administrador](#administrator-enhancements)
* [Aprimoramentos nos painéis](#dashboards)
* [Aprimoramentos de documento e comprovação](#document-and-proofing-enhancements)
* [Aprimoramentos na página inicial](#home-enhancements)
* [Aprimoramentos de projeto](#project-enhancements)
* [Melhorias no gerenciamento de recursos](#resource-management-enhancements)
* [Aprimoramentos nas solicitações](#requests-enhancements)
* [Outros aprimoramentos](#other-enhancements)

### Aprimoramentos do administrador

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Recurso</strong>
        </td>
        <td><strong>Pré-visualização</strong></td>
        <td><strong>Lançamento rápido</strong></td>
        <td><strong>Trimestralmente</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-admin-and-setup.md" class="MCXref xref" xrefformat="{para}"> Confirmação ao remover um formulário personalizado de um objeto</a><p>[!BADGE Off schedule]{type=Neutral}</p>
            <p>Para garantir que você mantenha o acesso aos dados necessários, adicionamos uma caixa de diálogo de confirmação ao remover um formulário personalizado de um objeto. Remover um formulário personalizado de um objeto remove permanentemente os dados desse formulário do objeto. Agora, a caixa de diálogo permite confirmar que você entende que esses dados serão removidos, garantindo que você não remova os dados necessários. </p>
        </td>
        <td>quinta-feira, 24 de setembro de 2025</td>
        <td>25 de setembro de 2025</td>
        <td>25 de setembro de 2025</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Nova exibição de administrador de painéis</a><p></p>
            <p>A Exibição de administrador dos painéis contém uma lista de todos os painéis na sua conta que os administradores do sistema podem usar para obter um instantâneo rápido dos detalhes gerais dos painéis, incluindo a última atualização, quantos cartões cada um tem e muito mais.</p>
        </td>
        <td>11 de setembro de 2025</td>
        <td>quinta-feira, 15 de outubro de 2025</td>
        <td>sexta-feira, 16 de outubro de 2025</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Habilitar recursos de IA Beta para sua organização</a><p></p>
            <p>Para facilitar a visualização e a influência dos recursos futuros de IA, possibilitamos que você ative as Betas para esses recursos na sua organização. Agora, você pode optar por ativar um ou mais recursos do AI Beta disponíveis atualmente nas Preferências do sistema.</p>
        </td>
        <td>sexta-feira, 28 de agosto de 2025</td>
        <td>11 de setembro de 2025</td>
        <td>sexta-feira, 16 de outubro de 2025</td>
    </tr>     
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Atualizações ao perfil de usuário do Workfront</a><p>[!BADGE Off schedule]{type=Neutral}</p>
            <p>Atualizamos a aparência do perfil de usuário do Workfront para um design moderno consistente com outras áreas do Workfront. Essas atualizações se aplicam a um administrador que edita um único perfil ou que edita em massa vários perfis, ou a um usuário que edita seu próprio perfil.</p>
            <p>Existem algumas pequenas diferenças de funcionalidade em relação ao perfil de usuário atual, incluindo:</p>
            <ul>
                <li>Algumas caixas de seleção (como marcar o usuário como ativo) foram alteradas para alternâncias ou botões.</li>
                <li>A opção "Enviar trabalho que eu atribuir a mim mesmo para minha guia Trabalhando em", em Preferências, foi renomeada para "Definir automaticamente o status da tarefa como Em andamento quando as tarefas forem autoatribuídas" para refletir sua finalidade.</li>
            </ul>
        </td>
        <td>sexta-feira, 28 de agosto de 2025</td>
        <td>Implantação em fases, a partir de 25 de setembro de 2025</td>
        <td>Implantação em fases, a partir de 25 de setembro de 2025</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Adicionar várias opções de valor de uma API externa a um formulário personalizado</a><p></p>
            <p>Um novo tipo de campo, Pesquisa externa de seleção múltipla, agora está disponível no designer de formulário personalizado. Quando os dados são armazenados em um sistema externo, esse tipo de campo permite carregar opções de uma API externa e filtrar com base em outros valores de campo no formulário personalizado. É o mesmo que uma pesquisa externa de seleção única.</p>
            <p>Quando o formulário é adicionado a um objeto, os valores retornados da API são exibidos em um campo suspenso e o usuário pode selecionar vários valores.</p>
        </td>
        <td>sexta-feira, 31 de julho de 2025</td>
        <td>sexta-feira, 14 de agosto de 2025</td>
        <td>sexta-feira, 16 de outubro de 2025</td>
    </tr>     
  </tbody>
</table>

### Aprimoramentos nos painéis

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Recurso</strong>
        </td>
        <td><strong>Pré-visualização</strong></td>
        <td><strong>Lançamento rápido</strong></td>
        <td><strong>Trimestralmente</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-dashboards.md" class="MCXref xref" xrefformat="{para}">Novos Painéis do Canvas abertos beta</a>
            <p>O novo recurso Painéis de tela de desenho ajuda você a visualizar facilmente os dados do Adobe Workfront, adicionando tipos de relatório em uma tela que oferece muitas opções de layout flexíveis, incluindo redimensionamento, arrastar e soltar e muito mais.</p>
        </td>
        <td>quarta-feira, 26 de agosto de 2025</td>
        <td>quarta-feira, 26 de agosto de 2025</td>
        <td>quarta-feira, 26 de agosto de 2025</td>
    </tr> 
</table>

### Aprimoramentos de documento e comprovação

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Recurso</strong>
        </td>
        <td><strong>Pré-visualização</strong></td>
        <td><strong>Lançamento rápido</strong></td>
        <td><strong>Trimestralmente</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-document-and-proof.md" class="MCXref xref" xrefformat="{para}">Implantação em Fases de Aprovações Unificadas</a><p>[!BADGE Off schedule]{type=Neutral}</p>
            <p>Estamos habilitando Aprovações unificadas, anteriormente conhecidas como Novas aprovações de documentos, em uma implantação em fases. Essa funcionalidade será ativada automaticamente na instância do Workfront nos próximos seis meses.</p>
            <p>As Aprovações unificadas substituem as aprovações de documentos herdados e fornecem a nova funcionalidade. 
</p>
        </td>
        <td>Implantação em fases, a partir de 17 de julho de 2025</td>
        <td>Implantação em fases, a partir de 17 de julho de 2025</td>
        <td>Implantação em fases, a partir de 17 de julho de 2025</td>
    </tr> 
  <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-document-and-proof.md" class="MCXref xref" xrefformat="{para}">Novo Revisor da IA do Workfront</a><p></p>
            <p>Observação: no momento, esse recurso está na versão beta.</p>
            <p>O novo Revisor da IA do Workfront ajuda a garantir a conformidade da marca de imagem, revisando automaticamente o conteúdo em relação às diretrizes da sua marca, começando pelas diretrizes de imagem. Ele fornece uma pontuação e feedback acionável para simplificar o processo de aprovação. </p>
            <p>Você pode adicionar o Revisor de IA aos modelos de aprovação ou às solicitações individuais de revisão e aprovação, permitindo uma produção de conteúdo mais rápida e, ao mesmo tempo, mantendo os padrões da marca.</p>
        </td>
        <td>sexta-feira, 14 de agosto de 2025</td>
        <td>sexta-feira, 14 de agosto de 2025</td>
        <td>sexta-feira, 14 de agosto de 2025</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-document-and-proof.md" class="MCXref xref" xrefformat="{para}">Nova integração de prova para o Adobe Express</a><p></p>
            <p>Estamos animados em anunciar uma nova integração entre o Adobe Express e a Workfront Proof.</p>
            <ul>
            <li>Simplifique a colaboração entre as equipes criativa, jurídica e de conformidade para reduzir o tempo de publicação e, ao mesmo tempo, manter a supervisão</li>
            <li>Realizar análises profundas usando marcações de desenho, anotações e comentários com o visualizador do Workfront Proof</li>
            <li>Atenda aos padrões de conformidade corporativa com assinaturas eletrônicas e registros completos de auditoria</li>
            <li>Exigir aprovação em qualquer arquivo remisturado de um modelo da marca Express</li>
            <li>Mapear um modelo expresso para um fluxo de trabalho de revisão e aprovação em vários estágios usando modelos de prova avançados</li>
            </ul>
        </td>
        <td>terça-feira, 28 de julho de 2025</td>
        <td>terça-feira, 28 de julho de 2025</td>
        <td>terça-feira, 28 de julho de 2025</td>
    </tr>     
  </tbody>
</table>

### Aprimoramentos na página inicial

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Recurso</strong>
        </td>
        <td><strong>Pré-visualização</strong></td>
        <td><strong>Lançamento rápido</strong></td>
        <td><strong>Trimestralmente</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-home.md" class="MCXref xref" xrefformat="{para}">Atualizações para o widget Minhas solicitações na Página inicial</a><p></p>
            <p>Para criar uma experiência mais simples entre o Workfront e o Workfront Planning, reprojetamos o widget Minhas solicitações na Página inicial. O novo widget apresenta as seguintes alterações:
            <ul>
                <li>Layout e organização das informações de solicitação aprimorados</li>
                <li>Opções aprimoradas de filtragem e classificação</li>
                <li>Integração com o Workfront Planning para melhorar a visibilidade da alocação de recursos</li>
            </ul>
            </p>
            <p>O novo widget Minhas solicitações exibe somente as solicitações que foram criadas na nova experiência de solicitação.</p>
        </td>
        <td>sexta-feira, 21 de agosto de 2025</td>
        <td>11 de setembro de 2025</td>
        <td>sexta-feira, 16 de outubro de 2025</td>
    </tr>     
  </tbody>
</table>

### Aprimoramentos de projeto

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Recurso</strong>
        </td>
        <td><strong>Pré-visualização</strong></td>
        <td><strong>Lançamento rápido</strong></td>
        <td><strong>Trimestralmente</strong></td>
    </tr>
      <!--
      <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-project.md" class="MCXref xref" xrefformat="{para}">Create project intake forms in Workfront</a>
            <p>To make it easier to create requested projects without converting from issues, we've created Project intake forms. You can configure these intake forms with specific fields, templates, and custom forms, and set approvers for project creation. Then, when a user uses this form, the project is configured to your specifications and sent for approval.</p>
        </td>
        <td>August 21, 2025</td>
        <td>September 11, 2025</td>
        <td>October 16, 2025</td>
    </tr>
    -->
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-project.md" class="MCXref xref" xrefformat="{para}">Novo beta de Integridade do Projeto</a>
            <p>O novo recurso Saúde do projeto utiliza o poder do Assistente de IA para fornecer instantaneamente uma avaliação de como seus projetos estão se saindo e quais áreas precisam de sua atenção.</p>
            <p>O Assistente de IA pode gerar uma avaliação de Integridade do projeto para um projeto, um programa e vários projetos.</p>
        </td>
        <td>11 de setembro de 2025</td>
        <td>11 de setembro de 2025</td>
        <td>11 de setembro de 2025</td>
    </tr> 
  <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-project.md" class="MCXref xref" xrefformat="{para}">Novas expressões adicionadas aos campos de fórmula no Planning e aos campos personalizados calculados no Workfront</a><p><p>[!BADGE Off schedule]{type=Neutral}</p></p>
            <p>Adicionamos novas expressões com o seguinte uso a campos de fórmula no Workfront Planning e a campos personalizados calculados no Workfront:</p>
            <ul>
            <li>REMOVEACCENTS(string): remove as marcas diacríticas de todos os caracteres acentuados na string de entrada.</li>
            <li>REPLACEPATTERN(string, padrão, string de substituição): substitui as correspondências do padrão fornecido pela string de substituição.</li>
            <li>PASCAL(string): converte a string de entrada em PascalCase capitalizando a primeira letra de cada palavra e removendo todos os espaços.</li>
            </ul>
        </td>
        <td>sexta-feira, 7 de agosto de 2025</td>
        <td>sexta-feira, 7 de agosto de 2025</td>
        <td>sexta-feira, 7 de agosto de 2025</td>
    </tr> 
  <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-project.md" class="MCXref xref" xrefformat="{para}">Maneira adicional de acessar Atribuições Avançadas de listas</a><p></p>
            <p>Um botão <b>Avançado</b> agora está disponível para atribuições em listas, agilizando o acesso à página Atribuições avançadas. O ícone <b>Pessoas</b> para acessar as Atribuições Avançadas também está disponível nas atribuições das listas.</p>
        </td>
        <td>sexta-feira, 7 de agosto de 2025</td>
        <td>11 de setembro de 2025</td>
        <td>sexta-feira, 16 de outubro de 2025</td>
    </tr> 
  </tbody>
  </table>

### Melhorias no gerenciamento de recursos

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Recurso</strong>
        </td>
        <td><strong>Pré-visualização</strong></td>
        <td><strong>Lançamento rápido</strong></td>
        <td><strong>Trimestralmente</strong></td>
    </tr>
  <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-resource-mgmt.md" class="MCXref xref" xrefformat="{para}">O Balanceador de carga de trabalho agora está disponível em seu perfil de usuário</a><p></p>
            <p>Todos os usuários agora podem visualizar seus próprios dados de demanda e capacidade no Balanceador de carga de trabalho a partir de seus perfis, independentemente do nível de acesso. Ao acessar o perfil de usuário do Workfront, o Balanceador de carga de trabalho é exibido no painel de navegação esquerdo.</p>
            <p>Os dados do Balanceador de carga de trabalho de um usuário são somente leitura. Não é possível atribuir trabalho, cancelar atribuição de trabalho ou ajustar alocações no nível do usuário.</p>
        </td>
        <td>sexta-feira, 31 de julho de 2025</td>
        <td>sexta-feira, 14 de agosto de 2025</td>
        <td>sexta-feira, 16 de outubro de 2025</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-resource-mgmt.md" class="MCXref xref" xrefformat="{para}">As atribuições de função são exibidas no Balanceador de carga de trabalho </a><p></p>
            <p>Agora, os gerentes de recursos podem revisar as atribuições de funções de trabalho no Balanceador de carga de trabalho. As atribuições são exibidas na área Trabalho não atribuído, sob as tarefas ou problemas aos quais as funções são atribuídas. Somente os itens de trabalho atribuídos aos usuários são exibidos na área Trabalho atribuído. </p>
            <p>Uma nova configuração do Balanceador de carga de trabalho, Mostrar atribuições de função, determina se as atribuições de função são exibidas. A configuração é ativada por padrão.</p>
        </td>
        <td>sexta-feira, 31 de julho de 2025</td>
        <td>sexta-feira, 14 de agosto de 2025</td>
        <td>sexta-feira, 16 de outubro de 2025</td>
    </tr>     
  </tbody>
</table>

### Aprimoramentos nas solicitações

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Recurso</strong>
        </td>
        <td><strong>Pré-visualização</strong></td>
        <td><strong>Lançamento rápido</strong></td>
        <td><strong>Trimestralmente</strong></td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-requests.md" class="MCXref xref" xrefformat="{para}">Criar e salvar exibições na área Solicitações</a><p></p>
            <p>Para facilitar a visualização das informações necessárias, adicionamos a capacidade de criar e salvar exibições na área Solicitações. Agora, você pode salvar uma visualização, incluindo filtros e configurações de coluna, e alternar entre visualizações. Um administrador do Workfront pode adicionar a nova visualização aos modelos de layout.</p>
        </td>
        <td>sexta-feira, 2 de outubro de 2025</td>
        <td>quinta-feira, 15 de outubro de 2025</td>
        <td>sexta-feira, 16 de outubro de 2025</td>
    </tr> 
    <!--
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-requests.md" class="MCXref xref" xrefformat="{para}">New combined Status column in unified Request list</a><p></p>
            <p>To simplify the unified request experience, the Status column now displays both Request Status and Approval Status, whichever applies to a given request.</p>
        </td>
        <td>August 28, 2025</td>
        <td>September 11, 2025</td>
        <td>October 16, 2025</td>
    </tr>
    -->
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-requests.md" class="MCXref xref" xrefformat="{para}">Atualizações para a experiência de Solicitação</a><p></p>
            <p>Para criar uma melhor experiência do usuário ao fazer solicitações no Workfront e no Workfront Planning, atualizamos a experiência de solicitação. Agora é possível:
            <ul>
                <li>Exiba as solicitações do Workfront e do Workfront Planning em uma única lista.</li>
                <li>Filtrar solicitações enviadas com base nos critérios especificados.</li>
                <li>Procure e selecione filas de solicitações do Workfront e formulários do Workfront Planning em uma experiência consolidada.</li>
                <li>Ocultar e reordenar colunas na lista de solicitações enviadas.</li>
            </ul>
            </p>
        </td>
        <td>sexta-feira, 21 de agosto de 2025</td>
        <td>11 de setembro de 2025</td>
        <td>sexta-feira, 16 de outubro de 2025</td>
    </tr>     
  </tbody>
</table>

### Outros aprimoramentos

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>Recurso</strong>
        </td>
        <td><strong>Pré-visualização</strong></td>
        <td><strong>Lançamento rápido</strong></td>
        <td><strong>Trimestralmente</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-other.md" class="MCXref xref" xrefformat="{para}">Adobe Unified Experience agora disponível para mais organizações do Workfront</a><p></p>
            <p>Para permitir que as organizações tenham acesso aos benefícios da Experiência Unificada da Adobe, estamos continuando a disponibilizá-la para clientes do Workfront.</p><p><span style="color: #ff0000;">A Experiência Unificada do Adobe está sendo disponibilizada em uma implantação em fases.</span> </p>
        </td>
        <td><p>11 de setembro de 2025</p><p>Ou</p><p>sexta-feira, 11 de dezembro de 2025</p></td>
        <td><p>sexta-feira, 16 de outubro de 2025</p><p>Ou</p><p>sexta-feira, 15 de janeiro de 2026</p></td>
        <td><p>sexta-feira, 16 de outubro de 2025</p><p>Ou</p><p>sexta-feira, 15 de janeiro de 2026</p></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-other.md" class="MCXref xref" xrefformat="{para}">Atualizações das listas aprimoradas</a><p></p>
            <p>Com o layout de listas avançado, é possível usar filtros e agrupamentos para exibir seu trabalho e mantê-lo melhor organizado. Agora, há um indicador de ponto azul acima de um widget para informar quando um filtro ou agrupamento foi aplicado a uma lista nas seguintes áreas:</p>
            <ul>
                <li>Widget Minhas solicitações</li>
                <li>Prioridades</li>
            </ul>
        </td>
        <td>sexta-feira, 28 de agosto de 2025</td>
        <td>11 de setembro de 2025</td>
        <td>sexta-feira, 16 de outubro de 2025</td>
    </tr>     
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Atualizações de aparência durante o período da versão do quarto trimestre de 2025</a></p>
                        <p>Pequenas atualizações na aparência de várias áreas do aplicativo Adobe Workfront estão sendo feitas dentro do período de lançamento do quarto trimestre de 2025. </p>
                    </td>
                    <td><p>Durante todo o período da versão do quarto trimestre de 2025<br /></p>
                    <td colspan="2"><p>Lançamento rápido: no mínimo uma semana após o lançamento em pré-visualização (a menos que especificado de outra forma)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

<!--
### Functionality soon to be removed from Workfront

* 
-->

## Modernização da interface

Estamos atualizando a interface em todo o Adobe Workfront para melhorar a experiência do usuário e unificá-la com outros aplicativos da Adobe. Essas alterações são lançadas fora do cronograma padrão de lançamento. Para obter uma lista dessas alterações, consulte [Modernização da interface](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

## Notas de versão para outras áreas

### Aprimoramentos do Workfront Fusion

Os novos recursos do Workfront Fusion são disponibilizados em Produção em um ritmo fora do cronograma de lançamentos padrão. Para obter mais informações sobre os recursos mais recentes, consulte [Atividade de lançamento do Adobe Workfront Fusion](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Aprimoramentos do Workfront Planning

Novos recursos no Workfront Planning estão disponíveis em Produção. Para obter mais informações sobre os recursos mais recentes, consulte a [atividade da versão do Quarto Trimestre de 2025 para o Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q4.md).

Ainda não há atualizações para o seguinte nesta versão:

* Planejador de cenários
* Proof
* Metas

## Atualizações do visualizador de prova para desktop

### Versão 2.1.52

**Versão de produção para todos os clientes: 31 de julho de 2025**

O Visualizador de prova para desktop foi atualizado para a versão 2.1.52, que aborda correções de erros.

A atualização 2.1.51 incluiu atualizações internas de ferramentas e não afetou os recursos para o usuário final.

Esta atualização é para Mac e Windows.

## Anúncios

### Nova versão do Workfront para Microsoft Teams

Como a [Microsoft faz a transição para o novo cliente Teams](https://learn.microsoft.com/pt-br/microsoftteams/teams-classic-client-end-of-availability), o cliente Classic Teams não estará mais disponível após 1º de julho de 2025. Para continuar usando o Microsoft Teams e aplicativos integrados como o Workfront, os clientes devem fazer a transição para o novo cliente Teams antes dessa data.

A integração atualizada do Workfront já está disponível e é totalmente compatível com a nova experiência do Teams. Na maioria dos casos, o Workfront aparecerá automaticamente assim que os usuários tiverem feito a transição. Caso contrário, a integração pode ser instalada manualmente a partir da App Store do Microsoft Teams. Para instalar ou verificar a integração do Workfront no novo cliente do Teams, consulte [Instalar [!DNL Adobe Workfront] para Microsoft Teams](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

### Workfront para Microsoft Outlook

[A Microsoft está desativando o suporte para tokens online do Exchange legados](https://learn.microsoft.com/pt-br/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), que atualmente são usados pelo complemento do Workfront Outlook para autenticação. Essa mudança da Microsoft já começou a afetar os clientes e continuará a ser implementada em fases até outubro de 2025.

* **Depois que a Microsoft desativar completamente esses tokens, a integração do Workfront para Microsoft Outlook não funcionará mais.**

Como parte dessa mudança, a Microsoft decidiu alterar a forma como os tokens são habilitados. Após **30 de junho de 2025**, os administradores não poderão mais habilitar os tokens por conta própria — somente o Suporte da Microsoft poderá conceder exceções. **Em 1º de outubro de 2025, os tokens legados serão desativados para todos os locatários. Exceções não serão concedidas.**

### Outras transições de integração do Workfront

Para fornecer integrações mais estáveis e escaláveis, estamos mudando para uma abordagem de integração moderna e flexível usando a Automação e Integração do Workfront (Fusion). Como parte desse processo de transição, as seguintes integrações não estarão disponíveis após **28 de fevereiro de 2026**:

* Workfront para G Suite
* Workfront para Jira
* Workfront para Salesforce.

Recomendamos usar a Automação e Integração do Workfront para as necessidades de integração de sua organização com o Google Workspace.
Para obter uma visão geral da Automação e Integração do Workfront, consulte [Visão geral do Adobe Workfront Fusion](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).

### API versão 20

A versão 20 da API do Workfront foi lançada em segunda-feira, 4 de maio de 2025. Para a versão 20 da API, modificamos alguns recursos e pontos de acesso. Algumas das alterações oferecem suporte a novas funcionalidades, enquanto outras facilitam o uso das informações disponíveis por meio da API.

Para obter informações sobre as novidades e atualizações, consulte [Novidades na versão 20 da API](/help/quicksilver/wf-api/api/new-api-version-19.md).

Para obter informações sobre as versões da API, consulte [controle de versão da API e cronograma de suporte](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Atualizações de manutenção do Workfront

Para obter informações sobre as atualizações de manutenção feitas durante a versão do primeiro trimestre de 2025, consulte [Atualizações de manutenção do Workfront](https://experienceleague.adobe.com/pt-br/docs/workfront-known-issues/releases/current-updates).

### Atualizações de treinamento

Explore as últimas atualizações feitas nos programas de aprendizagem, caminhos de aprendizagem, vídeos e guias para cada versão do Adobe Workfront. Para obter mais informações, consulte a seção &quot;Novidades&quot; da [página de tutoriais do Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=pt-BR).
