---
title: EntityExtractionResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 643b99ab-ff90-4411-864c-1077623028d6
description: EntityExtractionResult 要素は、アイテムの EntityExtractionResult プロパティを指定します。
ms.openlocfilehash: b550953233999bfd9c4dc08a7f892e798029df3c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520676"
---
# <a name="entityextractionresult"></a>EntityExtractionResult

**EntityExtractionResult** 要素は、アイテム **の EntityExtractionResult** プロパティを指定します。 
  
```XML
<EntityExtractionResult>
    <Addresses/>
    <MeetingSuggestions/>
    <TaskSuggestions/>
    <EmailAddresses/>
    <Contacts/>
    <Urls/>
    <PhoneNumbers/>
</EntityExtractionResult>
```

 **EntityExtractionResultType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Addresses (ArrayOfAddressEntitiesType)](addresses-arrayofaddressentitiestype.md) <br/> |**AddressEntity 要素の配列を指定** します。  <br/> |
|[MeetingSuggestions](meetingsuggestions.md) <br/> |**MeetingSuggestion 要素の配列を指定** します。  <br/> |
|[TaskSuggestions](tasksuggestions.md) <br/> |**TaskSuggestion 要素の配列を指定** します。  <br/> |
|[EmailAddresses (ArrayOfEmailAddressEntitiesType)](emailaddresses-arrayofemailaddressentitiestype.md) <br/> |電子メール アドレス エンティティの配列を指定します。  <br/> |
|[Contacts (ArrayOfContactsType)](contacts-arrayofcontactstype.md) <br/> |連絡先の配列を指定します。  <br/> |
|[Urls (ArrayOfUrlEntitiesType)](urls-arrayofurlentitiestype.md) <br/> |URL の配列を指定します。  <br/> |
|[PhoneNumbers (ArrayOfPhoneEntitiesType)](phonenumbers-arrayofphoneentitiestype.md) <br/> |電話番号の配列を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Item](item.md) <br/> |ストア内の汎用アイテムをExchangeします。  <br/> |
   
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

