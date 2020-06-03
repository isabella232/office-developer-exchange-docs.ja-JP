---
title: DeleteRuleOperation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteRuleOperation
api_type:
- schema
ms.assetid: c5e251af-f795-43cc-baaf-95d84475677c
description: DeleteRuleOperation 要素には、既存の受信トレイルールを削除する操作が含まれています。
ms.openlocfilehash: 6b17f7f99f1fd9b9889db00fdf55fba5eef5aba8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526922"
---
# <a name="deleteruleoperation"></a>DeleteRuleOperation

**DeleteRuleOperation**要素には、既存の受信トレイルールを削除する操作が含まれています。 
  
- [UpdateInboxRules](updateinboxrules.md)
- [Operations](operations.md)
  
```XML
<DeleteRuleOperation>
    <RuleId/>
</DeleteRuleOperation>
```

 **DeleteRuleOperationType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[RuleId](ruleid.md) <br/> |削除するルールの識別子を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Operations](operations.md) <br/> |受信トレイに対して実行できるルール操作の配列が含まれています。  <br/> |
   
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
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [UpdateInboxRules](updateinboxrules.md) 
- [SetRuleOperation](setruleoperation.md) 
- [CreateRuleOperation](createruleoperation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

