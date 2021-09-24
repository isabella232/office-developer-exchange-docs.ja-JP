---
title: Emails2
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 6ad95936-f61b-431a-9d86-df160b5d4b2d
description: Emails2 要素には、EmailAddressAttributedValue 値の配列と、関連付けられたペルサのソース属性の識別子が含まれます。
ms.openlocfilehash: 4f72dc160607bc2b92d25c9e62ea5a73d5f8fc6a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520788"
---
# <a name="emails2"></a>Emails2

**Emails2 要素には****、EmailAddressAttributedValue** 値の配列と、関連付けられたペルサのソース属性の識別子が含まれます。 
  
```XML
<Emails2>
    <EmailAddressAttributedValue></EmailAddressAttributedValue>
</Emails2>
```

 **ArrayOfEmailAddressAttributedValuesType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[EmailAddressAttributedValue](emailaddressattributedvalue.md) <br/> |電子メール アドレスの配列とその関連付けられた属性のインスタンスを指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ユーザー](persona.md) <br/> |**GetPersona** 要求によって返されるペルソナ データのセットを指定します。  <br/> |
   
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

