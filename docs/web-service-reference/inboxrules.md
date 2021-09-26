---
title: InboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- InboxRules
api_type:
- schema
ms.assetid: 7bb9896c-bd12-49ae-842a-a10b5f9a2ef6
description: InboxRules 要素は、ユーザーのメールボックス内のルールの配列を表します。
ms.openlocfilehash: 6b6b399f685accca90fbaffd3ed461aa43a3c2b3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547233"
---
# <a name="inboxrules"></a>InboxRules

**InboxRules 要素** は、ユーザーのメールボックス内のルールの配列を表します。 
  
[GetInboxRulesResponse](getinboxrulesresponse.md)
  
[InboxRules](inboxrules.md)
  
```XML
<InboxRules>
   <Rule/>
</InboxRules>
```

 **ArrayOfRulesType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Rule (RuleType)](rule-ruletype.md) <br/> |1 つのルールを含み、ユーザーのメールボックス内のルールを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |[GetInboxRules 操作要求への応答を定義](getinboxrules-operation.md)します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[GetInboxRules](getinboxrules.md)
  
[GetInboxRules の操作](getinboxrules-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

