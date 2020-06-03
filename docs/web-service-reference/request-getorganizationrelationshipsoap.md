---
title: Request (Get組織関係) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 85dc155c-fad0-4756-b9a8-dedf5040a7c6
description: Request 要素は、GetOrganizationRelationshipSettingsRequest (SOAP) 要求を表します。 Request 要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。
ms.openlocfilehash: 90ccd3579c91c916ea645e6a3b466c9de4706421
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459561"
---
# <a name="request-getorganizationrelationship-soap"></a>Request (Get組織関係) (SOAP)

**Request**要素は、 [Getorganizationrelationshipsettingsrequest (SOAP)](getorganizationrelationshipsettingsrequest-soap.md)要求を表します。 **Request**要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。 
  
```XML
<Request>
   <Domains/>
</Request>
```

 **Get組織の Relationshipsettingsrequest**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Domains (SOAP)](domains-soap.md) <br/> |自動検出が実行され、クエリで使用されるドメインを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetOrganizationRelationshipSettingsRequestMessage (SOAP)](getorganizationrelationshipsettingsrequestmessage-soap.md) <br/> |[Get組織の設定操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)操作要求を表します。  <br/> |
   
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



[Get組織の Relationshipsettingsrequest (SOAP)](getorganizationrelationshipsettingsrequest-soap.md)


[自動検出の使用](https://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx)

