---
title: DisableAppResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 11ebe618-d759-4f16-be99-eaaa817ba782
description: DisableAppResponse 要素は、DisableApp 要求への応答を指定します。
ms.openlocfilehash: 740801fa4b60e217f0b9148bcfcc5b206e96bf31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760065"
---
# <a name="disableappresponse"></a>DisableAppResponse

**DisableAppResponse**要素は、 **DisableApp**要求への応答を指定します。 
  
```XML
<DisableAppResponse>
    <MessageText></MessageText>
    <ResponseCode></ResponeCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</DisableAppResponse>
```

 **DisableAppResponseType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |応答のステータスの説明を提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求に関するステータス情報を提供します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在使用されていない、将来使用するために予約されています。  <br/> |
|[MessageXml](messagexml.md) <br/> |追加のエラー応答情報を提供します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

