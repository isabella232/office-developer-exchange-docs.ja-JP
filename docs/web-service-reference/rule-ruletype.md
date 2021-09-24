---
title: Rule (RuleType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Rule
api_type:
- schema
ms.assetid: 259a1f62-b235-4964-88bf-2d1f1c05a563
description: Rule 要素には 1 つのルールが含まれるので、ユーザーのメールボックス内のルールを表します。
ms.openlocfilehash: 0e7d7284d561ea374f66106072df0c4f850c590c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527517"
---
# <a name="rule-ruletype"></a>Rule (RuleType)

**Rule 要素** には 1 つのルールが含まれるので、ユーザーのメールボックス内のルールを表します。 
  
```XML
<Rule>
    <RuleId>
    <DisplayName>
    <Priority>
    <IsEnabled>
    <IsNotSupported>
    <IsInError>
    <Conditions>
    <Exceptions>
    <Actions>
</Rule>
```

 **RuleType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[RuleId](ruleid.md) <br/> |ルール識別子を指定します。  <br/> |
|[DisplayName (string)](displayname-string.md) <br/> |ルールの表示名を含む。  <br/> |
|[優先度](priority.md) <br/> |ルールを実行する順序を示します。  <br/> |
|[IsEnabled](isenabled.md) <br/> |ルールが有効かどうかを示します。  <br/> |
|[IsNotSupported](isnotsupported.md) <br/> |マネージ コード API でルールを変更できないかどうかを示します。  <br/> |
|[IsInError](isinerror.md) <br/> |ルールがエラー状態かどうかを示します。  <br/> |
|[条件](conditions.md) <br/> |満たされると、ルールのルール アクションをトリガーする条件を識別します。  <br/> |
|[例外](exceptions.md) <br/> |受信トレイ ルールで使用可能なすべてのルール例外条件を表す例外を識別します。  <br/> |
|[Actions](actions.md) <br/> |条件が満たされた場合にメッセージに対して実行されるアクションを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CreateRuleOperation](createruleoperation.md) <br/> |新しいルールを作成する操作を表します。  <br/> |
|[InboxRules](inboxrules.md) <br/> |ユーザーのメールボックス内のルールの配列を表します。  <br/> |
|[SetRuleOperation](setruleoperation.md) <br/> |既存のルールを更新する操作を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[UpdateInboxRules](updateinboxrules.md)
  
[SetRuleOperation](setruleoperation.md)
  
[CreateRuleOperation](createruleoperation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

