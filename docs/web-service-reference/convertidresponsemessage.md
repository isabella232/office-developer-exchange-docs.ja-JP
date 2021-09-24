---
title: ConvertIdResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConvertIdResponseMessage
api_type:
- schema
ms.assetid: 7a439cae-0268-4328-9ded-af56ad642227
description: ConvertIdResponseMessage 要素には、ConvertId 操作要求の状態と結果が含まれる。
ms.openlocfilehash: 28792cd62b76323f942138796ee2d0596b9664ff
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518660"
---
# <a name="convertidresponsemessage"></a>ConvertIdResponseMessage

**ConvertIdResponseMessage** 要素には [、ConvertId](convertid-operation.md)操作要求の状態と結果が含まれる。 
  
- [ConvertIdResponse](convertidresponse.md) 
- [ResponseMessages](responsemessages.md)
- [ConvertIdResponseMessage](convertidresponsemessage.md)
  
```xml
<ConvertIdResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <AlternateId/>
</ConvertIdResponseMessage>
```

 **ConvertIdResponseMessageType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ResponseClass** <br/> | ConvertId 操作応答の [状態を説明](convertid-operation.md) します。<br/><br/>この属性には、次の値が有効です。<br/><br/>- 成功  <br/>- 警告  <br/>- エラー  <br/> |
   
#### <a name="responseclass-attribute-values"></a>ResponseClass 属性値

|**値**|**説明**|
|:-----|:-----|
|**Success** <br/> |満たされた要求について説明します。  <br/> |
|**Warning** <br/> | 完全に処理されていない要求、または意図しない結果が発生した要求について説明します。  <br/> |
|**エラー** <br/> | 満たできない要求について説明します。<br/><br/>エラーの原因の例を次に示します。  <br/><br/>- 無効な属性または要素  <br/>- 範囲外の属性または要素  <br/>- 不明なタグ  <br/>- コンテキストで無効な属性または要素  <br/>- 任意のクライアントによる承認されていないアクセス試行  <br/>- 有効なクライアント側の呼び出しに応答したサーバー側のエラー<br/><br/>エラーに関する情報は [、ResponseCode](responsecode.md) 要素と [MessageText 要素で確認](messagetext.md) できます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |応答の状態のテキストの説明を提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求が発生した特定のエラーを識別するエラー コードを提供します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在未使用で、将来の使用のために予約されています。 この要素には、値 0 が含まれる。  <br/> |
|[MessageXml](messagexml.md) <br/> |追加のエラー応答情報を提供します。  <br/> |
|[AlternateId](alternateid.md) <br/> |応答内の変換された識別子について説明します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Web サービス要求の応答メッセージExchange含まれます。  <br/> |
   
## <a name="remarks"></a>注釈

変換された識別子ごとに 1 つの応答メッセージが返されます。 [エラー応答コードが返された場合、AlternateId](alternateid.md)要素は応答から欠落します。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Exchange 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [ConvertId 操作](convertid-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

