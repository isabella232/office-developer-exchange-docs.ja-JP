---
title: DeleteItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItemResponseMessage
api_type:
- schema
ms.assetid: c3d34c4d-8d83-4612-aa9e-66f9cc7314df
description: DeleteItemResponseMessage 要素には、状態および 1 つの DeleteItem 操作要求の結果が含まれています。
ms.openlocfilehash: 1f0cc3d49bfa5fba6da32cf65df6b6718ccfbded
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759997"
---
# <a name="deleteitemresponsemessage"></a>DeleteItemResponseMessage

**DeleteItemResponseMessage**要素には、状態および 1 つの結果が含まれている[DeleteItem の操作](deleteitem-operation.md)を要求します。 
  
- [DeleteItemResponse](deleteitemresponse.md) 
- [ResponseMessages](responsemessages.md)  
- [DeleteItemResponseMessage](deleteitemresponsemessage.md)
  
```xml
<DeleteItemResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DeleteItemResponseMessage>
```

 **DeleteItemResponseMessageType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ResponseClass** <br/> | [DeleteItem 操作](deleteitem-operation.md)の応答のステータスについて説明します。<br/><br/>次の値は、この属性の有効です。<br/><br/>-成功  <br/>-警告  <br/>-エラー  <br/> |
   
#### <a name="responseclass-attribute"></a>ResponseClass 属性

|**値**|**説明**|
|:-----|:-----|
|**Success** <br/> |満了する要求をについて説明します。  <br/> |
|**Warning** <br/> | 処理されなかった要求をについて説明します。 警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。<br/><br/>警告の送信元の例を次に示します。<br/><br/>-Exchange ストアは、バッチの中にオフラインです。  <br/>-Active Directory ドメイン サービス (AD DS) がオフラインになった。  <br/>-メールボックスを移動します。  <br/>-メッセージ データベース (MDB) がオフラインになった。  <br/>-パスワードの有効期限が切れています。  <br/>クォータを超えています。  <br/> |
|**Error** <br/> | 満たせない要求をについて説明します。<br/><br/>次に、エラーのソースの例を示します。<br/><br/>-無効な属性または要素  <br/>属性または要素が範囲外です  <br/>-不明なタグ  <br/>属性または要素のコンテキストでは無効です  <br/>-クライアントが、管理者によって許可されている最大レベルよりも上のエラーのログ出力レベルを設定しようとしています。  <br/>-クライアントが、管理者によって指定されている既定のレベル以下のエラーの重大度レベルを設定しようとしています。  <br/>の任意のクライアントから不正アクセスしようと  <br/>の有効なクライアント側の呼び出しに応答サーバー側の障害<br/><br/>  エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |応答のステータスの説明を提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求で発生した特定のエラーを識別するエラー コードを提供します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在使用されていない将来の使用に予約されているとします。 0 の値が含まれています。  <br/> |
|[MessageXml](messagexml.md) <br/> |追加のエラー応答情報を提供します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Exchange Web サービス要求に対する応答メッセージが含まれています。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
### <a name="version-differences"></a>バージョンの相違点

Exchange のビルド 15.00.0986.00 以降のバージョンでは、 **DeleteItemResponseMessage**要素は型**DeleteItemResponseMessageType**のです。 以前のバージョンでは、型**ResponseMessageType**の要素です。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [DeleteItem の操作](deleteitem-operation.md)
- 
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)
- [(Exchange Web サービス) の項目の削除](http://msdn.microsoft.com/library/9bfc39e6-d944-4eb6-8aee-cbaf1e37c67d%28Office.15%29.aspx)

