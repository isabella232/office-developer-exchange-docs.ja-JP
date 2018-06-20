---
title: PolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fa4b1447-dc7b-47ad-a677-78fcee443dc6
description: PolicyTag 要素は、アイテムまたはフォルダーの保存期間の識別子を指定します。
ms.openlocfilehash: d6cd5aab1145f6006912541c8f8c1d0a91d1e17e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832835"
---
# <a name="policytag"></a>PolicyTag

**PolicyTag**要素は、アイテムまたはフォルダーの保存期間の識別子を指定します。 
  
```xml
<PolicyTag IsExplicit="true | false"></PolicyTag>
```

 **RetentionTagType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|IsExplicit  <br/> |ポリシー タグがアイテムまたはフォルダーに明示的に設定するかどうかを示します。  <br/> の**場合は true** 、 **IsExplicit**属性のテキスト値は、ポリシー タグがアイテムまたはフォルダーを明示的に設定されていることを示します。 **False**のテキスト値は、ポリシー タグがアイテムまたはフォルダーの親フォルダーのポリシー タグに基づいて暗黙的に設定されていることを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[SearchPreviewItem](searchpreviewitem.md) | [アイテム](item.md) | [連絡先](contact.md) | [メッセージ](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [カレンダー項目](calendaritem.md) | [PostItem](postitem.md) | [タスク](task.md)
  
## <a name="text-value"></a>テキスト値

**PolicyTag**要素のテキスト値は、ポリシー タグ識別子です。 ポリシーのタグ識別子は、GUID です。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> ||
   

