---
title: IsQuickContact
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 1c9542d6-ef72-4743-828a-bb671e783836
description: IsQuickContact 要素は、基になる連絡先がクイック連絡先であるかどうかを示すブール値を指定します。
ms.openlocfilehash: 7821332e685b44983787ce05cc6b6ef4250ee01d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509687"
---
# <a name="isquickcontact"></a>IsQuickContact

**IsQuickContact** 要素は、基になる連絡先がクイック連絡先であるかどうかを示すブール値を指定します。 
  
```XML
<IsQuickContact>true | false</IsQuickContact>
```

 **boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Attribution (PersonaAttributionType)](attribution-personaattributiontype.md) <br/> |**Persona** 要素の属性の配列内のインスタンスを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**IsQuickContact** 要素のテキスト値 **が true** の場合は、連絡先がクイック連絡先です。 false の **値は** 、連絡先がクイック連絡先ではないかどうかを示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> |false  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

