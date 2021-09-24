---
title: DeleteFromFolderStateDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3aba59a0-f12a-48b5-842b-11cf4530dd51
description: DeleteFromFolderStateDefinition 要素は、アイテムがフォルダーから削除される状態を指定します。
ms.openlocfilehash: 270edfc0b7abd70b74ff8c8b4353140ec5fbe27b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510240"
---
# <a name="deletefromfolderstatedefinition"></a>DeleteFromFolderStateDefinition

**DeleteFromFolderStateDefinition 要素は**、アイテムがフォルダーから削除される状態を指定します。 
  
```XML
<DeleteFromFolderStateDefinition>
    <OccurrenceDate></OccurrenceDate>
    <IsOccurrencePresent></IsOccurrencePresent>
</DeleteFromFolderStateDefinition>
```

 **DeleteFromFolderStateDefinitionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Occurrence (タイム ゾーン切り替え)](occurrence-time-zone-transition.md) <br/> |予定表アイテムが出現する日付を指定します。  <br/> |
|[IsOccurrencePresent](isoccurrencepresent.md) <br/> |予定表アイテムが出現するかどうかを示すブール型 (Boolean) の値を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[StateDefinition](statedefinition.md) <br/> |状態定義を指定します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

