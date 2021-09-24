---
title: ResolveNamesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResolveNamesResponseMessage
api_type:
- schema
ms.assetid: edcdaf58-ef63-412e-8c58-409213e6ab0d
description: ResolveNamesResponseMessage 要素には、ResolveNames 操作要求の状態と結果が含まれる。
ms.openlocfilehash: a7debc5f5056ad7a33ebfaf2b0d5d914acdb2397
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523476"
---
# <a name="resolvenamesresponsemessage"></a>ResolveNamesResponseMessage

**ResolveNamesResponseMessage** 要素には [、ResolveNames](resolvenames-operation.md)操作要求の状態と結果が含まれる。 
  
- [ResolveNamesResponse](resolvenamesresponse.md) 
- [ResponseMessages](responsemessages.md)
- [ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
  
```xml
<ResolveNamesResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ResolutionSet/>
</ResolveNamesResponseMessage>
```

 **ResolveNamesResponseMessageType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ResponseClass** <br/> | ResolveNames 操作応答 [の状態を説明](resolvenames-operation.md) します。 <br/><br/>この属性には、次の値が有効です。  <br/><br/>- 成功  <br/>- 警告  <br/>- エラー  <br/> |
   
#### <a name="responseclass-attribute"></a>ResponseClass 属性

|**値**|**説明**|
|:-----|:-----|
|**Success** <br/> |満たされた要求について説明します。 これは、要求された名前があいまいで、応答に 1 つの受信者が含まれている場合に発生します。  <br/> |
|**Warning** <br/> | 処理されていない要求について説明します。 要求内のアイテムの処理中にエラーが発生し、後続のアイテムを処理できない場合は、警告が返される場合があります。 <br/><br/>警告のソースの例を次に示します。  <br/><br/>- バッチ中Exchangeストアがオフラインになります。  <br/>- Active Directory ドメイン サービス (AD DS) がオフラインになります。  <br/>- メールボックスが移動されます。  <br/>- メールボックス データベース (MDB) がオフラインになります。  <br/>- パスワードの有効期限が切れています。  <br/>- クォータを超えました。  <br/>- 要求された名前があいまいで、応答に複数の受信者が含まれている。  <br/> |
|**エラー** <br/> | 満たできない要求について説明します。 <br/><br/>エラーの原因の例を次に示します。  <br/><br/>- 要求された名前を解決できない。  <br/>- 属性または要素が無効です。  <br/>- 属性または要素が範囲を外しています。  <br/>- タグが不明です。  <br/>- 属性または要素がコンテキストで無効です。  <br/>- 任意のクライアントによる承認されていないアクセス試行が発生しました。  <br/>- 有効なクライアント側の呼び出しに応答してサーバー側のエラーが発生しました。  <br/>  <br/>エラーに関する情報は [、ResponseCode](responsecode.md) 要素と [MessageText 要素で確認](messagetext.md) できます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |応答の状態のテキストの説明を提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求に関するエラー情報を提供します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在は使用されていないので、将来の使用のために予約されています。 値 0 が含まれる。  <br/> |
|[MessageXml](messagexml.md) <br/> |追加のエラー応答情報を提供します。  <br/> |
|[ResolutionSet](resolutionset.md) <br/> |あいまいな名前の解像度の配列を含む。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Web サービス要求の応答メッセージExchange含まれます。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [ResolveNames](resolvenames.md)
- [ResolveNamesResponse](resolvenamesresponse.md)
- [ResolveNames 操作](resolvenames-operation.md)

