---
title: Exportar a página de registro
description: É possível exportar a página de visualização ou de detalhes de um registro do Adobe Workfront Planning para um arquivo do Microsoft Word.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8de68b70-dd87-4aad-9137-980ea9fc0d69
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 1%

---

# Exportar os detalhes de um registro

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ele está disponível somente no ambiente de Pré-visualização para todos os clientes ou no ambiente de Produção para clientes que habilitaram versões rápidas.</span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>


Para colaborar de forma mais eficiente com outras pessoas que talvez não tenham uma conta do Workfront, é possível exportar a página de detalhes de um registro para um arquivo do Microsoft Word e compartilhá-la com elas.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produtos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planejamento do Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>plano do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer um dos seguintes planos da Workfront:</p> 
<ul><li>Selecionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>O Workfront Planning não está disponível para planos herdados do Workfront</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Pacote de planejamento do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer </p> 
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td> 
   <td> 
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar todos os recursos do Workfront Planning.</p> 
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada da Adobe para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td> 
   <td> <p>Padrão</p>
   <p>O Workfront Planning não está disponível para licenças herdadas do Workfront</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Exibir ou aumentar permissões para um espaço de trabalho <span class="preview">e tipo de registro</span></a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modelo de layout</p></td> 
   <td> <p>No ambiente de Produção, todos os usuários, inclusive os Administradores do Sistema, devem ser atribuídos a um modelo de layout que inclua o Planning.</p>
<p><span class="preview">No ambiente de Pré-visualização, os usuários do Standard e os administradores do sistema têm o Planning habilitado por padrão.</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Considerações sobre a exportação de detalhes de um registro:

* É possível exportar os detalhes de um registro para os seguintes formatos de arquivo:

   * .docx Word
   * .pdf

* Você pode exportar somente a guia Detalhes da página ou da área de visualização de um registro.

* O arquivo exportado preserva o layout da página de registro, incluindo a miniatura e as imagens de capa.

## Exportar os detalhes de um registro

{{step1-to-planning}}

1. Clique no cartão de um espaço de trabalho.

   O espaço de trabalho é aberto e os tipos de registro são exibidos em cartões.

1. Clique em um cartão de tipo de registro.
A página de tipo de registro é aberta e todos os registros desse tipo são exibidos.

1. Em qualquer exibição, clique no nome de um registro.

   A caixa de visualização do registro é aberta.

1. (Opcional) Clique no ícone **Abrir em nova guia** ![Abrir detalhes em um novo ícone de guia](assets/open-details-in-a-new-tab-icon.png) para abrir a página do registro.

1. Escolha a guia **Detalhes**. A guia Detalhes deve ser aberta por padrão.

1. Clique no menu **Exportar** ![ícone Exportar na página de detalhes do registro](assets/export-icon-in-record-details-page.png), na visualização ou na página do registro, e clique em uma das seguintes opções:

   * **Microsoft Word**
   * **Adobe PDF**

   Um arquivo do Word (.docx) ou PDF é baixado e salvo no computador.

   O nome do arquivo exportado é o campo Primary do registro.

   ![Arquivo Word exportado](assets/exported-word-file.png)

   >[!NOTE]
   >
   >    As informações adicionais que não são exibidas na página e só são visíveis depois de clicar em Mostrar mais na área de detalhes do registro não são exibidas no arquivo PDF exportado. Somente as informações visíveis na página são exibidas no arquivo exportado.


1. (Opcional) Vá para o arquivo baixado, abra-o e edite-o (se for um arquivo do Word) ou compartilhe-o com outras pessoas.

