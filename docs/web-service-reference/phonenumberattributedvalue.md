---
title: PhoneNumberAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8bf16552-b672-424a-91b6-6470e20a49ad
description: PhoneNumberAttributedValue 要素は、電話番号の配列のインスタンスと、それに関連付けられている attributions を指定します。
ms.openlocfilehash: b1597ea33973d0dde5bd528061cf732101582c9d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465626"
---
# <a name="phonenumberattributedvalue"></a>PhoneNumberAttributedValue

**PhoneNumberAttributedValue**要素は、電話番号の配列のインスタンスと、それに関連付けられている attributions を指定します。 
  
```XML
<PhoneNumberAttributedValue>
   <Value/>
   <Attributions/>
</PhoneNumberAttributedValue>
```

 **PhoneNumberAttributedValueType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[Value (PersonaPhoneNumberType)](value-personaphonenumbertype.md)  | [Attributions (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md)
  
### <a name="parent-elements"></a>親要素

[BusinessPhoneNumbers](businessphonenumbers.md)  | [BusinessPhoneNumbers2](businessphonenumbers2.md)  | [ホーム電話](homephones.md)  | [HomePhones2](homephones2.md)  | [MobilePhones](mobilephones.md)  | [MobilePhones2](mobilephones2.md)  | [AssistantPhoneNumbers](assistantphonenumbers.md)  | [電話機](callbackphones.md)  | [カーフォン](carphones.md)  | [ホーム fax](homefaxes.md)  | [組織のメイン電話](organizationmainphones.md)  | その[他の fax](otherfaxes.md)  | [Othertelephones](othertelephones.md)  | [OtherPhones2](otherphones2.md)  | [ポケットベル](pagers.md)  | [RadioPhones](radiophones.md)  | [Telexnumbers](telexnumbers.md)  | [TTYTDDPhoneNumbers](ttytddphonenumbers.md)  | [ファックス](workfaxes.md)
  
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
   

