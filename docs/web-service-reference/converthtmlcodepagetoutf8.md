---
title: ConvertHtmlCodePageToUTF8
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f02c8331-0a4e-4d01-adc2-2b93ed838a42
description: ConvertHtmlCodePageToUTF8 要素は、アイテムの HTML 本文が UTF8 に変換されるかどうかを示します。
ms.openlocfilehash: a714eacd8cc105146a1471f062ec35dc16730d61
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457593"
---
# <a name="converthtmlcodepagetoutf8"></a>ConvertHtmlCodePageToUTF8

**ConvertHtmlCodePageToUTF8**要素は、アイテムの HTML 本文が UTF8 に変換されるかどうかを示します。 
  
```XML
<ConvertHtmlCodePageToUTF8/>
```

 **xs: boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |応答で返される一連のプロパティを識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**ConvertHtmlCodePageToUTF8**要素のテキスト値が**true**の場合は、HTML 本文が UTF8 に変換されることを示します。 テキスト値が**false**の場合は、HTML 本文が UTF8 に変換されないことを示します。 
  
## <a name="remarks"></a>注釈

**ConvertHtmlCodePageToUTF8**要素が要求で指定されていない場合は、既定値の**true**が使用されます。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

