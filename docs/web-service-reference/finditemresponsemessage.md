---
title: FindItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FindItemResponseMessage
api_type:
- schema
ms.assetid: fb2cd399-8a04-4f26-9091-993134ed1d15
description: FindItemResponseMessage 要素には、1 つの FindItem 操作要求の状態と結果が含まれる。
ms.openlocfilehash: 8a736f6782b6901a2b41ea8c602832614a331a06
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518415"
---
# <a name="finditemresponsemessage"></a>FindItemResponseMessage

**FindItemResponseMessage** 要素には、1 つの FindItem 操作要求の状態と結果 [が含](finditem-operation.md)まれる。 
  
- [FindItemResponse](finditemresponse.md) 
- [ResponseMessages](responsemessages.md)
- [FindItemResponseMessage](finditemresponsemessage.md)
  
```xml
<FindItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RootFolder/>
</FindItemResponseMessage>
```

 **FindItemResponseMessageType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ResponseClass** <br/> | FindItem 操作応答の [状態を説明](finditem-operation.md) します。<br/><br/> この属性には、次の値が有効です。 <br/> <br/>- 成功  <br/>- 警告  <br/>- エラー  <br/> |
   
#### <a name="responseclass-attribute-values"></a>ResponseClass 属性値

|**値**|**説明**|
|:-----|:-----|
|**Success** <br/> |満たされた要求について説明します。  <br/> |
|**Warning** <br/> | 処理されていない要求について説明します。 要求内のアイテムの処理中にエラーが発生し、後続のアイテムを処理できない場合、警告が返される場合があります。 <br/><br/>次に、警告の発生源の例を示します。 <br/> <br/>- バッチ中Exchangeストアがオフラインになります。  <br/>- Active Directory ドメイン サービス (AD DS) がオフラインになります。  <br/>- メールボックスが移動されます。  <br/>- メッセージ データベース (MDB) がオフラインになります。  <br/>- パスワードの有効期限が切れています。  <br/>- クォータを超えました。  <br/> |
|**エラー** <br/> | 満たできない要求について説明します。 <br/><br/>エラーの原因の例を次に示します。  <br/><br/>- 無効な属性または要素  <br/>- 範囲外の属性または要素  <br/>- 不明なタグ  <br/>- コンテキストで無効な属性または要素  <br/>- 任意のクライアントによる承認されていないアクセス試行  <br/>- 有効なクライアント側の呼び出しに応答したサーバー側のエラー  <br/><br/>  エラーに関する情報は [、ResponseCode](responsecode.md) 要素と [MessageText 要素で確認](messagetext.md) できます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |応答の状態のテキストの説明を提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求が発生した特定のエラーを識別するエラー コードを提供します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在は使用されていないので、将来の使用のために予約されています。 値 0 が含まれる。  <br/> |
|[MessageXml](messagexml.md) <br/> |追加のエラー応答情報を提供します。  <br/> |
|[RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md) <br/> |FindItem 操作中に 1 つのルート フォルダーを検索した結果 [を格納します](finditem-operation.md)。  <br/> |
   
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

- [FindItem 操作](finditem-operation.md)
- [アイテムの検索](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

