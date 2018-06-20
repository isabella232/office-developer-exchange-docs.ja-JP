---
title: PostalAddressAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0f92aa41-1499-4d96-a973-24529ec64d24
description: PostalAddressAttributedValue 要素は、アドレスの郵便番号の配列と、関連付けられている帰属のインスタンスを指定します。
ms.openlocfilehash: f2b8b9818e39780b934522910d016875dbe5af2e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832854"
---
# <a name="postaladdressattributedvalue"></a>PostalAddressAttributedValue

**PostalAddressAttributedValue**要素は、アドレスの郵便番号の配列と、関連付けられている帰属のインスタンスを指定します。 
  
```XML
<PostalAddressAttributedValue>
   <Value/>
   <Attributions/>
</PostalAddressAttributedValue>
```

 **PostalAddressAttributedValueType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[値 (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [(ArrayOfValueAttributionsType) の帰属](attributions-arrayofvalueattributionstype.md)
  
### <a name="parent-elements"></a>親要素

[BusinessAddresses](businessaddresses.md) | [HomeAddresses](homeaddresses.md) | [OtherAddresses](otheraddresses.md)
  
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
   

