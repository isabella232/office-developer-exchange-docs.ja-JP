---
title: Phone
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 9381d8e0-b705-49fd-a822-00fb485bdbab
description: '[電話] 要素は、連絡先エンティティの抽出に基く単一の電話番号を指定します。'
ms.openlocfilehash: fa9e0be88c2142b30304c3c5b758624fa73da7d1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528361"
---
# <a name="phone"></a>Phone

**[電話]** 要素は、連絡先エンティティ抽出の結果として 1 つの電話番号を指定します。 
  
```XML
<Phone>
   <OriginalPhoneString/>
   <PhoneString/>
   <Type/>
</Phone>
```

 **PhoneType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[OriginalPhoneString](originalphonestring.md)  | [PhoneString](phonestring.md)  | [型 (文字列)](type-string.md)
  
### <a name="parent-elements"></a>親要素

[PhoneNumbers (ArrayOfPhonesType)](phonenumbers-arrayofphonestype.md)
  
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
   

