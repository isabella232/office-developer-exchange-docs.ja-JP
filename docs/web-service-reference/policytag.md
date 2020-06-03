---
title: PolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fa4b1447-dc7b-47ad-a677-78fcee443dc6
description: PolicyTag 要素は、アイテムまたはフォルダーの保持識別子を指定します。
ms.openlocfilehash: ddc4d890d1e514586ba5ea7f6a8b541b2e4786c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460898"
---
# <a name="policytag"></a>PolicyTag

**Policytag**要素は、アイテムまたはフォルダーの保持識別子を指定します。 
  
```xml
<PolicyTag IsExplicit="true | false"></PolicyTag>
```

 **RetentionTagType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|IsExplicit  <br/> |アイテムまたはフォルダーにポリシータグが明示的に設定されているかどうかを示します。  <br/> **IsExplicit**属性のテキスト値が**true の場合**は、ポリシータグがアイテムまたはフォルダーに明示的に設定されていることを示します。 テキスト値が**false**の場合は、親フォルダーポリシータグに基づいてアイテムまたはフォルダーにポリシータグが暗黙的に設定されていることを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[Searchプレビューアイテム](searchpreviewitem.md)  | [アイテム](item.md)  | [連絡先](contact.md)  | [メッセージ](message-ex15websvcsotherref.md)  | [DistributionList](distributionlist.md)  | [Calendaritem](calendaritem.md)  | [Postitem](postitem.md)  | [タスク](task.md)
  
## <a name="text-value"></a>テキスト値

**Policytag**要素のテキスト値は、ポリシータグ識別子です。 ポリシータグ識別子は GUID です。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   

