---
title: DisplayNamePrefix
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 60363698-7603-4051-a66e-007c02db17cb
description: DisplayNamePrefix 要素は、関連付けられているペルソナの表示名のプレフィックスを指定します。
ms.openlocfilehash: 120a6402be386bc0c11f5859265098324ce4687f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760122"
---
# <a name="displaynameprefix"></a>DisplayNamePrefix

**DisplayNamePrefix**要素は、関連付けられているペルソナの表示名のプレフィックスを指定します。 
  
```xml
<DisplayNamePrefix></DisplayNamePrefix>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ペルソナ](persona.md) <br/> |**GetPersona**の要求によって返されるペルソナ データのセットを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**DisplayNamePrefix**要素のテキスト値は、表示名のプレフィックスを指定する文字列値です。 
  
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

