---
title: EntityExtractionResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 643b99ab-ff90-4411-864c-1077623028d6
description: EntityExtractionResult 要素は、アイテムの EntityExtractionResult プロパティを指定します。
ms.openlocfilehash: f2f069717a5862adff3349090c35f95499d135f8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456956"
---
# <a name="entityextractionresult"></a>EntityExtractionResult

**Entityextractionresult**要素は、アイテムの**entityextractionresult**プロパティを指定します。 
  
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
|[住所 (ArrayOfAddressEntitiesType)](addresses-arrayofaddressentitiestype.md) <br/> |**Addressentity**要素の配列を指定します。  <br/> |
|[MeetingSuggestions](meetingsuggestions.md) <br/> |**会議提案**要素の配列を指定します。  <br/> |
|[TaskSuggestions](tasksuggestions.md) <br/> |**Tasksuggestion**要素の配列を指定します。  <br/> |
|[EmailAddresses (ArrayOfEmailAddressEntitiesType)](emailaddresses-arrayofemailaddressentitiestype.md) <br/> |電子メールアドレスエンティティの配列を指定します。  <br/> |
|[連絡先 (ArrayOfContactsType)](contacts-arrayofcontactstype.md) <br/> |連絡先の配列を指定します。  <br/> |
|[Url (ArrayOfUrlEntitiesType)](urls-arrayofurlentitiestype.md) <br/> |Url の配列を指定します。  <br/> |
|[PhoneNumbers (ArrayOfPhoneEntitiesType)](phonenumbers-arrayofphoneentitiestype.md) <br/> |電話番号の配列を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Item](item.md) <br/> |Exchange ストア内の汎用アイテムを表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

