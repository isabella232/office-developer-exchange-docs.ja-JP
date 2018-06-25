---
title: IsQuickContact
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1c9542d6-ef72-4743-828a-bb671e783836
description: IsQuickContact 要素は、基になっている取引先担当者が取引先担当者を簡易であるかどうかを示すブール値を指定します。
ms.openlocfilehash: 979dbd3c0358eacd443eed79b258f7dd6bb9bc7d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832092"
---
# <a name="isquickcontact"></a>IsQuickContact

**IsQuickContact**要素は、基になっている取引先担当者が取引先担当者を簡易であるかどうかを示すブール値を指定します。 
  
```XML
<IsQuickContact>true | false</IsQuickContact>
```

 **boolean**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[属性 (PersonaAttributionType)](attribution-personaattributiontype.md) <br/> |**ペルソナ**の要素の属性の配列のインスタンスを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

の**場合は true** 、 **IsQuickContact**要素のテキスト値は、連絡先がクイック連絡先であることを示します。 **False**の値は、連絡先がクイック連絡先ではないことを示します。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型のスキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

