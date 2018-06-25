---
title: IsAutomaticForward
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAutomaticForward
api_type:
- schema
ms.assetid: 6876b849-a648-482e-8934-93eb5a0c465f
description: IsAutomaticForward 要素は、受信メッセージに適用する条件または例外の順に自動転送をする必要があるかどうかを示します。
ms.openlocfilehash: c2d44d6dce30cbf55e0c7673aaf41b114a3e2cd4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831989"
---
# <a name="isautomaticforward"></a>IsAutomaticForward

**IsAutomaticForward**要素は、受信メッセージに適用する条件または例外の順に自動転送をする必要があるかどうかを示します。 
  
```XML
<IsAutomaticForward/> true | false</IsAutomaticForward>
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
|[条件](conditions.md) <br/> |条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。  <br/> |
|[Exceptions](exceptions.md) <br/> |受信トレイ ルールの使用可能なルールの例外条件をすべてを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**True**の場合、テキスト値は、メッセージは、[自動転送] を適用する場合の条件または例外の順序のである必要があることを示します。 **False**の値は、メッセージを適用する場合の条件または例外の順序で、自動転送する必要がありますできないことを示します。 
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

