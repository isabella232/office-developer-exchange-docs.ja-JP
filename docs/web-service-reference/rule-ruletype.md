---
title: ルール (RuleType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Rule
api_type:
- schema
ms.assetid: 259a1f62-b235-4964-88bf-2d1f1c05a563
description: Rule 要素には、1つのルールが含まれており、ユーザーのメールボックス内のルールを表します。
ms.openlocfilehash: cdbd21df235a62a9e201e1eaae1d82a8ac10cdd2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465080"
---
# <a name="rule-ruletype"></a>ルール (RuleType)

**Rule**要素には、1つのルールが含まれており、ユーザーのメールボックス内のルールを表します。 
  
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
|[DisplayName (文字列)](displayname-string.md) <br/> |ルールの表示名を含みます。  <br/> |
|[[優先度]](priority.md) <br/> |ルールを実行する順序を示します。  <br/> |
|[IsEnabled](isenabled.md) <br/> |ルールが有効になっているかどうかを示します。  <br/> |
|[IsNotSupported](isnotsupported.md) <br/> |マネージコード Api でルールを変更できないかどうかを示します。  <br/> |
|[IsInError](isinerror.md) <br/> |ルールがエラー状態かどうかを示します。  <br/> |
|[条件](conditions.md) <br/> |[処理時] がルールのルールの処理をトリガーする条件を指定します。  <br/> |
|[例外](exceptions.md) <br/> |受信トレイルールの使用可能なルールの例外条件をすべて表す例外を識別します。  <br/> |
|[Actions](actions.md) <br/> |条件が満たされたときにメッセージに対して実行されるアクションを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CreateRuleOperation](createruleoperation.md) <br/> |新しいルールを作成する操作を表します。  <br/> |
|[受信トレイのルール](inboxrules.md) <br/> |ユーザーのメールボックス内のルールの配列を表します。  <br/> |
|[SetRuleOperation](setruleoperation.md) <br/> |既存のルールを更新する操作を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[UpdateInboxRules](updateinboxrules.md)
  
[SetRuleOperation](setruleoperation.md)
  
[CreateRuleOperation](createruleoperation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

