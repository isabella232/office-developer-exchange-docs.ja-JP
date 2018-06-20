---
title: EntityExtractionResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 643b99ab-ff90-4411-864c-1077623028d6
description: EntityExtractionResult 要素は、項目の EntityExtractionResult プロパティを指定します。
ms.openlocfilehash: ef99629beb95f1e1123569fa99e3f495c1b56e95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760313"
---
# <a name="entityextractionresult"></a>EntityExtractionResult

**EntityExtractionResult**要素は、項目の**EntityExtractionResult**プロパティを指定します。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[アドレス (ArrayOfAddressEntitiesType)](addresses-arrayofaddressentitiestype.md) <br/> |**AddressEntity**要素の配列を指定します。  <br/> |
|[MeetingSuggestions](meetingsuggestions.md) <br/> |**MeetingSuggestion**要素の配列を指定します。  <br/> |
|[TaskSuggestions](tasksuggestions.md) <br/> |**TaskSuggestion**要素の配列を指定します。  <br/> |
|[EmailAddresses (ArrayOfEmailAddressEntitiesType)](emailaddresses-arrayofemailaddressentitiestype.md) <br/> |E メール アドレスのエンティティの配列を指定します。  <br/> |
|[連絡先 (ArrayOfContactsType)](contacts-arrayofcontactstype.md) <br/> |メンバーの配列を指定します。  <br/> |
|[Url (ArrayOfUrlEntitiesType)](urls-arrayofurlentitiestype.md) <br/> |Url の配列を指定します。  <br/> |
|[PhoneNumbers (ArrayOfPhoneEntitiesType)](phonenumbers-arrayofphoneentitiestype.md) <br/> |電話番号の配列を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Item](item.md) <br/> |Exchange ストア内の一般的な項目を表します。  <br/> |
   
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

