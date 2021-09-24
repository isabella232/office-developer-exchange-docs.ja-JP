---
title: Contact (ContactType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 7f7119b7-f5b4-484d-a7de-fa74836d9aee
description: Contact 要素は、統合連絡先ストア内の連絡先を指定します。
ms.openlocfilehash: e52573841f934a11c05a1da9e19f91146ed9c774
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511994"
---
# <a name="contact-contacttype"></a>Contact (ContactType)

**Contact 要素** は、統合連絡先ストア内の連絡先を指定します。 
  
```XML
<Contact>
    <PersonName></PersonName>
    <BusinessName></BusinessName>
    <PhoneNumbers></PhoneNumbers>
    <Urls></Urls>
    <EmailAddresses></EmailAddresses>
    <Addresses></Addesses>    <ContactString></ContactString
</Contact>
```

 **ContactType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[PersonName](personname.md) <br/> |個人の名前を指定します。  <br/> |
|[BusinessName](businessname.md) <br/> |ビジネスの名前を指定します。  <br/> |
|[PhoneNumbers](phonenumbers.md) <br/> |連絡先の電話番号のコレクションを表します。  <br/> |
|[Urls](urls.md) <br/> |ペルサの URL の配列を指定します。  <br/> |
|[EmailAddresses (ArrayOfExtractedEmailAddresses)](emailaddresses-arrayofextractedemailaddresses.md) <br/> |抽出された電子メール アドレスの配列を指定します。  <br/> |
|[Addresses (ArrayOfAddressesType)](addresses-arrayofaddressestype.md) <br/> |Address 要素の配列 **を指定** します。  <br/> |
|[ContactString](contactstring.md) <br/> |連絡先の表示名を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Contacts (ArrayOfContactsType)](contacts-arrayofcontactstype.md) <br/> |連絡先の配列を指定します。  <br/> |
   
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

