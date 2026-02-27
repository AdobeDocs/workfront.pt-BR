---
title: Visão geral da versão do segundo trimestre de 2026
description: Esta página fornece informações sobre a funcionalidade incluída na versão do segundo trimestre de 2026. Essas melhorias estão previstas para serem disponibilizadas no ambiente de produção ao longo do trimestre.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7e440fc0-45ad-4f73-ae7e-5374e4ae1480
source-git-commit: b889ba54594275587c97fe3a5073f2e28df97350
workflow-type: tm+mt
source-wordcount: '1169'
ht-degree: 48%

---

# Visão geral da versão do segundo trimestre de 2026

Esta página fornece informações sobre a funcionalidade incluída na versão do Segundo trimestre de 2026 programada para abril de 2026.

As melhorias nesta página estão disponíveis no ambiente de pré-visualização. Esta página será atualizada com melhorias adicionais à medida que a versão do Segundo trimestre de 2026 se aproximar da versão de produção planejada.


<!-- Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>. -->

>[!IMPORTANT]
>
>
>As versões mensais e trimestrais estão previstas para serem disponibilizadas na quinta-feira da segunda semana completa do mês, salvo indicação em contrário.
>
>| Versão mensal | Versão trimestral |
>|----|----|
>| <ul><li>26.2 (12 de fevereiro de 2026)</li><li>26.3 (12 de março de 2026)</li><li>26.4 (15 de abril de 2026)</li></ul> | <ul><li>26.1 (16 de abril de 2026)</li></ul> |
>
>Observe que, para o lançamento final de cada trimestre (26.4 neste trimestre), os usuários no cronograma de lançamento rápido receberão o lançamento um dia antes (15 de abril de 2026).
>
>Para obter mais informações sobre o processo de lançamento rápido, consulte [Habilitar ou desabilitar o processo de lançamento rápido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Aprimoramentos do Adobe Workfront

* [Aprimoramentos do administrador](#administrator-enhancements)
* [Aprimoramentos de documentos](#document-enhancements)
* [Aprimoramentos de projeto](#project-enhancements)
* [Aprimoramentos nos relatórios](#reporting-enhancements)
* [Solicitação de aprimoramentos](#requesting-enhancements)
* [Outros aprimoramentos](#other-enhancements)

### Aprimoramentos do administrador

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
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Recolher seção de formulário personalizado por padrão</a><p>Por padrão, todas as seções em um formulário personalizado são expandidas quando o próprio formulário é expandido. Uma nova opção no designer de formulário personalizado permite marcar uma seção para ser recolhida por padrão quando um usuário abrir o formulário. Essa opção é aplicada no nível da seção, não em campos.</p>
        </td>
        <td><p>quinta-feira, 26 de fevereiro de 2025</p></td>
        <td><p>sexta-feira, 12 de março de 2026</p></td>
        <td><p>sexta-feira, 16 de abril de 2026</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">O tipo de campo Rich Text agora está disponível em formulários personalizados</a><p>O novo tipo de campo <b>Rich text</b> em formulários personalizados é um editor de texto robusto, com opções de formatação como sobrescrito e subscrito, cabeçalhos e tabelas, além das opções tradicionais de negrito, itálico, sublinhado, marcadores, numeração, hiperlinks e aspas duplas. O limite de caracteres permanece de 15.000.</p>
        </td>
        <td><p>sexta-feira, 29 de janeiro de 2026</p></td>
        <td><p>sexta-feira, 12 de fevereiro de 2026</p>
            <p>Esse recurso foi removido temporariamente do ambiente de Produção do em 13 de fevereiro de 2026.</p></td>
        <td><p>A ser definido</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Novos endereços IP para notificações por email do Workfront</a><p></p>
            <p>Estamos atualizando os endereços IP usados para enviar notificações por email do Workfront. Se sua organização mantém um incluo na lista de permissões de email ou firewall, você <b>deve</b> adicionar os novos endereços IP abaixo para garantir a entrega contínua das notificações da Workfront.</p><p>Essas atualizações se aplicam a todos os emails de saída gerados pelo aplicativo do Workfront, incluindo aprovações, lembretes, notificações de prova e outras mensagens do sistema.</p>
            <ul>
            <li>EUA:
            <ul>
            <li>206.55.149.212</li>
            <li>206.55.149.214</li>
            <li>206.55.149.215</li>
            <li>206.55.149.213</li>
            <li>206.55.149.211</li>
            </ul>
            </li>
            <li>UE: 
            <ul>
            <li>24.110.76.224</li>
            <li>24.110.76.223</li>
            </ul>
            </li>
            </ul> </p>
        </td>
        <td><p>sexta-feira, 15 de janeiro de 2026</p></td>
        <td><p>sexta-feira, 15 de janeiro de 2026</p></td>
        <td><p>15 de janeiro de 2026</p></td>
    <tr>
            </tbody>
        </table>

<!--

### Document enhancements

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>Feature</strong>
        </td>
        <td><strong>Preview</strong></td>
        <td><strong>Fast release</strong></td>
        <td><strong>Quarterly</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-documents.md" class="MCXref xref" xrefformat="{para}">Multi‑stage approval workflows available for unified approvals</a><p></p>
            <p>Multi‑stage approval workflows are now available in unified approvals, helping organizations enforce structured, repeatable approval processes that reflect how work is reviewed in the real world. </p>
        </td>
        <td><p>February 26, 2025</p></td>
        <td><p>March 12, 2026</p></td>
        <td><p>April 16, 2026</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-documents.md" class="MCXref xref" xrefformat="{para}">Set up and use multi-stage approval workflow templates</a><p></p>
            <p>You can now configure and reuse multi-stage approval workflow templates, making it easier to apply consistent governance across repeatable approval workflows. </p>
        </td>
        <td><p>February 26, 2025</p></td>
        <td><p>March 12, 2026</p></td>
        <td><p>April 16, 2026</p></td>
    </tr>
             </tbody>
        </table>   

-->

### Aprimoramentos de projeto

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
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-projects.md" class="MCXref xref" xrefformat="{para}">Experiência atualizada com atribuição única ou em massa de tarefas de modelo </a><p>[!BADGE Off schedule]{type=Neutral}</p><p> Atualizamos a seção Atribuições na caixa Editar Tarefas de Modelo ao editar tarefas de modelo único ou editá-las em massa.  </p>
        </td>
        <td><p>sexta-feira, 5 de fevereiro de 2026</p></td>
        <td><p>A partir de 5 de fevereiro de 2026</p></td>
        <td><p>A partir de 5 de fevereiro de 2026</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">Experiência atualizada ao atribuir tarefas únicas ou em massa </a><p>[!BADGE Off schedule]{type=Neutral}</p><p> Atualizamos a seção Atribuições na caixa Editar tarefas ao editar tarefas únicas ou editá-las em massa. </p>
        </td>
        <td><p>terça-feira, 26 de janeiro de 2026</p></td>
        <td><p>A partir de 5 de fevereiro de 2026</p></td>
        <td><p>A partir de 5 de fevereiro de 2026</p></td>
    </tr>
            </tbody>
        </table>

### Aprimoramentos nos relatórios

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
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">Rótulos de campos personalizados exibidos ao criar relatórios</a><p></p>
            <p>O rótulo de campo personalizado agora é exibido antes do nome do campo e do objeto nas ferramentas de criação de relatório, ajudando a localizar campos mais facilmente. Os rótulos de campo também são exibidos ao definir filtros, visualizações e agrupamentos em listas.</p>
        </td>
        <td><p>quinta-feira, 26 de fevereiro de 2025</p></td>
        <td><p>sexta-feira, 12 de março de 2026</p></td>
        <td><p>sexta-feira, 16 de abril de 2026</p></td>
    </tr>
   <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">Pastas de Relatórios Compartilháveis</a><p></p>
            <p>Agora é possível organizar e compartilhar relatórios usando pastas de relatórios compartilháveis. Esse novo recurso ajuda as equipes que gerenciam grandes volumes de relatórios a manter um controle de acesso escalável e consistente.</p>
        </td>
        <td><p>quinta-feira, 26 de fevereiro de 2025</p></td>
        <td><p>sexta-feira, 12 de março de 2026</p></td>
        <td><p>sexta-feira, 16 de abril de 2026</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">Rótulos de data aprimorados para agrupamentos de gráfico em painéis da tela</a><p></p>
            <p>Os gráficos que agrupam dados por data agora exibem rótulos de data mais claros e legíveis. Com essa atualização, os rótulos de data se ajustam dinamicamente com base na opção Agrupar por selecionada (como dia, semana, mês ou ano), facilitando a leitura e a interpretação rápidas dos gráficos.</p><p>Observação: o Canvas Dashboards está atualmente na versão beta.</p>
        </td>
        <td><p>quinta-feira, 26 de fevereiro de 2025</p></td>
        <td><p>sexta-feira, 12 de março de 2026</p></td>
        <td><p>sexta-feira, 16 de abril de 2026</p></td>
    </tr>
             </tbody>
        </table>

### Solicitação de aprimoramentos

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
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-requests.md" class="MCXref xref" xrefformat="{para}">Atualização da experiência de compartilhamento para exibições aprimoradas</a><p></p>
            <p>Na área Novas solicitações, ao compartilhar uma exibição aprimorada com um usuário e conceder a ele permissões de exibição, o usuário poderá modificar os elementos de exibição e essas alterações serão salvas nas preferências pessoais do usuário. Agora, eles têm a opção de salvar uma cópia da exibição que inclui suas alterações ou redefinir a exibição compartilhada para suas configurações originais. Eles podem compartilhar ainda mais a visualização copiada com outras pessoas. </p>
        </td>
           <td><p>quinta-feira, 26 de fevereiro de 2025</p></td>
        <td><p>sexta-feira, 12 de março de 2026</p></td>
        <td><p>sexta-feira, 16 de abril de 2026</p></td>
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
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-other.md" class="MCXref xref" xrefformat="{para}">Adobe Unified Experience agora disponível para mais organizações do Workfront</a><p></p>
            <p>Para permitir que as organizações tenham acesso aos benefícios da Experiência Unificada da Adobe, estamos continuando a disponibilizá-la para clientes do Workfront.</p>
        </td>
        <td><p>sexta-feira, 11 de dezembro de 2025</p></td>
        <td><p>quinta-feira, 11 de fevereiro de 2026</p></td>
        <td><p>quinta-feira, 11 de fevereiro de 2026</p></td>
    </tr>
            </tbody>
        </table>


<!--### Functionality soon to be removed from Workfront-->

<!--

## Interface modernization

We are updating the interface throughout Adobe Workfront to improve the user experience and unify it with other Adobe applications. These changes are released outside the standard release schedule. For a list of these changes, see [Interface Modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

-->

## Notas de versão para outras áreas

### Aprimoramentos do Workfront Fusion

Os novos recursos do Workfront Fusion são disponibilizados em Produção em um ritmo fora do cronograma de lançamentos padrão. Para obter mais informações sobre os recursos mais recentes, consulte [Atividade de lançamento do Adobe Workfront Fusion](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Aprimoramentos do Workfront Planning

Novos recursos no Workfront Planning estão disponíveis em Produção. Para obter mais informações sobre os recursos mais recentes, consulte a [atividade da versão do Segundo Trimestre de 2026 para o Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-26-q2.md).

Ainda não há atualizações para o seguinte nesta versão:

* Planejador de cenários
* Proof
* Metas

## Atualizações do visualizador de prova para desktop

### Versão 2.1.54

**Lançamento de produção para todos os clientes: 11 de dezembro de 2025**

O Visualizador de prova para desktop foi atualizado da versão 2.1.52 para a 2.1.54. Essa atualização incluiu melhorias internas nas ferramentas e não impactou os recursos para o usuário final.

A versão 2.1.53 também incluiu alterações internas nas ferramentas.

Esta atualização é para Mac e Windows.

## Avisos

### API versão 21

A versão 21 da API do Workfront foi lançada em 23 de outubro de 2025. Para a versão 21 da API, modificamos alguns recursos e pontos de acesso. Algumas das alterações oferecem suporte a novas funcionalidades, enquanto outras facilitam o uso das informações disponíveis por meio da API.

>[!IMPORTANT]
>
>Esta alteração na versão da API apresenta uma mudança significativa que pode afetar suas chamadas de API. Isso se deve ao fato de que a versão 21 da API usa a versão 2 das assinaturas de eventos.
>
> Para campos de seleção múltipla, a versão 2 das Assinaturas de evento sempre envia como matriz. A versão 1 enviava uma matriz se mais de um valor fosse selecionado. Se apenas um valor fosse selecionado, ela enviaria uma string.

Para obter informações sobre as novidades e atualizações, consulte [Novidades na versão 21 da API](/help/quicksilver/wf-api/api/new-api-version-21.md).

Para obter informações sobre as versões da API, consulte [controle de versão da API e cronograma de suporte](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Outras transições de integração do Workfront

Para fornecer integrações mais estáveis e escaláveis, estamos mudando para uma abordagem de integração moderna e flexível usando a Automação e Integração do Workfront (Fusion). Como parte desse processo de transição, as seguintes integrações não estarão disponíveis após **28 de fevereiro de 2026**:

* Workfront para G Suite
* Workfront para Jira
* Workfront para Salesforce.

Recomendamos usar a Automação e Integração do Workfront para as necessidades de integração de sua organização com o Google Workspace.
Para obter uma visão geral da Automação e Integração do Workfront, consulte [Visão geral do Adobe Workfront Fusion](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).


### Atualizações de manutenção do Workfront

Para obter informações sobre as atualizações de manutenção feitas durante a versão do Segundo trimestre de 2025, consulte [Atualizações de manutenção do Workfront](https://experienceleague.adobe.com/pt-br/docs/workfront-known-issues/releases/current-updates).

### Atualizações de treinamento

Explore as últimas atualizações feitas nos programas de aprendizagem, caminhos de aprendizagem, vídeos e guias para cada versão do Adobe Workfront. Para obter mais informações, consulte a seção &quot;Novidades&quot; da [página de tutoriais do Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=pt-BR).
