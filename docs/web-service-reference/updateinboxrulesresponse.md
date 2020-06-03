---
title: Update受信トレイルールの応答
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateInboxRulesResponse
api_type:
- schema
ms.assetid: 0947b6aa-0d95-421b-aebb-d03021ecc110
description: Update受信トレイの Response 要素は、Update受信トレイルール要求への応答を定義します。
ms.openlocfilehash: 1216a32bdaf2dd5211021add0728844eb62089ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455906"
---
# <a name="updateinboxrulesresponse"></a>Update受信トレイルールの応答

**Update受信**トレイの response 要素は、Update受信トレイルール要求への応答を定義します。 
  
```XML
<UpdateInboxRulesResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RuleOperationErrors/>
</UpdateInboxRulesResponse>
```

 **Update受信トレイルール Responsetype**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ResponseClass** <br/> | 登録[解除操作](unsubscribe-operation.md)の応答の状態を表します。<br/><br/> この属性には、次の値が有効です。  <br/><br/>-成功  <br/>-Warning  <br/>-エラー  <br/> |
   
#### <a name="responseclass-attribute-values"></a>ResponseClass 属性の値

|**値**|**説明**|
|:-----|:-----|
|**Success** <br/> |満たされる要求を記述します。  <br/> |
|**Warning** <br/> | 処理されなかった要求を示します。 要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。 <br/><br/>警告のソースの例を次に示します。  <br/><br/>-バッチ処理中に Exchange ストアがオフラインになります。  <br/>-Active Directory ドメインサービス (AD DS) がオフラインになっています。  <br/>-メールボックスは移動されます。  <br/>-メッセージデータベース (MDB) はオフラインです。  <br/>-パスワードの有効期限が切れています。  <br/>-クォータが上限を超えています。  <br/> |
|**Error** <br/> | 満たされない要求を記述します。 <br/><br/>エラーのソースの例を次に示します。  <br/><br/>-無効な属性または要素  <br/>-範囲外の属性または要素  <br/>-不明なタグ  <br/>-コンテキスト内で有効ではない属性または要素  <br/>-クライアントによる権限のないアクセス試行  <br/>-有効なクライアント側の呼び出しに応答した場合のサーバー側障害  <br/> <br/> エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |応答の状態を説明するテキストを提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求に関する状態情報を提供します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在未使用で、今後の使用のために予約されています。 このプロパティには0の値が含まれています。  <br/> |
|[MessageXml](messagexml.md) <br/> |エラー応答に関する追加情報を提供します。  <br/> |
|[RuleOperationErrors](ruleoperationerrors.md) <br/> |エラーが発生した各ルールフィールドのルール検証エラーの配列を表します。  <br/> |
   
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

- [UpdateInboxRules](updateinboxrules.md)
- [UpdateInboxRules の操作](updateinboxrules-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

