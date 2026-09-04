---
title: Melhorias no gerenciamento financeiro do quarto trimestre de 2026
description: Melhorias no gerenciamento financeiro do quarto trimestre de 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 4ca5bba5090d9e3a72c8964bdf6cca1085c314db
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 3%

---

# Melhorias no gerenciamento financeiro do quarto trimestre de 2026

Esta página descreve os aprimoramentos do Financial Management feitos com a versão do Quarto Trimestre de 2026 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de produção, conforme indicado.

Para obter uma lista de todas as alterações disponíveis neste momento do ciclo de lançamento do quarto trimestre de 2026, consulte [Visão geral da versão do quarto trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

## Melhorias nas taxas de cobrança da empresa

>[!NOTE]
>
>Visualização: 3 de setembro de 2026
>Versão rápida de produção: 17 de setembro de 2026
>Produção para todos: 15 de outubro de 2026

Várias atualizações foram feitas na funcionalidade de taxas de cobrança da empresa.

### Para clientes em todos os pacotes de Workfront e Workflow

* Atualizamos as caixas de diálogo para adicionar e editar taxas de cobrança da empresa com um design mais moderno que é consistente com outras áreas do Workfront.
* A configuração &quot;Permitir que taxas de cobrança no nível da empresa substituam taxas de cobrança no nível do projeto&quot; adiciona corretamente as sobreposições de taxa quando uma empresa é adicionada a um projeto, e os cálculos de receita planejada usam taxas de cobrança no nível da empresa.
* Usuários sem acesso a Editar finanças gerais e Editar taxas de cobrança no nível do projeto não podem mais adicionar uma empresa a um projeto.

### Para clientes somente no pacote Workflow Ultimate

Os atributos de tarifa agora estão disponíveis para serem aplicados às taxas de cobrança no nível da empresa. As datas de efetivação também podem ser aplicadas às taxas da empresa.

NOTA: As taxas no nível da empresa não foram adicionadas à hierarquia de taxas.

Para obter mais informações, consulte [Substituir taxas de cobrança de função de trabalho no nível da empresa](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md) e [Substituir taxas de cobrança no nível do projeto por taxas de cobrança no nível da empresa](/help/quicksilver/manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## Agora, as hierarquias de atributo permanecem conectadas automaticamente

>[!NOTE]
>
>Visualização: 3 de setembro de 2026
>Versão rápida de produção: 17 de setembro de 2026
>Produção para todos: 15 de outubro de 2026
>Esse recurso só está disponível para organizações no pacote Workflow Ultimate.

Ao usar atributos de taxa como filtros em várias áreas do Workfront, como Atribuições avançadas, a validação adicional agora é aplicada à filtragem pai-filho.

Anteriormente, se você vinculava um atributo a um pai e esse pai a um avô, o sistema também não reconhecia automaticamente o atributo original como pertencente ao avô. Agora, quando você escolhe o atributo de nível mais baixo, cada nível acima dele é atribuído automaticamente.

Para obter informações sobre atributos, consulte [Definir atributos de taxa](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).
