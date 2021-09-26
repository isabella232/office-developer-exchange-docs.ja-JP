---
title: GroupIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GroupIndex
api_type:
- schema
ms.assetid: 7a596ff7-6cc3-4626-a52c-538a92202337
description: GroupIndex 要素は、FindItem 操作呼び出しの現在の項目グループのアイテムをグループ化するために使用されるプロパティ値を表します。
ms.openlocfilehash: 5e6e2c36e64edec1647c844209d86ceece840b05
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547345"
---
# <a name="groupindex"></a>GroupIndex

**GroupIndex 要素は、FindItem** 操作呼び出しの現在の項目グループのアイテムをグループ化するために使用されるプロパティ [値を表](finditem-operation.md)します。 
  
[FindItemResponse](finditemresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[FindItemResponseMessage](finditemresponsemessage.md)
  
[RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md)
  
[グループ](groups.md)
  
[GroupedItems](groupeditems.md)
  
[GroupIndex](groupindex.md)
  
```xml
<GroupIndex/>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GroupedItems](groupeditems.md) <br/> |グループ化された FindItem 操作呼び出しの結果であるアイテムの [コレクションを表](finditem-operation.md) します。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/FindItemResponse/ResponseMessages/FindItemResponseMessage/RootFolder/Groups/GroupedItems[i]` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。
  
## <a name="remarks"></a>注釈

この要素は [、FindItem 操作応答でのみ発生](finditem-operation.md) します。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[FindItem 操作](finditem-operation.md)


[アイテムの検索](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

