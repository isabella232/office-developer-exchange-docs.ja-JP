---
title: 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Operations
api_type:
- schema
ms.assetid: d8cd41b1-28ae-4c95-9ff6-8b25c8e18306
description: 操作要素には、受信トレイで実行可能なルール操作の配列が含まれています。
ms.openlocfilehash: 1030703d5e496be391d557e99e1420f9fddfdb36
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832655"
---
# <a name="operations"></a>操作

**操作**要素には、受信トレイで実行可能なルール操作の配列が含まれています。 
  
[UpdateInboxRules](updateinboxrules.md)
  
```XML
<Operations>
    <CreateRuleOperation/>
    <SetRuleOperation/>
    <DeleteRuleOperation/>
</Operations>
```

 **ArrayOfRuleOperationsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[CreateRuleOperation](createruleoperation.md) <br/> |新しい受信トレイ ルールを作成する操作を表します。  <br/> |
|[SetRuleOperation](setruleoperation.md) <br/> |受信トレイ ルールを更新する操作を表します。  <br/> |
|[DeleteRuleOperation](deleteruleoperation.md) <br/> |受信トレイ ルールを削除する操作を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[UpdateInboxRules](updateinboxrules.md) <br/> |サーバー ストア内のメールボックスの受信トレイ ルールを更新する要求を定義します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[UpdateInboxRules の操作](updateinboxrules-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

