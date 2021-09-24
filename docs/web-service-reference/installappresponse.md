---
title: InstallAppResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c5e0582d-c1e1-453b-93ed-c31165c82697
description: InstallAppResponse 要素は、InstallApp 要求への応答を指定します。
ms.openlocfilehash: c124757d60a1e4fedd583cc677afddaa5a32e856
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59532931"
---
# <a name="installappresponse"></a>InstallAppResponse

**InstallAppResponse 要素は****、InstallApp** 要求への応答を指定します。 
  
```xml
<InstallAppResponse ResponseClass="">
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</InstallAppResponse>
```

 **InstallAppResponseType**
## <a name="attributes-and-elements"></a>属性と要素

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
|Error  <br/> |エラーを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在未使用で、将来の使用のために予約されています。  <br/> |
|[MessageText](messagetext.md) <br/> |応答の状態のテキストの説明を提供します。  <br/> |
|[MessageXml](messagexml.md) <br/> |追加のエラー応答情報を提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求に関する状態情報を提供します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Web サービス要求の応答メッセージExchange含まれます。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

**GetAppManifestsResponseMessage** 要素は、2013 年から Exchange Online およびバージョンの Microsoft Exchange Server を対象とするクライアントExchangeです。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

