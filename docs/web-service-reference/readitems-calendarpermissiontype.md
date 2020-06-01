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
description: ReadItems 要素は、ユーザーが予定表フォルダー内のアイテムを読み取る権限を持っているかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: e040b643016781f9f890050f189191356f8d4f0b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468300"
---
# <a name="readitems-calendarpermissiontype"></a>ReadItems (CalendarPermissionType)

**ReadItems**要素は、ユーザーが予定表フォルダー内のアイテムを読み取る権限を持っているかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
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
|[CalendarPermission](calendarpermission.md) <br/> |ユーザーが予定表フォルダーに対して持っているアクセス権を定義します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に、 **ReadItems**要素に指定できる値を示します。 
  
**ReadItems 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |ユーザーが予定表のアイテムを表示する権限を持っていないことを示します。  <br/> |
|TimeOnly  <br/> |ユーザーが予定表の空き時間情報のみを表示するアクセス許可を持っていることを示します。  <br/> |
|TimeAndSubjectAndLocation  <br/> |ユーザーが予定表の空き時間情報を表示するためのアクセス許可と、予定の件名と場所を表示できることを示します。  <br/> |
|FullDetails  <br/> |ユーザーが予定表のすべてのアイテムを表示するためのアクセス許可を持っていることを示します。空き時間情報、件名、場所、および予定の詳細が含まれます。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


[フォルダーレベルのアクセス許可を設定する](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

