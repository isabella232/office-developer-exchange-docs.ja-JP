---
title: Response (GetDomainSettings) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a5b052df-93bd-4fe1-ac30-83de9a3dfcd7
description: Response 要素は、個々のドメインに対する GetDomainSettings 呼び出しへの応答を表します。
ms.openlocfilehash: 67fe7aea4533058fa0df972e49a2069749dc258b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455584"
---
# <a name="response-getdomainsettings-soap"></a>Response (GetDomainSettings) (SOAP)

**Response**要素は、個々のドメインに対する**getdomainsettings**呼び出しへの応答を表します。 
  
```XML
<Response>
   <DomainResponses/>
   <ErrorCode/>
   <ErrorMessage/>
</Response>
```

 **GetDomainSettingsResponse**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[DomainResponses (SOAP)](domainresponses-soap.md) <br/> |**Getdomainsettings**要求で要求された各ドメインに対する応答を含みます。  <br/> |
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |応答に関連付けられているエラーコードが含まれます (該当する場合)。  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |応答に関連付けられているエラーメッセージ (該当する場合) が含まれます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetDomainSettingsResponseMessage (SOAP)](getdomainsettingsresponsemessage-soap.md) <br/> |発信者にドメインの構成設定を返します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)

