---
title: Emails2
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6ad95936-f61b-431a-9d86-df160b5d4b2d
description: Emails2 要素には、EmailAddressAttributedValue の値の配列と関連付けられているペルソナにそのソースの帰属の識別子が含まれています。
ms.openlocfilehash: 1767d6bfaee335717e33e0345c605025a073335c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760237"
---
# <a name="emails2"></a>Emails2

**Emails2**要素には、 **EmailAddressAttributedValue**の値の配列と関連付けられているペルソナにそのソースの帰属の識別子が含まれています。 
  
```XML
<Emails2>
    <EmailAddressAttributedValue></EmailAddressAttributedValue>
</Emails2>
```

 **ArrayOfEmailAddressAttributedValuesType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[EmailAddressAttributedValue](emailaddressattributedvalue.md) <br/> |電子メール アドレスと関連付けられている、帰属の配列のインスタンスを指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ペルソナ](persona.md) <br/> |**GetPersona**の要求によって返されるペルソナ データのセットを指定します。  <br/> |
   
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

