---
title: GetPasswordExpirationDateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d3fff1f-ef13-46d5-bd7f-ef535eb80c72
description: GetPasswordExpirationDateResponse 要素は、GetPasswordExpirationDate 操作操作要求への応答を定義します。
ms.openlocfilehash: c925b2b37879ba0f8f25b2dd73737ed2f3202555
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530205"
---
# <a name="getpasswordexpirationdateresponse"></a>GetPasswordExpirationDateResponse

**GetPasswordExpirationDateResponse**要素は、 [GetPasswordExpirationDate 操作](getpasswordexpirationdate-operation.md)操作要求への応答を定義します。 
  
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
|**ResponseClass** <br/> | 応答の状態を表します。 <br/><br/>この属性には、次の値が有効です。  <br/><br/>-成功  <br/>-Warning  <br/>-エラー  <br/> |
   
#### <a name="responseclass-attribute-values"></a>ResponseClass 属性の値

|**値**|**説明**|
|:-----|:-----|
|**Success** <br/> |満たされる要求を記述します。  <br/> |
|**Warning** <br/> | 処理されなかった要求を示します。 要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。<br/><br/> 警告のソースの例を次に示します。  <br/><br/>-バッチ処理中に Exchange ストアがオフラインになります。  <br/>-Active Directory ドメインサービス (AD DS) がオフラインになっています。  <br/>-メールボックスが移動されました。  <br/>-メッセージデータベース (MDB) はオフラインです。  <br/>-パスワードの有効期限が切れています。  <br/>-クォータが限界を超えています。  <br/> |
|**Error** <br/> | 満たされない要求を記述します。 <br/><br/>エラーのソースの例を次に示します。  <br/><br/>-属性または要素が無効です。  <br/>-範囲外の属性または要素。  <br/>-不明なタグ。  <br/>-コンテキスト内で有効ではない属性または要素。  <br/>-クライアントによる権限のないアクセス試行。  <br/>-有効なクライアント側の呼び出しに応答して、サーバー側で障害が発生した。  <br/><br/>  エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素名**|**説明**|
|:-----|:-----|
|[PasswordExpirationDate](passwordexpirationdate.md) <br/> |要求で指定された電子メールアカウントのパスワードの有効期限日を示します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素名**|**説明**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Exchange Web サービス (EWS) 要求に対する応答メッセージが保存されています。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetPasswordExpirationDate 操作](getpasswordexpirationdate-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

