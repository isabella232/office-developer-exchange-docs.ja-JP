---
title: 受信トレイのルール
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InboxRules
api_type:
- schema
ms.assetid: 7bb9896c-bd12-49ae-842a-a10b5f9a2ef6
description: 受信トレイルール要素は、ユーザーのメールボックス内のルールの配列を表します。
ms.openlocfilehash: a3107c3c317a912d0bd3e60d03da4168f2f3a0a9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458272"
---
# <a name="inboxrules"></a>受信トレイのルール

受信**トレイルール**要素は、ユーザーのメールボックス内のルールの配列を表します。 
  
[Get受信規則の応答](getinboxrulesresponse.md)
  
[受信トレイのルール](inboxrules.md)
  
```XML
<InboxRules>
   <Rule/>
</InboxRules>
```

 **ArrayOfRulesType y**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ルール (RuleType)](rule-ruletype.md) <br/> |1つのルールを含み、ユーザーのメールボックス内のルールを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Get受信規則の応答](getinboxrulesresponse.md) <br/> |[Get受信トレイルール操作](getinboxrules-operation.md)要求への応答を定義します。  <br/> |
   
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
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[GetInboxRules](getinboxrules.md)
  
[GetInboxRules の操作](getinboxrules-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

