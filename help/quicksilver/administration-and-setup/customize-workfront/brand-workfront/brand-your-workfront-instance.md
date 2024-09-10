---
title: Marque sua instância do Adobe Workfront
user-type: administrator
product-area: system-administration
navigation-topic: brand-workfront
description: Como administrador do Workfront, você pode marcar o Workfront com logotipos na tela de logon, na área de navegação superior e no menu principal. Você também pode alterar a imagem de fundo e a cor da tela de logon.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 94603393-bdea-4673-9256-08da14f6916e
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 1%

---

# Marque sua instância do Adobe Workfront

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

>[!IMPORTANT]
>
>O procedimento descrito nesta página aplica-se apenas a organizações que ainda não foram integradas no [!DNL Adobe Experience Cloud].
>
> Se sua organização foi integrada ao [!DNL Adobe Experience Cloud], a identidade visual não está disponível.

Como administrador do Workfront, você pode marcar o Workfront com logotipos nos seguintes locais:

* Tela de login

  ![](assets/brand-login-screen-nwe-adobe.jpg)

* Área de navegação superior

  ![](assets/brand-top-nav-area-nwe-adobe.jpg)

* Menu principal

  ![](assets/brand-main-menu-adobe.jpg)

Você também pode alterar a imagem de fundo e a cor da tela de logon:

![](assets/wf_banner_on_login_screen-adobe.png)

>[!NOTE]
>
>* A alteração da imagem e da cor de fundo do logon não estará disponível se a instância do Workfront da sua organização usar um portal de SSO personalizado. Consulte o administrador de rede ou de TI se precisar de mais informações.
><!--
>or is enabled with Adobe IMS  >
>  >
>-->
>
>* Um administrador ou administrador de grupo do Workfront também pode marcar o Workfront para determinados grupos e usuários usando um modelo de layout. A marca em um modelo de layout substitui a marca no nível do sistema explicada neste artigo. Para obter instruções sobre a identidade visual em um modelo de layout, consulte [Brand Adobe Workfront usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p>
       <p>Ou</p>
       <p>Atual: Plano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Marca a tela de logon

{{step-1-to-setup}}

1. Clique em **Sistema** > **Identidade Visual**.

1. Faça qualquer uma das alterações a seguir para personalizar o Workfront com suas imagens de marca.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Marque o ícone Início <span style="font-weight: normal;"> (exibido na extremidade esquerda da área de navegação superior)</span></p> </td> 
      <td> <p>Na seção <strong>Área de navegação superior</strong>, em <strong>Ícone da página inicial</strong>, clique em qualquer lugar na caixa, localize e selecione a imagem do logotipo. Ou arraste uma imagem para a caixa.</p> <p>Para recortar a imagem, use os controles de rolagem e arraste a imagem para a posição desejada dentro do espaço prescrito.</p> <p>Recomendamos uma imagem de 120 x 120. Pode estar em qualquer um dos seguintes formatos: GIF, JPG, PNG, SVG.</p> <p>Esse ícone também aparece em relatórios, listas, painéis e relatórios entregues que os usuários exportam como arquivos PDF.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Marque o logotipo <span style="font-weight: normal;"> do Menu Principal <img src="assets/main-menu-icon.png"> (exibido no canto superior direito do Menu Principal)</span></p> </td> 
      <td> <p>Na seção <strong>Área de navegação superior</strong>, em <strong>Logotipo do menu principal</strong>, clique em qualquer lugar na caixa, localize e selecione a imagem do logotipo. Ou arraste uma imagem para a caixa.</p> <p>Para recortar a imagem, use os controles de rolagem e arraste a imagem para a posição desejada dentro do espaço prescrito.</p> <p>Recomendamos uma imagem de 300 x 120 pixels. Pode estar em qualquer um dos seguintes formatos: GIF, JPG, PNG, SVG.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Marque o logotipo da tela de logon <span style="font-weight: normal;"> (exibido na parte superior esquerda da caixa onde os usuários digitam as credenciais de logon)</span></td> 
      <td> <p>Em <strong>Tela de Login</strong>, clique em qualquer lugar na caixa, localize e selecione a imagem do seu logotipo. Para recortar a imagem, use os controles de rolagem e arraste a imagem para a posição desejada dentro do espaço prescrito.</p> <p>Recomendamos uma imagem de 300 x 120 pixels. Pode estar em qualquer um dos seguintes formatos: GIF, JPG, PNG, SVG.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Marque a cor de fundo da tela de logon <span style="font-weight: normal;"> (exibida atrás da caixa onde os usuários digitam as credenciais de logon)</span></td> 
      <td> <p>Em <strong>Tela de Login</strong>, defina uma <strong>Cor do Plano de Fundo</strong>. </p> <p>Você pode usar códigos de cor RGB ou HEX.</p> <p>A cor do plano de fundo só estará visível se o plano de fundo da tela de logon for maior que a imagem do plano de fundo da tela de logon (consulte a próxima linha desta tabela) ou se houver alguma transparência na imagem.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Marque a imagem de fundo da tela de logon <span style="font-weight: normal;"> (exibida atrás da caixa onde os usuários digitam suas credenciais de logon)</span></td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1"> <p> Na área <strong>Tela de Login</strong>, em <strong>Imagem de Fundo</strong>, clique na caixa, localize e selecione sua imagem ou imagens JPG ou PNG (até 20 ). </p> <p>Várias imagens de fundo são exibidas em ordem aleatória, alterando cada vez que os usuários atualizam suas páginas de logon. Recomendamos imagens com no máximo 2 MB.</p> </li> 
        <li value="2"> <p>Passe o mouse sobre cada imagem de fundo carregada, clique no ícone Configurações (engrenagem) e use uma das seguintes opções para especificar onde e como você deseja que a imagem apareça no plano de fundo da tela de logon:</p> 
         <ul> 
          <li> <p><strong>Tela cheia</strong>: ajusta a imagem para o plano de fundo da tela de logon, o que pode aumentar a imagem. Use uma imagem de alta resolução (até 2 MB) para obter melhores resultados.</p> <p>Quando você usa essa opção, o banner do Workfront, que não é personalizável, obscurece parte da imagem.</p> </li> 
          <li> <p><strong>Bloco</strong>: divide a imagem lado a lado na área de plano de fundo da tela de logon, em seu tamanho original. Isso é útil para criar um padrão. Selecione uma opção de alinhamento azul para iniciar a divisão em blocos gráficos a partir do canto superior esquerdo, do centro superior ou do canto superior direito da área do plano de fundo.</p> </li> 
          <li> <p><strong>Posição</strong>: coloca a imagem no tamanho original na posição escolhida usando uma das opções de alinhamento azul: parte superior esquerda, parte superior central ou parte superior direita da área de fundo da tela de logon.</p> <p>A cor do plano de fundo preenche o restante da área de plano de fundo da tela de logon. Para obter mais informações sobre a cor do plano de fundo, consulte a linha anterior nesta tabela.</p> </li> 
         </ul> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Redefinir para a identidade visual padrão</td> 
      <td> <p>A redefinição da identidade visual padrão exclui todas as fotos e imagens carregadas.</p> <p>Clique em <strong>Redefinir todas as marcas para os padrões da Workfront</strong> no canto inferior direito da tela e em <strong>Sim</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Isso não estará disponível se a instância Workfront da sua organização usar um portal SSO personalizado.
   ><!--   >
   >or is enabled with Adobe IMS   >
   >   >
   >-->
   >
   >Consulte o administrador de rede ou de TI se precisar de mais informações.

1. Clique em **Salvar**.
