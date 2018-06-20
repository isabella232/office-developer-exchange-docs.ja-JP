---
title: ReadItems (CalendarPermissionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReadItems
api_type:
- schema
ms.assetid: bec01982-26a1-4373-b1e6-2e0c838d83c4
description: ReadItems 要素は、ユーザーが予定表フォルダー内のアイテムの読み取りアクセス許可を持っているかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 532b90c47cca7117a89d59e7012436268be9ebb0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832964"
---
# <a name="readitems-calendarpermissiontype"></a>ReadItems (CalendarPermissionType)

**ReadItems**要素は、ユーザーが予定表フォルダー内のアイテムの読み取りアクセス許可を持っているかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
```xml
<ReadItems>None or TimeOnly or TimeAndSubjectAndLocation or FullDetails</ReadItems>
```

 **CalendarPermissionReadAccessType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarPermission](calendarpermission.md) <br/> |予定表フォルダーにユーザーが持つアクセス権を定義します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

**ReadItems**要素の有効な値を次の表に一覧します。 
  
**ReadItems 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |ユーザーに予定表にアイテムを表示する権限がないことを示します。  <br/> |
|TimeOnly  <br/> |ユーザーが予定表の空き時間のみを表示する権限を持っていることを示します。  <br/> |
|TimeAndSubjectAndLocation  <br/> |ユーザーが予定表、件名、予定の場所に空き時間情報を表示するアクセス許可を持っていることを示します。  <br/> |
|FullDetails  <br/> |ユーザーが空き時間情報、件名、場所、および予定の詳細情報を含む、予定表のすべての項目を表示する権限を持っていることを示します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


[フォルダー レベルのアクセス許可の設定](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

