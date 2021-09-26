---
title: IsAssignmentEditable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsAssignmentEditable
api_type:
- schema
ms.assetid: 0ddf9181-f65e-4ad6-ad69-7b074ea0f2e7
description: IsAssignmentEditable 要素は、タスクの種類を表します。
ms.openlocfilehash: 10676cc8c6196a7294f3550856a47dce7d717e6a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544951"
---
# <a name="isassignmenteditable"></a>IsAssignmentEditable

**IsAssignmentEditable 要素は**、タスクの種類を表します。 
  
```xml
<IsAssignmentEditable/>
```

 **integer**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[タスク](task.md) <br/> |ストア内のタスクをExchangeします。  <br/> |
   
## <a name="text-value"></a>テキスト値

このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。 次の表に、使用可能な値を示します。
  
|**値**|**説明**|
|:-----|:-----|
|0  <br/> |すべてのタスク アイテムの既定値。  <br/> |
|1  <br/> |タスク要求。  <br/> |
|2  <br/> |タスク要求の受信者からのタスクの受け入れ。  <br/> |
|3  <br/> |タスク要求の受信者からのタスクの低下。  <br/> |
|4   <br/> |以前のタスク要求の更新。  <br/> |
|5  <br/> |不使用。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

