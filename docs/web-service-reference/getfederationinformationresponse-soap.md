---
title: GetFederationInformationResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2033c14f-dcc8-43c2-9fd9-a51946ec7055
description: GetFederationInformationResponse 要素には、GetFederationInformation (SOAP) の操作の応答が含まれています。
ms.openlocfilehash: 28b002b45968278ad4c7160b4eed29721422646d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760730"
---
# <a name="getfederationinformationresponse-soap"></a>GetFederationInformationResponse (SOAP)

**GetFederationInformationResponse**要素には、 [GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)の応答が含まれています。 
  
```XML
<GetFederationInformationResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <TokenIssuers/>
   <ApplicationUri/>
   <Domains/>
</GetFederationInformationResponse>
```

 **GetFederationInformationResponse**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[エラー コード (SOAP)](errorcode-soap.md) <br/> |自動検出サービスによって返されるエラー コードを表します。  <br/> |
|[エラー メッセージ (SOAP)](errormessage-soap.md) <br/> |自動検出サービスによって返されるエラー コードに関連付けられているメッセージを表します。  <br/> |
|[ApplicationUri (SOAP)](applicationuri-soap.md) <br/> |アプリケーションの場所を定義します。  <br/> |
|[TokenIssuers (SOAP)](tokenissuers-soap.md) <br/> |セキュリティ トークン サービスの識別子は、エンドポイントが含まれているは、セキュリティ トークンのコレクションを表します。  <br/> |
|[ドメイン (SOAP)](domains-soap.md) <br/> |構成が[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings**の操作で返されるドメインまたは組織は、 [GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)でフェデレーション ドメインを表す**GetFederationInformation**操作です。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)

