---
title: Is割り当て編集可能
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
description: Is/編集可能な要素は、タスクの種類を表します。
ms.openlocfilehash: 5eb091b24e2c97f7aa6072044fed998b6c9c1651
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468055"
---
# <a name="isassignmenteditable"></a>Is割り当て編集可能

**Is/編集可能**な要素は、タスクの種類を表します。 
  
```xml
<IsAssignmentEditable/>
```

 **以外**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Task](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。 次の表に、使用可能な値を示します。
  
|**値**|**説明**|
|:-----|:-----|
|.0  <br/> |すべてのタスクアイテムの既定値。  <br/> |
|1   <br/> |仕事の依頼。  <br/> |
|pbm-2  <br/> |タスクの依頼の受信者からのタスクの承諾。  <br/> |
|1/3  <br/> |仕事の依頼の受信者からのタスク declination。  <br/> |
|4   <br/> |以前のタスクの依頼に対する更新。  <br/> |
|5   <br/> |不使用。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

