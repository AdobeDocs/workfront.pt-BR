---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Impedir falsificação e adicionar [!DNL Adobe Workfront] registros SPF
description: Se os usuários não estiverem recebendo  [!DNL Adobe Workfront] notificações por email, será necessário adicionar  [!DNL Workfront] registros SPF ao firewall. Você deve trabalhar com sua equipe de TI para adicionar registros SPF.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# Impedir falsificação e adicionar [!DNL Adobe Workfront] registros SPF

## Problema

Se os usuários não estiverem recebendo notificações por email do [!DNL Adobe Workfront], será necessário adicionar [!DNL Workfront] registros SPF ao firewall. Você deve trabalhar com sua equipe de TI para adicionar registros SPF.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador [!DNL Workfront]. Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a um usuário acesso administrativo total</a>.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solução

Se você já tiver adicionado os endereços IP ao arquivo de produção, conforme descrito em [Configurar o arquivo de incluir na lista de permissões inclui na lista de permissões do firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md), e os usuários ainda não estiverem recebendo emails:

1. Adicione o seguinte registro SPF ao firewall:

   *spf.workfront.com*

   Isso adiciona automaticamente todos os endereços IP do [!DNL Workfront] à sua inclui na lista de permissões do  no firewall e permite que todos os filtros de spam (que usam registros SPF) validem servidores do [!DNL Workfront] como remetentes válidos para seu domínio.

   >[!NOTE]
   >
   > Um registro SPF é um registro TXT que faz parte de um arquivo de zona DNS. Não oferecemos suporte à modificação do arquivo de zona DNS.

1. Você deve especificar o tipo de registro SPF que precisa ser configurado. Estes são os tipos válidos de registros SPF:

   * todos (https://dmarcian.com/spf-syntax-table/#all)
   * ip4 (https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6 (https://dmarcian.com/spf-syntax-table/#ip6)
   * a (https://dmarcian.com/spf-syntax-table/#a)
   * mx (https://dmarcian.com/spf-syntax-table/#mx)
   * ptr (https://dmarcian.com/spf-syntax-table/#ptr)
   * existe (https://dmarcian.com/spf-syntax-table/#exists)
   * incluir (https://dmarcian.com/spf-syntax-table/#include)

   Por exemplo, &quot;v=spf1 a mx include: spf.workfront.com -all&quot;

Se você não puder adicionar registros SPF ao firewall devido à política da empresa, entre em contato com o representante de suporte do [!DNL Workfront].
