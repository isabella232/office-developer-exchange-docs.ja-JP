---
title: GetPasswordExpirationDateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3d3fff1f-ef13-46d5-bd7f-ef535eb80c72
description: GetPasswordExpirationDateResponse 要素は、GetPasswordExpirationDate 操作要求への応答を定義します。
ms.openlocfilehash: bad4cf5ea70e669ccfb98cc9e2eb7d0e5924949e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535025"
---
# <a name="getpasswordexpirationdateresponse"></a>GetPasswordExpirationDateResponse

**GetPasswordExpirationDateResponse** 要素は [、GetPasswordExpirationDate](getpasswordexpirationdate-operation.md)操作要求への応答を定義します。 
  
- [ResponseMessages](responsemessages.md)
- [GetPasswordExpirationDateResponse](getpasswordexpirationdateresponse.md)
  
```XML
<GetPasswordExpirationDateResponse>
    <PasswordExpirationDate />
</GetPasswordExpirationDateResponse>
```

 **GetPasswordExpirationDateResponseMessageType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ResponseClass** <br/> | 応答の状態を説明します。 <br/><br/>この属性には、次の値が有効です。  <br/><br/>- 成功  <br/>- 警告  <br/>- エラー  <br/> |
   
#### <a name="responseclass-attribute-values"></a>ResponseClass 属性値

|**値**|**説明**|
|:-----|:-----|
|**Success** <br/> |満たされた要求について説明します。  <br/> |
|**Warning** <br/> | 処理されていない要求について説明します。 要求内のアイテムの処理中にエラーが発生し、後続のアイテムを処理できない場合は、警告が返される場合があります。<br/><br/> 次に、警告の発生源の例を示します。  <br/><br/>- バッチExchangeストアはオフラインです。  <br/>- Active Directory ドメイン サービス (AD DS) がオフラインです。  <br/>- メールボックスが移動されました。  <br/>- メッセージ データベース (MDB) がオフラインです。  <br/>- パスワードの有効期限が切れています。  <br/>- クォータを超えました。  <br/> |
|**エラー** <br/> | 満たできない要求について説明します。 <br/><br/>エラーの原因の例を次に示します。  <br/><br/>- 無効な属性または要素。  <br/>- 範囲外の属性または要素。  <br/>- 不明なタグ。  <br/>- コンテキストで無効な属性または要素。  <br/>- 任意のクライアントによる未承認のアクセス試行。  <br/>- 有効なクライアント側の呼び出しに応答したサーバー側のエラー。  <br/><br/>  エラーに関する情報は [、ResponseCode](responsecode.md) 要素と [MessageText 要素で確認](messagetext.md) できます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素名**|**説明**|
|:-----|:-----|
|[PasswordExpirationDate](passwordexpirationdate.md) <br/> |要求で指定された電子メール アカウントのパスワードの有効期限を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素名**|**説明**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Web サービス (EWS) 要求Exchange応答メッセージが含まれます。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetPasswordExpirationDate 操作](getpasswordexpirationdate-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

