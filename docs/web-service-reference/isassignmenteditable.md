---
title: IsAssignmentEditable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAssignmentEditable
api_type:
- schema
ms.assetid: 0ddf9181-f65e-4ad6-ad69-7b074ea0f2e7
description: IsAssignmentEditable 要素は、タスクの種類を表します。
ms.openlocfilehash: 91922c4d6abd4d88ac9e36dd3d4c0224fc1ee716
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831992"
---
# <a name="isassignmenteditable"></a>IsAssignmentEditable

**IsAssignmentEditable**要素は、タスクの種類を表します。 
  
```xml
<IsAssignmentEditable/>
```

 **整数**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

このプロパティは値の取得のみ可能です。 次の表は、可能な値を一覧します。
  
|**値**|**説明**|
|:-----|:-----|
|0  <br/> |すべての作業項目の既定値です。  <br/> |
|1  <br/> |仕事の依頼です。  <br/> |
|2  <br/> |仕事の依頼の受信者からの仕事の承諾します。  <br/> |
|3  <br/> |仕事の依頼の受信者からのタスクの拒否します。  <br/> |
|4  <br/> |前の仕事の依頼を更新します。  <br/> |
|5  <br/> |使用されません。  <br/> |
   
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

