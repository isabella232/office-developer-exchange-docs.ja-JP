---
title: ConvertHtmlCodePageToUTF8
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f02c8331-0a4e-4d01-adc2-2b93ed838a42
description: ConvertHtmlCodePageToUTF8 要素は、項目の HTML 本文が UTF8 に変換されるかどうかを示します。
ms.openlocfilehash: aff6579835097a273101188c02a9919003b71b58
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759773"
---
# <a name="converthtmlcodepagetoutf8"></a>ConvertHtmlCodePageToUTF8

**ConvertHtmlCodePageToUTF8**要素は、項目の HTML 本文が UTF8 に変換されるかどうかを示します。 
  
```XML
<ConvertHtmlCodePageToUTF8/>
```

 **xs:boolean**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |応答で返されるプロパティのセットを識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

の**場合は true** 、 **ConvertHtmlCodePageToUTF8**要素のテキスト値は、HTML 本文が UTF8 に変換することを示します。 テキスト値が**false**のでは、HTML 本文が UTF8 に変換されないことを示します。 
  
## <a name="remarks"></a>備考

要求に**ConvertHtmlCodePageToUTF8**要素が指定されていない場合、既定値の**true**が使用されます。 
  
この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

