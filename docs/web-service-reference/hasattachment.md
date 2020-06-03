---
title: HasAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: de152be6-fc2f-48bc-a05d-1211935da20a
description: HasAttachment 要素は、アイテムに添付ファイルがあるかどうかを示すブール値を指定します。
ms.openlocfilehash: c6bc0932a08a1bbec215bb8a974ed746d2961123
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530262"
---
# <a name="hasattachment"></a>HasAttachment

**Hasattachment**要素は、アイテムに添付ファイルがあるかどうかを示すブール値を指定します。 
  
```XML
<HasAttachment> true | false </HasAttachment
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Searchプレビューアイテム](searchpreviewitem.md) <br/> |アイテムを開かずに、プレビューのメールボックスアイテムの最初の256文字を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**Hasattachment**要素のテキスト値が**true の場合**は、アイテムに添付ファイルがあることを示します。 値が**false**の場合は、アイテムに添付ファイルがないことを示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

