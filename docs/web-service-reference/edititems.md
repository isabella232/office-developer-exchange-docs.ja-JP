---
title: EditItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- EditItems
api_type:
- schema
ms.assetid: 1cb14493-c999-4d66-b82c-ecb410dc1c00
description: EditItems 要素は、ユーザーが編集権限を持つフォルダー内のアイテムを示します。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。
ms.openlocfilehash: 51c038cf93d43fffe785b1946a52c8bcb5c1c302
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538262"
---
# <a name="edititems"></a>EditItems

**EditItems 要素は**、ユーザーが編集権限を持つフォルダー内のアイテムを示します。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。 
  
```xml
<EditItems>None or Owned or All</EditItems>
```

 **PermissionActionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[アクセス許可](permission.md) <br/> |ユーザーがフォルダーに対して持つアクセスを定義します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[CalendarPermission](calendarpermission.md) <br/> |ユーザーが予定表フォルダーに対して持つアクセスを定義します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に **、EditItems 要素に使用できる値を示** します。 
  
**EditItems 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |ユーザーがフォルダー内のアイテムを編集する権限を持たないかどうかを示します。  <br/> |
|Owned (所有)  <br/> |ユーザーがフォルダー内で所有しているアイテムを編集するアクセス許可を持っているかどうかを示します。  <br/> |
|すべて  <br/> |ユーザーがフォルダー内のすべてのアイテムを編集する権限を持っているかどうかを示します。  <br/> |
   
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
- [アクセス許可Folder-Level設定する](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

