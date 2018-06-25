---
title: SyncFolderItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderItemsResponseMessage
api_type:
- schema
ms.assetid: f58e773f-94a7-4729-90f0-ac4c71b4ba59
description: SyncFolderItemsResponseMessage 要素には、状態および 1 つの SyncFolderItems 操作要求の結果が含まれています。
ms.openlocfilehash: 9bb32232143df56ad9de93480e10a5941e68025a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839644"
---
# <a name="syncfolderitemsresponsemessage"></a>SyncFolderItemsResponseMessage

**SyncFolderItemsResponseMessage**要素には、状態および 1 つの結果が含まれている[SyncFolderItems の操作](syncfolderitems-operation.md)を要求します。 
  
- [SyncFolderItemsResponse](syncfolderitemsresponse.md) 
- [ResponseMessages](responsemessages.md)
- [SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)
  
```xml
<SyncFolderItemsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SyncState/>
   <IncludesLastItemInRange/>
   <Changes/>
</SyncFolderItemsResponseMessage>
```

 **SyncFolderItemsResponseMessageType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ResponseClass** <br/> | [SyncFolderItems 操作](syncfolderitems-operation.md)の応答のステータスについて説明します。 <br/><br/>次の値は、この属性の有効です。 <br/> <br/>-成功  <br/>-警告  <br/>-エラー  <br/> |
   
#### <a name="responseclass-attribute"></a>ResponseClass 属性

|**値**|**説明**|
|:-----|:-----|
|**Success** <br/> |満了する要求をについて説明します。  <br/> |
|**Warning** <br/> | 処理されなかった要求をについて説明します。 警告が表示される場合は、要求内のアイテムの処理中にエラーが発生しましたし、それ以降の項目を処理することはできません。 <br/><br/>警告の送信元の例を次に示します。  <br/><br/>-Exchange ストアは、バッチの実行中にオフラインです。  <br/>-Active Directory ドメイン サービス (AD DS) では、オフラインです。  <br/>-メールボックスは移動されました。  <br/>-メッセージ データベース (MDB) は、オフラインです。  <br/>-パスワードの有効期限が切れています。  <br/>クォータを超過しました。  <br/> |
|**Error** <br/> | 満たせない要求をについて説明します。 <br/><br/>次に、エラーのソースの例を示します。  <br/><br/>-無効な属性または要素  <br/>属性または要素の範囲を超えています。  <br/>-不明なタグ  <br/>属性または要素のコンテキストでは有効ではないです。  <br/>-任意のクライアントから許可されていないアクセス試行  <br/>-有効なクライアント側の呼び出しへの応答でサーバー側の障害  <br/>  <br/>エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |応答のステータスの説明を提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求で発生した特定のエラーを識別するエラー コードを提供します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在使用されていない将来の使用に予約されているとします。 0 の値が含まれています。  <br/> |
|[MessageXml](messagexml.md) <br/> |追加のエラー応答情報を提供します。  <br/> |
|[同期状態](syncstate-ex15websvcsotherref.md) <br/> |各成功した要求の後に更新された同期データの base64 でエンコードされたフォームが含まれています。 これを使用して、同期の状態を識別します。  <br/> |
|[IncludesLastItemInRange](includeslastiteminrange.md) <br/> |最後の項目を同期するが、応答に含まれているかどうかを示します。  <br/> |
|[変更 (アイテム)](changes-items.md) <br/> |クライアント上のアイテムと、Exchange サーバー上のアイテム間の相違点の種類を表すの種類の変更の順序の配列が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Exchange Web サービス要求に対する応答メッセージが含まれています。  <br/> |
   
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [SyncFolderItems の操作](syncfolderitems-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

