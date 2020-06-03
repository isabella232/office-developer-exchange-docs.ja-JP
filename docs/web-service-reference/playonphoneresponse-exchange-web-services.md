---
title: PlayOnPhoneResponse (Exchange Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PlayOnPhoneResponse
api_type:
- schema
ms.assetid: 578b70d1-dc9d-4bce-b859-0109b2d2bcec
description: PlayOnPhoneResponse 要素は、電話でボイスメールを再生する要求に対する応答を指定します。
ms.openlocfilehash: 907864d7fe669aac99b2ff6d1c5eba71b9ddf79f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459624"
---
# <a name="playonphoneresponse-exchange-web-services"></a>PlayOnPhoneResponse (Exchange Web サービス)

**PlayOnPhoneResponse**要素は、電話でボイスメールを再生する要求に対する応答を指定します。 
  
```xml
<PlayOnPhoneResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <PhoneCallId/>
</PlayOnPhoneResponse>
```

 **PlayOnPhoneResponseMessageType**
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
|**Warning** <br/> | 処理されなかった要求を示します。 要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。<br/><br/> 警告のソースの例を次に示します。 <br/><br/>-バッチ処理中に Exchange ストアがオフラインになります。  <br/>-Active Directory ドメインサービス (AD DS) がオフラインになっています。  <br/>-メールボックスが移動されました。  <br/>-メッセージデータベース (MDB) はオフラインです。  <br/>-パスワードの有効期限が切れています。  <br/>-クォータが限界を超えています。  <br/> |
|**Error** <br/> | 満たされない要求を記述します。 <br/><br/>エラーのソースの例を次に示します。  <br/><br/>-属性または要素が無効です。  <br/>-範囲外の属性または要素  <br/>-不明なタグ。  <br/>-コンテキスト内で有効ではない属性または要素。  <br/>-クライアントによる権限のないアクセス試行。  <br/>-有効なクライアント側の呼び出しに応答して、サーバー側で障害が発生した。  <br/><br/>  エラーに関する情報については、「応答[sec」](responsecode.md)および「 [messagetext](messagetext.md)要素」のトピックを参照してください。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |応答の状態を説明するテキストを提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求で発生した特定のエラーを識別するエラーコードを提供します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在未使用で、今後の使用のために予約されています。 この要素には0の値が含まれています。  <br/> |
|[MessageXml](messagexml.md) <br/> |エラー応答に関する追加情報を提供します。  <br/> |
|[PhoneCallId](phonecallid.md) <br/> |電話の通話識別子を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

