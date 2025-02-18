---
title: ペルソナ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: b115c990-3a2d-4536-9af3-ac1fd06d00dc
description: Persona 要素は、GetPersona 要求によって返されるペルソナ データのセットを指定します。
ms.openlocfilehash: 0bbab94b7767b19a3b27bd240151c2abd42f3e6f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519241"
---
# <a name="persona"></a>ペルソナ

Persona **要素は****、GetPersona** 要求によって返されるペルソナ データのセットを指定します。 
  
```XML
<Persona>
   <PersonaId/>
   <PersonaType/>
   <PersonaObjectStatus/>
   <CreationTime/>
   <Bodies/>
   <DisplayNameFirstLastSortKey/>
   <DisplayNameLastFirstSortKey/>
   <CompanyNameSortKey/>
   <HomeCitySortKey/>
   <WorkCitySortKey/>
   <DisplayNameFirstLastHeader/>
   <DisplayNameLastFirstHeader/>
   <FileAsHeader/>
   <DisplayName/>
   <DisplayNameFirstLast/>
   <DisplayNameLastFirst/>
   <FileAs/>
   <FileAsId/>
   <DisplayNamePrefix/>
   <GivenName/>
   <MiddleName/>
   <Surname/>
   <Generation/>
   <Nickname/>
   <YomiCompanyName/>
   <YomiFirstName/>
   <YomiLastName/>
   <Title/>
   <Department/>
   <CompanyName/>
   <Location/>
   <EmailAddress/>
   <EmailAddresses/>
   <PhoneNumber/>
   <ImAddress/>
   <HomeCity/>
   <WorkCity/>
   <RelevanceScore/>
   <FolderIds/>
   <Attributions/>
   <DisplayNames/>
   <FileAses/>
   <FileAsIds/>
   <DisplayNamePrefixes/>
   <GivenNames/>
   <MiddleNames/>
   <Surnames/>
   <Generations/>
   <Nicknames/>
   <Initials/>
   <YomiCompanyNames/>
   <YomiFirstNames/>
   <YomiLastNames/>
   <BusinessPhoneNumbers/>
   <BusinessPhoneNumbers2/>
   <HomePhones/>
   <HomePhones2/>
   <MobilePhones/>
   <MobilePhones2/>
   <AssistantPhoneNumbers/>
   <CallbackPhones/>
   <CarPhones/>
   <HomeFaxes/>
   <OrganizationMainPhones/>
   <OtherFaxes/>
   <OtherTelephones/>
   <OtherPhones2/>
   <Pagers/>
   <RadioPhones/>
   <TelexNumbers/>
   <TTYTDDPhoneNumbers/>
   <WorkFaxes/>
   <Emails1/>
   <Emails2/>
   <Emails3/>
   <BusinessHomePages/>
   <PersonalHomePages/>
   <OfficeLocations/>
   <ImAddresses/>
   <ImAddresses2/>
   <ImAddresses3/>
   <BusinessAddresses/>
   <HomeAddresses/>
   <OtherAddresses/>
   <Titles/>
   <Departments/>
   <CompanyNames/>
   <Managers/>
   <AssistantNames/>
   <Professions/>
   <SpouseNames/>
   <Children/>
   <Schools/>
   <Hobbies/>
   <WeddingAnniversaries/>
   <Birthdays/>
   <Locations/>
   <ExtendedProperties/>
</Persona>

```

 **PersonaType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[PersonaId](personaid.md)  | [PersonaType](personatype.md)  | [PersonaObjectStatus](personaobjectstatus.md)  | [CreationTime](creationtime.md)  | [Bodies](bodies.md)  | [DisplayNameFirstLastSortKey](displaynamefirstlastsortkey.md)  | [DisplayNameLastFirstSortKey](displaynamelastfirstsortkey.md)  | [CompanyNameSortKey](companynamesortkey.md)  | [HomeCitySortKey](homecitysortkey.md)  | [WorkCitySortKey](workcitysortkey.md)  | [DisplayNameFirstLastHeader](displaynamefirstlastheader.md)  | [DisplayNameLastFirstHeader](displaynamelastfirstheader.md)  | [FileAsHeader](fileasheader.md)  | [DisplayName (string)](displayname-string.md)  | [DisplayNameFirstLast](displaynamefirstlast.md)  | [DisplayNameLastFirst](displaynamelastfirst.md)  | [FileAs](fileas.md)  | [FileAsId](fileasid.md)  | [DisplayNamePrefix](displaynameprefix.md)  | [GivenName](givenname.md)  | [MiddleName](middlename.md)  | [姓](surname.md)  | [ジェネレーション](generation.md)  | [ニックネーム](nickname.md)  | [YomiCompanyName](yomicompanyname.md)  | [YomiFirstName](yomifirstname.md)  | [YomiLastName](yomilastname.md)  | [Title](title.md)  | [部署](department.md)  | [CompanyName](companyname.md)  | [場所](location.md)  | [EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md)  | [EmailAddresses (ArrayOfEmailAddressesType)](emailaddresses-arrayofemailaddressestype.md)  | [PhoneNumber](phonenumber.md)  | [ImAddress (String)](imaddress-string.md)  | [HomeCity](homecity.md)  | [WorkCity](workcity.md)  | [RelevanceScore](relevancescore.md)  | [FolderIds (ArrayOfFolderIdType)](folderids-arrayoffolderidtype.md)  | [属性 (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md)  | [DisplayNames](displaynames.md)  | [FileAses](fileases.md)  | [FileAsIds](fileasids.md)  | [DisplayNamePrefixes](displaynameprefixes.md)  | [GivenNames](givennames.md)  | [MiddleNames](middlenames.md)  | [姓](surnames.md)  | [世代](generations.md)  | [ニックネーム](nicknames.md)  | [Initials (ArrayOfStringAttributedValuesType)](initials-arrayofstringattributedvaluestype.md)  | [YomiCompanyNames](yomicompanynames.md)  | [YomiFirstNames](yomifirstnames.md)  | [YomiLastNames](yomilastnames.md)  | [BusinessPhoneNumbers](businessphonenumbers.md)  | [BusinessPhoneNumbers2](businessphonenumbers2.md)  | [HomePhones](homephones.md)  | [HomePhones2](homephones2.md)  | [MobilePhone](mobilephones.md)  | [MobilePhones2](mobilephones2.md)  | [AssistantPhoneNumbers](assistantphonenumbers.md)  | [CallbackPhones](callbackphones.md)  | [CarPhones](carphones.md)  | [HomeFaxes](homefaxes.md)  | [OrganizationMainPhones](organizationmainphones.md)  | [OtherFaxes](otherfaxes.md)  | [OtherTelephones](othertelephones.md)  | [OtherPhones2](otherphones2.md)  | [Pagers](pagers.md)  | [RadioPhone](radiophones.md)  | [TelexNumbers](telexnumbers.md)  | [TTYTDDPhoneNumbers](ttytddphonenumbers.md)  | [WorkFaxes](workfaxes.md)  | [Emails1](emails1.md)  | [Emails2](emails2.md)  | [Emails3](emails3.md)  | [BusinessHomePages](businesshomepages.md)  | [PersonalHomePages](personalhomepages.md)  | [OfficeLocations](officelocations.md)  | [ImAddresses (ArrayOfStringAttributedValuesType)](imaddresses-arrayofstringattributedvaluestype.md)  | [ImAddresses2](imaddresses2.md)  | [ImAddresses3](imaddresses3.md)  | [BusinessAddresses](businessaddresses.md)  | [HomeAddresses](homeaddresses.md)  | [OtherAddresses](otheraddresses.md)  | [タイトル](titles.md)  | [部署](departments.md)  | [CompanyNames](companynames.md)  | [管理者](managers.md)  | [AssistantNames](assistantnames.md)  | [専門職](professions.md)  | [SpouseNames](spousenames.md)  | [子 (ArrayOfStringArrayAttributedValuesType)](children-arrayofstringarrayattributedvaluestype.md)  | [学校](schools.md)  | [趣味](hobbies.md)  | [WeddingAnniversaries](weddinganniversaries.md)  | [誕生日](birthdays.md)  | [場所](locations.md)  | [ExtendedProperties (ArrayOfExtendedPropertyAttributedValueType)](extendedproperties-arrayofextendedpropertyattributedvaluetype.md)
  
### <a name="parent-elements"></a>親要素

[AddNewImContactToGroupResponse](addnewimcontacttogroupresponse.md)  | [AddNewTelUriContactToGroupResponse](addnewteluricontacttogroupresponse.md)  | [GetPersonaResponseMessage](getpersonaresponsemessage.md)  | [ユーザー](people.md)  | [ペルサ](personas-ex15websvcsotherref.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> |false  <br/> |
   

