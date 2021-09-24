---
title: FormattedAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 643f8663-1fab-4625-a7e9-5724e352972b
description: FormattedAddress 要素は、関連付けられた郵送先住所の書式設定された表示値を指定します。
ms.openlocfilehash: 379b02a4ed667ec1a01b54f26dd6d58c7f66fa89
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535106"
---
# <a name="formattedaddress"></a>FormattedAddress

**FormattedAddress** 要素は、関連付けられた郵送先住所の書式設定された表示値を指定します。 
  
```XML
<FormattedAddress></FormattedAddress>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Value (PersonaPostalAddressType)](value-personapostaladdresstype.md) <br/> |郵便番号に関連付けられている情報を指定します。  <br/> |
|[PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md) <br/> |場所の郵便番号を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**FormattedAddress 要素のテキスト** 値は、書式設定されたアドレスを指定する文字列値です。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

