---
title: IsHidden
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2377b584-bd1e-49fc-b80a-a6634721a297
description: IsHidden 要素には、基になる連絡先を非表示にするか、ペルソナの一部として表示するかを示すブール値が含まれています。
ms.openlocfilehash: a22628e9ab4a46de04fe395f2d6c1b70083a5c77
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464239"
---
# <a name="ishidden"></a>IsHidden

**IsHidden**要素には、基になる連絡先を非表示にするか、ペルソナの一部として表示するかを示すブール値が含まれています。 
  
```XML
<IsHidden>true | false</IsHidden>
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
|[属性 (PersonaAttributionType)](attribution-personaattributiontype.md) <br/> |**Persona**要素の属性の配列のインスタンスを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**IsHidden**要素のテキスト値が**true**になっている場合は、基になる連絡先を非表示にするか、ペルソナの一部として表示する必要があることを示します。 値が**false**の場合は、基になる連絡先を非表示にしたり、ペルソナの一部として表示したりしないことを示します。 
  
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

