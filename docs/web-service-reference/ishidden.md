---
title: IsHidden
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2377b584-bd1e-49fc-b80a-a6634721a297
description: IsHidden 要素には、基になるメンバーを非表示またはペルソナの一部として表示するかどうかを示すブール値が含まれています。
ms.openlocfilehash: ee20bf0af287e3cddaedb5bc6d3c63ef9a7a7006
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832032"
---
# <a name="ishidden"></a>IsHidden

**IsHidden**要素には、基になるメンバーを非表示またはペルソナの一部として表示するかどうかを示すブール値が含まれています。 
  
```XML
<IsHidden>true | false</IsHidden>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[属性 (PersonaAttributionType)](attribution-personaattributiontype.md) <br/> |**ペルソナ**の要素の属性の配列のインスタンスを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

の**場合は true** 、 **IsHidden**要素のテキスト値は、基になるメンバーを非表示またはペルソナの一部として表示することを示します。 値が**false**のかを示して連絡先を基になる必要がありますいない非表示に、ペルソナの一部として表示されます。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型のスキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

