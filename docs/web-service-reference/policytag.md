---
title: PolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fa4b1447-dc7b-47ad-a677-78fcee443dc6
description: PolicyTag 要素は、アイテムまたはフォルダーの保持識別子を指定します。
ms.openlocfilehash: 16759748dded6978e68450a6b8d504dd378c04be
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519255"
---
# <a name="policytag"></a>PolicyTag

**PolicyTag 要素** は、アイテムまたはフォルダーの保持識別子を指定します。 
  
```xml
<PolicyTag IsExplicit="true | false"></PolicyTag>
```

 **RetentionTagType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|IsExplicit  <br/> |アイテムまたはフォルダーにポリシー タグが明示的に設定されたかどうかを示します。  <br/> **IsExplicit** 属性のテキスト値 **が true** の場合は、ポリシー タグがアイテムまたはフォルダーに明示的に設定されたかどうかを示します。 false **のテキスト値** は、ポリシー タグが親フォルダー ポリシー タグに基づいてアイテムまたはフォルダーに暗黙的に設定されたかどうかを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[SearchPreviewItem](searchpreviewitem.md)  | [アイテム](item.md)  | [連絡先](contact.md)  | [メッセージ](message-ex15websvcsotherref.md)  | [DistributionList](distributionlist.md)  | [CalendarItem](calendaritem.md)  | [PostItem](postitem.md)  | [タスク](task.md)
  
## <a name="text-value"></a>テキスト値

PolicyTag 要素の **テキスト値** は、ポリシー タグ識別子です。 ポリシー タグ識別子は GUID です。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> ||
   

