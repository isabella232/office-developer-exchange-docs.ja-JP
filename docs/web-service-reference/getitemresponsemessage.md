---
title: GetItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetItemResponseMessage
api_type:
- schema
ms.assetid: cc583723-54d1-4a17-8c1f-6586f70fdefd
description: GetItemResponseMessage 要素には、1 つの GetItem 操作要求の状態と結果が含まれる。
ms.openlocfilehash: 3c931a6d7df91e4e90bfd0a69dc4816ee71a0aad
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521963"
---
# <a name="getitemresponsemessage"></a>GetItemResponseMessage

**GetItemResponseMessage** 要素には、1 つの GetItem 操作要求の状態と結果 [が含](getitem-operation.md)まれる。 
  
- [GetItemResponse](getitemresponse.md) 
- [ResponseMessages](responsemessages.md)
- [GetItemResponseMessage](getitemresponsemessage.md)
  
```xml
<GetItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</GetItemResponseMessage>
```

**ItemInfoResponseMessageType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ResponseClass** <br/> | GetItem 操作応答の [状態を説明](getitem-operation.md) します。 <br/><br/>この属性には、次の値が有効です。<br/><br/>- 成功<br/>- 警告<br/>- エラー |
   
#### <a name="responseclass-attribute-values"></a>ResponseClass 属性値

|**値**|**説明**|
|:-----|:-----|
|**Success** <br/> |満たされた要求について説明します。  <br/> |
|**Warning** <br/> | 処理されていない要求について説明します。 要求内のアイテムの処理中にエラーが発生し、後続のアイテムを処理できない場合、警告が返される場合があります。<br/><br/>次に、警告のソースの例を示します。<br/><br/>- バッチExchangeストアはオフラインです。<br/>- Active Directory ドメイン サービス (AD DS) がオフラインです。<br/>- メールボックスが移動されます。<br/>- MDB はオフラインです。<br/>- パスワードの有効期限が切れています。  <br/>- クォータを超えました。 |
|**エラー** <br/> | 満たできない要求について説明します。<br/><br/>エラーのソースの例を次に示します。<br/><br/>- 無効な属性または要素<br/>- 範囲外の属性または要素<br/>- 不明なタグ<br/>- コンテキストで属性または要素が無効<br/>- 任意のクライアントが試行した未承認のアクセス<br/>- 有効なクライアント側の呼び出しに応答してサーバー側でエラーが発生しました<br/><br/>エラーに関する情報は [、ResponseCode](responsecode.md) 要素と [MessageText 要素で確認](messagetext.md) できます。 |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |応答の状態のテキストの説明を提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求が発生した特定のエラーを識別するエラー コードを提供します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在は使用されていないので、将来の使用のために予約されています。 値 0 が含まれる。  <br/> |
|[MessageXml](messagexml.md) <br/> |追加のエラー応答情報を提供します。  <br/> |
|[Items](items.md) <br/> |返されるアイテムの配列を含む。  <br/> |
   
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
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetItem](getitem.md)
- [GetItem 操作](getitem-operation.md)

