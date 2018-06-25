---
title: ConflictResults
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConflictResults
api_type:
- schema
ms.assetid: 08cdd547-4de7-4c7a-b60f-e618dc217d20
description: ConflictResults 要素には、競合 UpdateItem 操作の応答の数が含まれています。
ms.openlocfilehash: faa6dc6c5fbbe874438a89c810a12fa675e8a1c9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759657"
---
# <a name="conflictresults"></a>ConflictResults

[ConflictResults](conflictresults.md)要素には、競合[UpdateItem 操作](updateitem-operation.md)の応答の数が含まれています。 
  
[UpdateItemResponse](updateitemresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[UpdateItemResponseMessage](updateitemresponsemessage.md)
  
[ConflictResults](conflictresults.md)
  
```xml
<ConflictResults>
   <Count/>
</ConflictResults>
```

 **ConflictResultsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[Count](count.md) <br/> |[UpdateItem 操作](updateitem-operation.md)の応答の競合の数が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[UpdateItem 操作](updateitem-operation.md)を要求します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割と Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目




  [UpdateItem 操作](updateitem-operation.md)
  
 **ConflictResultsType**

