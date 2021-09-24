---
title: RefreshSharingFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RefreshSharingFolderResponse
api_type:
- schema
ms.assetid: 951ab681-f2d5-4f10-933e-ff199685ff8e
description: RefreshSharingFolderResponse 要素は、RefreshSharingFolder 操作要求への応答を定義します。
ms.openlocfilehash: 8e59a4481db2b5f6adc9d819c2c76dee3fe46671
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513473"
---
# <a name="refreshsharingfolderresponse"></a>RefreshSharingFolderResponse

**RefreshSharingFolderResponse** 要素は [、RefreshSharingFolder](refreshsharingfolder-operation.md)操作要求への応答を定義します。 
  
```xml
<RefreshSharingFolderResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</RefreshSharingFolderResponse>
```

 **RefreshSharingFolderResponseMessageType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ResponseClass** <br/> | 応答の状態を説明します。 <br/><br/>この属性には、次の値が有効です。  <br/><br/>- 成功  <br/>- 警告  <br/>- エラー  <br/>- |
   
#### <a name="responseclass-attribute-values"></a>ResponseClass 属性値

|**値**|**説明**|
|:-----|:-----|
|**Success** <br/> |満たされた要求について説明します。  <br/> |
|**Warning** <br/> | 処理されていない要求について説明します。 要求内のアイテムの処理中にエラーが発生し、後続のアイテムを処理できない場合は、警告が返される場合があります。 <br/><br/>次に、警告の発生源の例を示します。 <br/> <br/>- バッチExchangeストアはオフラインです。  <br/>- Active Directory ディレクトリ サービスがオフラインです。  <br/>- メールボックスが移動されました。  <br/>- メッセージ データベース (MDB) がオフラインです。  <br/>- パスワードの有効期限が切れています。  <br/>- クォータを超えました。  <br/> |
|**エラー** <br/> | 満たできない要求について説明します。<br/><br/> エラーの原因の例を次に示します。  <br/><br/>- 無効な属性または要素  <br/>- 範囲外の属性または要素  <br/>- 不明なタグ  <br/>- コンテキストで属性または要素が無効  <br/>- 任意のクライアントによる未承認のアクセス試行  <br/>- 有効なクライアント側の呼び出しに応答してサーバー側でエラーが発生しました  <br/>  <br/>エラーに関する情報は [、ResponseCode](responsecode.md) 要素と [MessageText 要素で確認](messagetext.md) できます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |応答の状態のテキストの説明を提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求が発生した特定のエラーを識別するエラー コードを提供します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在未使用で、将来の使用のために予約されています。 この要素には、値 0 が含まれる。  <br/> |
|[MessageXml](messagexml.md) <br/> |追加のエラー応答情報を提供します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [RefreshSharingFolder 操作](refreshsharingfolder-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

