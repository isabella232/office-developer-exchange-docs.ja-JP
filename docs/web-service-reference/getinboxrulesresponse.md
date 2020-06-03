---
title: Get受信規則の応答
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetInboxRulesResponse
api_type:
- schema
ms.assetid: 6d6c1950-c328-489a-94bf-a250fdbd5cd9
description: Get受信規則の Response 要素は、Get受信トレイの操作要求への応答を定義します。
ms.openlocfilehash: 0d67d7eaf6ffbeeb790249190a98f252dbdb9c87
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458286"
---
# <a name="getinboxrulesresponse"></a>Get受信規則の応答

**Get受信**規則の response 要素は、 [get受信トレイの操作](getinboxrules-operation.md)要求への応答を定義します。 
  
```XML
<GetInboxRulesResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <OutlookRuleBlobExists/>
   <InboxRules/>
</GetInboxRulesResponse>
```

 **Get受信規則 Responsetype**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ResponseClass** <br/> | [Get受信トレイの操作](getinboxrules-operation.md)応答の状態を表します。 <br/><br/>この属性には、次の値が有効です。 <br/> <br/>-成功  <br/>-Warning  <br/>-エラー  <br/> |
   
#### <a name="responseclass-attribute"></a>ResponseClass 属性

|**値**|**説明**|
|:-----|:-----|
|**Success** <br/> |満たされる要求を記述します。  <br/> |
|**Warning** <br/> | 処理されなかった要求を示します。 要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。 <br/><br/>警告のソースの例を次に示します。  <br/><br/>-バッチ処理中に Exchange ストアがオフラインになります。  <br/>-Active Directory ドメインサービス (AD DS) がオフラインになっています。  <br/>-メールボックスは移動されます。  <br/>-メッセージデータベース (MDB) はオフラインです。  <br/>-パスワードの有効期限が切れています。  <br/>-クォータが上限を超えています。  <br/> |
|**Error** <br/> | 満たされない要求を記述します。 <br/><br/>エラーのソースの例を次に示します。  <br/><br/>-無効な属性または要素  <br/>-範囲外の属性または要素  <br/>-不明なタグ  <br/>-コンテキスト内で有効ではない属性または要素  <br/>-クライアントによる権限のないアクセス試行  <br/>-有効なクライアント側の呼び出しに応答した場合のサーバー側障害  <br/><br/>  エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |応答の状態の説明をテキストで提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求に関する状態情報を提供します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在未使用で、今後の使用のために予約されています。 このプロパティには0の値が含まれています。  <br/> |
|[MessageXml](messagexml.md) <br/> |エラー応答に関する追加情報を提供します。  <br/> |
|[OutlookRuleBlobExists](outlookruleblobexists.md) <br/> |ユーザーのメールボックスに Microsoft Outlook のルール blob が存在するかどうかを示します。  <br/> |
|[受信トレイのルール](inboxrules.md) <br/> |ユーザーのメールボックス内のルールの配列を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetInboxRules](getinboxrules.md)
- [GetInboxRules の操作](getinboxrules-operation.md)

