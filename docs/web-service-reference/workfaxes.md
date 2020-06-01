---
title: ファックス
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 95d115a1-2743-4416-af6f-1ef1be8c4e93
description: 仕事用の Fax 要素は、勤務先の fax 番号の配列と、関連付けられたペルソナのソース attributions の識別子を指定します。
ms.openlocfilehash: d0da5fc2e1b26d14ef3c07f876174da6ccacd016
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459687"
---
# <a name="workfaxes"></a>ファックス

仕事用の**fax**要素は、勤務先の fax 番号の配列と、関連付けられたペルソナのソース attributions の識別子を指定します。 
  
```XML
<WorkFaxes>
   <PhoneNumberAttributedValue/>
</WorkFaxes>
```

 **ArrayOfPhoneNumberAttributedValuesType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[PhoneNumberAttributedValue](phonenumberattributedvalue.md)
  
### <a name="parent-elements"></a>親要素

[ユーザー](persona.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   

