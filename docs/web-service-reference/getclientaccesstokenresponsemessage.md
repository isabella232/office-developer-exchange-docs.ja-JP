---
title: GetClientAccessTokenResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 45ca2500-ceab-4c98-9576-cb9e158e5896
description: GetClientAccessTokenResponseMessage 要素は、GetClientAccessToken 要求の応答メッセージを指定します。
ms.openlocfilehash: 4921e47b6f5c082ed7daf9f0d5250a4a14682bcc
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511558"
---
# <a name="getclientaccesstokenresponsemessage"></a>GetClientAccessTokenResponseMessage

**GetClientAccessTokenResponseMessage** 要素は **、GetClientAccessToken 要求の応答メッセージを指定** します。 
  
```XML
<GetClientAccessTokenResponseMessage ResponseClass=" Success | Warning | Error ">
    <Token/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetClientAccessTokenResponseMessage>
```

 **GetClientAccessTokenResponseMessageType**
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
|[Token (ClientAccessTokenType)](token-clientaccesstokentype.md) <br/> |クライアント アクセス トークンを指定します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在未使用で、将来の使用のために予約されています。  <br/> |
|[MessageText](messagetext.md) <br/> |応答の状態のテキストの説明を提供します。  <br/> |
|[MessageXml](messagexml.md) <br/> |追加のエラー応答情報を提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求に関する状態情報を提供します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Web サービス (EWS) 要求Exchange応答メッセージが含まれます。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

