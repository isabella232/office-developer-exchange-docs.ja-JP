---
title: PostalAddressAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 0f92aa41-1499-4d96-a973-24529ec64d24
description: PostalAddressAttributedValue 要素は、住所の配列とその関連付けられた属性のインスタンスを指定します。
ms.openlocfilehash: a4f89b7b2dd54aafe51e0b20da032cc28a90cfeb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519220"
---
# <a name="postaladdressattributedvalue"></a>PostalAddressAttributedValue

**PostalAddressAttributedValue** 要素は、住所の配列とその関連付けられた属性のインスタンスを指定します。 
  
```XML
<PostalAddressAttributedValue>
   <Value/>
   <Attributions/>
</PostalAddressAttributedValue>
```

 **PostalAddressAttributedValueType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[Value (PersonaPostalAddressType)](value-personapostaladdresstype.md)  | [属性 (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md)
  
### <a name="parent-elements"></a>親要素

[BusinessAddresses](businessaddresses.md)  | [HomeAddresses](homeaddresses.md)  | [OtherAddresses](otheraddresses.md)
  
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
   

