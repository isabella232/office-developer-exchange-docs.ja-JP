---
title: RefreshSharingFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RefreshSharingFolderResponse
api_type:
- schema
ms.assetid: 951ab681-f2d5-4f10-933e-ff199685ff8e
description: RefreshSharingFolderResponse 要素は、RefreshSharingFolder 操作の要求に対する応答を定義します。
ms.openlocfilehash: 4ef7a63b2153c6106dae988439f499046689c2b4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833048"
---
# <a name="refreshsharingfolderresponse"></a>RefreshSharingFolderResponse

**RefreshSharingFolderResponse**要素は、 [RefreshSharingFolder 操作](refreshsharingfolder-operation.md)の要求に対する応答を定義します。 
  
```xml
<RefreshSharingFolderResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</RefreshSharingFolderResponse>
```

 **RefreshSharingFolderResponseMessageType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ResponseClass** <br/> | 応答のステータスについて説明します。 <br/><br/>次の値は、この属性の有効です。  <br/><br/>-成功  <br/>-警告  <br/>-エラー  <br/>- |
   
#### <a name="responseclass-attribute-values"></a>ResponseClass 属性の値

|**値**|**説明**|
|:-----|:-----|
|**Success** <br/> |満了する要求をについて説明します。  <br/> |
|**Warning** <br/> | 処理されなかった要求をについて説明します。 警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。 <br/><br/>警告の送信元の例を次に示します。 <br/> <br/>-Exchange ストアは、バッチの実行中にオフラインです。  <br/>-Active Directory ディレクトリ サービスは、オフラインです。  <br/>-メールボックスは移動されました。  <br/>-メッセージ データベース (MDB) は、オフラインです。  <br/>-パスワードの有効期限が切れています。  <br/>クォータを超えています。  <br/> |
|**Error** <br/> | 満たせない要求をについて説明します。<br/><br/> 次に、エラーのソースの例を示します。  <br/><br/>-無効な属性または要素  <br/>属性または要素が範囲外です  <br/>-不明なタグ  <br/>属性または要素のコンテキストでは無効です  <br/>の任意のクライアントから不正アクセスしようと  <br/>の有効なクライアント側の呼び出しに応答サーバー側の障害  <br/>  <br/>エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |応答のステータスの説明を提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求で発生した特定のエラーを識別するエラー コードを提供します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在使用されていない、将来使用するために予約されています。 この要素には、0 の値が含まれています。  <br/> |
|[MessageXml](messagexml.md) <br/> |追加のエラー応答情報を提供します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [RefreshSharingFolder 操作](refreshsharingfolder-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

