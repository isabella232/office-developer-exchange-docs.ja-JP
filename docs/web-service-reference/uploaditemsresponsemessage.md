---
title: UploadItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UploadItemsResponseMessage
api_type:
- schema
ms.assetid: 03febd08-c015-4009-b291-1b4296182ffe
description: UploadItemsResponseMessage 要素には、1つのメールボックスアイテムをアップロードする要求の状態と結果が含まれています。
ms.openlocfilehash: 4049772c560f3d54a31351fe1fbed77fe5780bf8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468496"
---
# <a name="uploaditemsresponsemessage"></a>UploadItemsResponseMessage

**UploadItemsResponseMessage**要素には、1つのメールボックスアイテムをアップロードする要求の状態と結果が含まれています。 
  
- [UploadItemsResponse](uploaditemsresponse.md) 
- [ResponseMessages](responsemessages.md)
- [UploadItemsResponseMessage](uploaditemsresponsemessage.md)
  
```XML
<UploadItemsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ItemId/>
</UploadItemsResponseMessage>
```

 **UploadItemsResponseMessageType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ResponseClass** <br/> | 応答の状態を表します。 <br/><br/>この属性には、次の値が有効です。  <br/><br/>-成功  <br/>-Warning  <br/>-エラー  <br/> |
   
#### <a name="responseclass-attribute-values"></a>ResponseClass 属性の値

|**値**|**説明**|
|:-----|:-----|
|**Success** <br/> |満たされる要求を記述します。  <br/> |
|**Warning** <br/> | 処理されなかった要求を示します。 要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。 <br/><br/>警告のソースの例を次に示します。  <br/><br/>-バッチ処理中に Exchange ストアがオフラインになります。  <br/>-Active Directory ドメインサービス (AD DS) がオフラインになっています。  <br/>-メールボックスが移動されました。  <br/>-メッセージデータベース (MDB) はオフラインです。  <br/>-パスワードの有効期限が切れています。  <br/>-クォータが限界を超えています。  <br/> |
|**Error** <br/> | 満たされない要求を記述します。 <br/><br/>エラーのソースの例を次に示します。  <br/><br/>-無効な属性または要素  <br/>-範囲外の属性または要素  <br/>-不明なタグ  <br/>-コンテキスト内で有効ではない属性または要素  <br/>-クライアントによる権限のないアクセス試行  <br/>-有効なクライアント側の呼び出しに応答した場合のサーバー側障害  <br/> <br/> エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |応答の状態を説明するテキストを提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求で発生した特定のエラーを識別するエラーコードを提供します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在未使用で、今後の使用のために予約されています。 この要素には0の値が含まれています。  <br/> |
|[MessageXml](messagexml.md) <br/> |エラー応答に関する追加情報を提供します。  <br/> |
|[ItemId](itemid.md) <br/> |アップロードされたアイテムのアイテム識別子を含みます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Exchange Web サービス要求に対する応答メッセージを含みます。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [ExportItems 操作](exportitems-operation.md)
- [UploadItems 操作](uploaditems-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

