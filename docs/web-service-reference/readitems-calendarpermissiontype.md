---
title: ReadItems (CalendarPermissionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ReadItems
api_type:
- schema
ms.assetid: bec01982-26a1-4373-b1e6-2e0c838d83c4
description: ReadItems 要素は、ユーザーが Calendar フォルダー内のアイテムを読み取る権限を持つかどうかを示します。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。
ms.openlocfilehash: a12b5316eaebfdf6d0d70468f172f227db7ab3ef
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519087"
---
# <a name="readitems-calendarpermissiontype"></a>ReadItems (CalendarPermissionType)

**ReadItems 要素** は、ユーザーが Calendar フォルダー内のアイテムを読み取る権限を持つかどうかを示します。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。 
  
```xml
<ReadItems>None or TimeOnly or TimeAndSubjectAndLocation or FullDetails</ReadItems>
```

 **CalendarPermissionReadAccessType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarPermission](calendarpermission.md) <br/> |ユーザーが予定表フォルダーに対して持つアクセスを定義します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に **、ReadItems** 要素に使用できる値を示します。 
  
**ReadItems 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |ユーザーに予定表内のアイテムを表示するアクセス許可が付与されていないかどうかを示します。  <br/> |
|TimeOnly  <br/> |ユーザーが予定表の空き時間のみ表示するアクセス許可を持っているかどうかを示します。  <br/> |
|TimeAndSubjectAndLocation  <br/> |ユーザーが予定表の空き時間情報と予定の件名と場所を表示するアクセス許可を持っているかどうかを示します。  <br/> |
|FullDetails  <br/> |ユーザーが予定表内のすべてのアイテム (空き時間と件名、場所、予定の詳細など) を表示する権限を持っているかどうかを示します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


[アクセス許可Folder-Level設定する](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

