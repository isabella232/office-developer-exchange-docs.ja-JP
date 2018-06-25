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
description: ルール要素は、1 つのルールが含まれていて、ユーザーのメールボックス内のルールを表します。
ms.openlocfilehash: b1f9f058213543633335db11f03729964baf98ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833259"
---
# <a name="rule-ruletype"></a>ルール (RuleType)

**ルール**要素は、1 つのルールが含まれていて、ユーザーのメールボックス内のルールを表します。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[規則 Id](ruleid.md) <br/> |ルールの識別子を指定します。  <br/> |
|[表示名 (文字列)](displayname-string.md) <br/> |ルールの表示名が含まれています。  <br/> |
|[Priority](priority.md) <br/> |ルールの実行順序を示します。  <br/> |
|[有効](isenabled.md) <br/> |ルールが有効になっているかどうかを示します。  <br/> |
|[IsNotSupported](isnotsupported.md) <br/> |Api のマネージ コードでルールを変更できないかどうかを示します。  <br/> |
|[IsInError](isinerror.md) <br/> |ルールがエラー状態かどうかを示します。  <br/> |
|[条件](conditions.md) <br/> |条件を識別するには、満たされるとときに、ルールのルールの処理をトリガーします。  <br/> |
|[Exceptions](exceptions.md) <br/> |受信トレイ ルールの使用可能なルールの例外条件をすべてを表す例外を識別します。  <br/> |
|[アクション](actions.md) <br/> |条件が満たされるときに、メッセージに対して実行されるアクションを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CreateRuleOperation](createruleoperation.md) <br/> |新しいルールを作成する操作を表します。  <br/> |
|[InboxRules](inboxrules.md) <br/> |ユーザーのメールボックスのルールの配列を表します。  <br/> |
|[SetRuleOperation](setruleoperation.md) <br/> |既存のルールを更新する操作を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[UpdateInboxRules](updateinboxrules.md)
  
[SetRuleOperation](setruleoperation.md)
  
[CreateRuleOperation](createruleoperation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

