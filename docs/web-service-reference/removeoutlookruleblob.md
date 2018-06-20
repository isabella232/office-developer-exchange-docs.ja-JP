---
title: RemoveOutlookRuleBlob
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveOutlookRuleBlob
api_type:
- schema
ms.assetid: 69614475-8bd3-4475-b988-614fe9cad8ef
description: RemoveOutlookRuleBlob 要素では、Microsoft Outlook のルールの blob を削除するかどうかを示します。
ms.openlocfilehash: 45336e296c39161704ce6e0d51fba1d2c61797b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833102"
---
# <a name="removeoutlookruleblob"></a>RemoveOutlookRuleBlob

**RemoveOutlookRuleBlob**要素では、Microsoft Outlook のルールの blob を削除するかどうかを示します。 
  
[UpdateInboxRules](updateinboxrules.md)
  
[RemoveOutlookRuleBlob](removeoutlookruleblob.md)
  
```XML
<RemoveOutlookRuleBlob>true | false</RemoveOutlookRuleBlob>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[UpdateInboxRules](updateinboxrules.md) <br/> |サーバー ストア内のメールボックスの受信トレイ ルールを更新する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**True**の場合、テキスト値は、Outlook のルールの blob を削除する必要があることを示します。 テキスト値が**false**のでは、Outlook のルールの blob を削除されないことを示します。 
  
## <a name="remarks"></a>備考

**True**に、受信トレイ ルールの更新プログラムでは、この要素を設定します。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[UpdateInboxRules の操作](updateinboxrules-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

