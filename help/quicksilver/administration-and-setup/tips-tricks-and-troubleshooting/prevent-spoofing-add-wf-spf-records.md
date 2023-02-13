---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Evitar falsificação e adicionar [!DNL Adobe Workfront] Registros SPF
description: Se os usuários não estiverem recebendo [!DNL Adobe Workfront] notificações por email, é necessário adicionar [!DNL Workfront] Registros SPF no firewall. Você deve trabalhar com a equipe de TI para adicionar registros SPF.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# Evitar falsificação e adicionar [!DNL Adobe Workfront] Registros SPF

## Problema

Se os usuários não estiverem recebendo [!DNL Adobe Workfront] notificações por email, é necessário adicionar [!DNL Workfront] Registros SPF no firewall. Você deve trabalhar com a equipe de TI para adicionar registros SPF.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador. Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> <p><b>OBSERVAÇÃO</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solução

Se você já tiver adicionado os endereços IP à sua lista de permissões de  pelo ambiente de produção, conforme descrito em [Configurar a  lista de permissões do firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) Os usuários do e do ainda não estão recebendo emails:

1. Adicione o seguinte registro SPF ao firewall:

   *spf.workfront.com*

   Isso adiciona automaticamente tudo [!DNL Workfront] Endereços IP à sua listas de permissões no firewall e permitem que todos os filtros de spam (que usam registros SPF) validem [!DNL Workfront] servidores como remetentes válidos para o seu domínio.

   >[!NOTE]
   >
   > Um registro SPF é um registro TXT que faz parte de um arquivo de zona DNS. Não oferecemos suporte à modificação do arquivo de zona DNS.

1. Você deve especificar o tipo de registro SPF que precisa ser configurado. Esses são os tipos válidos de registros SPF:

   * todos (https://dmarcian.com/spf-syntax-table/#all)
   * ip4 (https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6 (https://dmarcian.com/spf-syntax-table/#ip6)
   * a (https://dmarcian.com/spf-syntax-table/#a)
   * mx (https://dmarcian.com/spf-syntax-table/#mx)
   * ptr (https://dmarcian.com/spf-syntax-table/#ptr)
   * existe (https://dmarcian.com/spf-syntax-table/#exists)
   * incluir (https://dmarcian.com/spf-syntax-table/#include)

   Por exemplo, &quot;v=spf1 a mx inclui: [spf.workfront.com](http://spf.workfront.com/) -all&quot;

Se não conseguir adicionar registros SPF ao firewall devido à política da empresa, trabalhe com a [!DNL Workfront] Representante de suporte.
