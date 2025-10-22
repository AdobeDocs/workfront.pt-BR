---
content-type: reference
navigation-topic: get-started-with-workfront
title: Preparação para a HIPAA para o Workfront
description: Um cliente da Workfront que seja, conforme definido na HIPAA, um Associado comercial e/ou a Entidade coberta em cujo nome o Associado comercial fornece a Adobe Workfront deve usar as diretrizes a seguir para configurar o Workfront para uso pronto para a HIPAA.
feature: Get Started with Workfront
author: Courtney
exl-id: e3cdaa03-d523-46a4-954b-8456d5f190e4
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Preparação para a HIPAA para o Workfront

Um cliente da Workfront que seja, conforme definido na HIPAA, um Associado comercial e/ou a Entidade coberta em cujo nome o Associado comercial fornece a Adobe Workfront deve usar as seguintes diretrizes para configurar o Workfront para uso Pronto para HIPAA:


## Requisitos de senha

| **Configuração de Segurança** | **O Que É?** | **Requisito** |
|----------------------|------------------|------------------|
| Força mínima de senha para contratos | Qual é a força mínima para senhas de contrato? | Não menos de 8 caracteres |
| Força mínima de senha para senhas de usuário | Qual é a força mínima para as senhas dos usuários? | Caracteres de três das seguintes categorias:<br> Letras maiúsculas (alfabeto latino)<br> Letras minúsculas (alfabeto latino)<br> Dígitos de base 10<br> Caracteres não alfanuméricos |
| Duração da senha | Por quanto tempo as senhas devem permanecer inalteradas? | As senhas devem ser alteradas pelo menos a cada 90 dias |
| Histórico de senhas | Quantas senhas passadas devem ser lembradas e não permitidas? | Não inferior a 5 |


## Requisitos de logon

| **Configuração de Segurança** | **O Que É?** | **Requisito** |
|----------------------|------------------|------------------|
| Máximo de falhas de logon | Quantas tentativas de login com falha fazem com que o usuário seja bloqueado? | Não mais de 5 tentativas em um período de 5 minutos; nova tentativa permitida após 30 minutos |
| Máximo de Falhas de Verificação de SSO | Quantas tentativas de verificação de SSO com falha causam um bloqueio? | Não superior a 5 (aplica-se somente a clientes que usam SSO) |


## Requisitos da sessão

| **Configuração de Segurança** | **O Que É?** | **Requisito** |
|----------------------|------------------|------------------|
| Tempo limite da sessão | Quantos minutos de inatividade causam logout? | Não mais de 15 minutos |

## Responsabilidades do cliente

Garantir que todos os funcionários, representantes e/ou agentes conheçam e compreendam os termos dos contratos de licenciamento e/ou serviço assinados entre as partes, conforme aplicável, relevantes para o uso de dados com a Workfront.

Em especial, as seguintes responsabilidades e obrigações devem ser revistas e comunicadas: 

* O cliente é responsável pelo uso do Serviço Workfront por todos os usuários. 

* O cliente deve cumprir todos os termos de seu contrato com a Adobe, que inclui a proibição de upload de elementos de dados no Workfront. 

* Qualquer dado confidencial, incluindo, mas não limitado a, ePHI, é carregado por conta e risco do cliente.  O cliente é sempre responsável por todos os dados do cliente. 


## Proteção de dados e conformidade

>[!IMPORTANT]
>
>O Workfront não foi projetado para ser um repositório de registros eletrônicos de saúde (EHRs). A ePHI só poderá ser processada se expressamente autorizada por escrito pela Adobe. 

* Para qualquer banco de dados do Workfront em que ePHI possa ser acessado, verifique se **a Criptografia em repouso (EAR)** está habilitada.
   * Entre em contato com o Executivo de conta (AE) para verificar se o EAR está incluído em sua compra da Workfront.
   * Configurar sistemas/bancos de dados acessíveis por meio do Workfront para atender às obrigações de conformidade.
* Certifique-se de que a ePHI não seja transferida, vinculada ou compartilhada com outras soluções da Adobe que não sejam prontas para HIPAA.
* Garantir que as fotografias dos pacientes processadas via Workfront sejam armazenadas de forma segura e não estejam acessíveis publicamente.
