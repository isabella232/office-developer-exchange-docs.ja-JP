---
title: GetAppMarketplaceUrlResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc3368ec-78c2-4f8d-8394-4891e90dafd2
description: GetAppMarketplaceUrlResponse 要素は、GetAppMarketplaceUrl 要求への応答を指定します。
ms.openlocfilehash: 553ebfc4615280c77d4a1ef9e5db3e5d10a0f2a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760634"
---
# <a name="getappmarketplaceurlresponse"></a>GetAppMarketplaceUrlResponse

**GetAppMarketplaceUrlResponse**要素は、 **GetAppMarketplaceUrl**要求への応答を指定します。 
  
```XML
<GetAppMarketplaceUrlResponse ResponseClass=" Success | Warning | Error ">
    <AppMarketplaceUrl/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetAppMarketplaceUrlResponse>
```

 **GetAppMarketplaceUrlResponseMessageType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ResponseClass  <br/> |応答のクラスを示します。  <br/> |
   
#### <a name="responseclass"></a>ResponseClass

|**値**|**説明**|
|:-----|:-----|
|成功  <br/> |成功を示します。  <br/> |
|警告  <br/> |警告を示します。  <br/> |
|エラー  <br/> |エラーを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[AppMarketplaceUrl](appmarketplaceurl.md) <br/> |アプリケーションの URL を指定します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在使用されていない、将来使用するために予約されています。  <br/> |
|[MessageText](messagetext.md) <br/> |応答のステータスの説明を提供します。  <br/> |
|[MessageXml](messagexml.md) <br/> |追加のエラー応答情報を提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求に関するステータス情報を提供します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Exchange Web サービス要求に対する応答メッセージが含まれています。  <br/> |
   
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

