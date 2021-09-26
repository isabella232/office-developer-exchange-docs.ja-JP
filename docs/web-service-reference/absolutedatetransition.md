---
title: AbsoluteDateTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AbsoluteDateTransition
api_type:
- schema
ms.assetid: 8f5731eb-bed0-45bf-ba89-4aaf20c34a39
description: AbsoluteDateTransition 要素は、特定の日付と特定の時刻に発生するタイム ゾーン遷移を表します。
ms.openlocfilehash: c0d4e28d8ecefaaa72ded50ab3022666d74ce479
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542548"
---
# <a name="absolutedatetransition"></a>AbsoluteDateTransition

**AbsoluteDateTransition 要素** は、特定の日付と特定の時刻に発生するタイム ゾーン遷移を表します。 
  
```xml
<AbsoluteDateTransition>
   <To/>
   <DateTime/>
</AbsoluteDateTransition>
```

**AbsoluteDateTransitionType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[To](to.md) <br/> |タイム ゾーン遷移 [の](period.md) ターゲットである Period または [TransitionsGroup](transitionsgroup.md) を指定します。  <br/> |
|[DateTime](datetime.md) <br/> |タイム ゾーンの切り替えが発生する日時を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Transitions](transitions.md) <br/> |タイム ゾーンの切り替えのコレクションを表します。  <br/> |
|[TransitionsGroup](transitionsgroup.md) <br/> |タイム ゾーンの切り替えのコレクションを表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

