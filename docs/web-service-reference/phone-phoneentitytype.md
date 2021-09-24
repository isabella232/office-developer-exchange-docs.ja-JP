---
title: Phone (PhoneEntityType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f6925cc9-7f22-478f-b9ba-b77575772471
description: 電話要素は、電話番号エンティティの抽出に基く単一の電話番号を指定します。
ms.openlocfilehash: a8f0404c2cb9f141bf818dfe2fd07d3f4b1dacb8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528477"
---
# <a name="phone-phoneentitytype"></a>Phone (PhoneEntityType)

電話 **要素** は、電話番号エンティティ抽出の結果として 1 つの電話番号を指定します。 
  
```XML
<Phone>
   <Position/>
   <OriginalPhoneString/>
   <PhoneString/>
   <Type/>
</Phone>
```

 **PhoneEntityType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[位置](position.md)  | [OriginalPhoneString](originalphonestring.md)  | [PhoneString](phonestring.md)  | [型 (文字列)](type-string.md)
  
### <a name="parent-elements"></a>親要素

[PhoneNumbers (ArrayOfPhoneEntitiesType)](phonenumbers-arrayofphoneentitiestype.md)
  
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
   

