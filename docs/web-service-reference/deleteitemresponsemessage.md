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
description: DeleteItemResponseMessage 要素には、1つの DeleteItem 操作要求の状態と結果が含まれています。
ms.openlocfilehash: 78e3efc6a9e9e6629d7efe7f2dc294e0a731005a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526929"
---
# <a name="deleteitemresponsemessage"></a>DeleteItemResponseMessage

**DeleteItemResponseMessage**要素には、1つの[DeleteItem 操作](deleteitem-operation.md)要求の状態と結果が含まれています。 
  
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
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ResponseClass** <br/> | [DeleteItem 操作](deleteitem-operation.md)の応答の状態を表します。<br/><br/>この属性には、次の値が有効です。<br/><br/>-成功  <br/>-Warning  <br/>-エラー  <br/> |
   
#### <a name="responseclass-attribute"></a>ResponseClass 属性

|**値**|**説明**|
|:-----|:-----|
|**Success** <br/> |満たされる要求を記述します。  <br/> |
|**Warning** <br/> | 処理されなかった要求を示します。 要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。<br/><br/>警告のソースの例を次に示します。<br/><br/>-バッチ処理中に Exchange ストアがオフラインになります。  <br/>-Active Directory ドメインサービス (AD DS) はオフラインになります。  <br/>-メールボックスは移動されます。  <br/>-メッセージデータベース (MDB) はオフラインになります。  <br/>-パスワードの有効期限が切れています。  <br/>-クォータが上限を超えています。  <br/> |
|**Error** <br/> | 満たされない要求を記述します。<br/><br/>エラーのソースの例を次に示します。<br/><br/>-無効な属性または要素  <br/>-属性または要素が範囲外です  <br/>-不明なタグ  <br/>-属性または要素がコンテキスト内で有効ではありません  <br/>-クライアントは、管理者によって許可されている最大レベル以上のエラーログ出力レベルを設定しようとしました  <br/>-クライアントは、管理者によって指定された既定のレベルの下に重大度エラーレベルを設定しようとしています。  <br/>-クライアントによる権限のないアクセス試行  <br/>-有効なクライアント側の呼び出しに応答した場合のサーバー側エラー<br/><br/>  エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |応答の状態を説明するテキストを提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求で発生した特定のエラーを識別するエラーコードを提供します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在未使用で、今後の使用のために予約されています。 このプロパティには0の値が含まれています。  <br/> |
|[MessageXml](messagexml.md) <br/> |エラー応答に関する追加情報を提供します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Exchange Web サービス要求に対する応答メッセージを含みます。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
### <a name="version-differences"></a>バージョンの相違点

Build 15.00.0986.00 以降のバージョンの Exchange では、 **DeleteItemResponseMessage**要素の型は**Deleteitemresponsemessagetype**です。 以前のバージョンでは、要素の種類は**Responsemessagetype**です。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [DeleteItem 操作](deleteitem-operation.md)
- [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)
- [アイテムの削除 (Exchange Web サービス)](https://msdn.microsoft.com/library/9bfc39e6-d944-4eb6-8aee-cbaf1e37c67d%28Office.15%29.aspx)

