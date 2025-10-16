---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Impedir Falsificação e Adicionar [!DNL Adobe Workfront] Registros SPF
description: Se os usuários não estiverem recebendo  [!DNL Adobe Workfront] notificações por email, será necessário adicionar  [!DNL Workfront] registros SPF ao firewall. Você deve trabalhar com sua equipe de TI para adicionar registros SPF.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 1%

---

# Impedir falsificação e adicionar [!DNL Adobe Workfront] registros SPF

## Problema

Se os usuários não estiverem recebendo notificações por email do [!DNL Adobe Workfront], será necessário adicionar [!DNL Workfront] registros SPF ao firewall. Você deve trabalhar com sua equipe de TI para adicionar registros SPF.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacote</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licença</td> 
   <td><p>Standard</p>
       <p>Plano</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
