---
title: ペルソナ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b115c990-3a2d-4536-9af3-ac1fd06d00dc
description: Persona 要素は、GetPersona 要求によって返される一連のペルソナデータを指定します。
ms.openlocfilehash: 093b346300b5fdcbfb31f2e1240d57d9476e250a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465878"
---
# <a name="persona"></a>ペルソナ

**Persona**要素は、 **getpersona**要求によって返される一連のペルソナデータを指定します。 
  
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

 **個人の Atype**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[個人補助](personaid.md)  | [個人の atype](personatype.md)  | [個人情報](personaobjectstatus.md)  | [前回の時間](creationtime.md)  | [本文](bodies.md)  | [Displaynamefirstlastsortkey](displaynamefirstlastsortkey.md)  | [Displaynamelastfirstsortkey](displaynamelastfirstsortkey.md)  | 会社の[Namesortkey](companynamesortkey.md)  | [HomeCitySortKey](homecitysortkey.md)  | [WorkCitySortKey](workcitysortkey.md)  | [DisplayNameFirstLastHeader](displaynamefirstlastheader.md)  | [DisplayNameLastFirstHeader](displaynamelastfirstheader.md)  | [Fileasheader](fileasheader.md)  | [DisplayName (文字列)](displayname-string.md)  | [Displaynamefirstlast](displaynamefirstlast.md)  | [Displaynamelastfirst](displaynamelastfirst.md)  | [FileAs](fileas.md)  | [Fileasid](fileasid.md)  | [Displaynameprefix](displaynameprefix.md)  | [GivenName](givenname.md)  | [ミドルネーム](middlename.md)  | [姓](surname.md)  | [生成](generation.md)  | [ニックネーム](nickname.md)  | [YomiCompanyName](yomicompanyname.md)  | [ヨーク Mifirstname](yomifirstname.md)  | [YomiLastName](yomilastname.md)  | [タイトル](title.md)  | [Department](department.md)  | [CompanyName](companyname.md)  | [場所](location.md)  | [EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md)  | [Emailaddresses (ArrayOfEmailAddressesType)](emailaddresses-arrayofemailaddressestype.md)  | [PhoneNumber](phonenumber.md)  | [Imaddress (文字列)](imaddress-string.md)  | [HomeCity](homecity.md)  | [勤務先市区町村](workcity.md)  | [RelevanceScore](relevancescore.md)  | [FolderIds (ArrayOfFolderIdType)](folderids-arrayoffolderidtype.md)  | [Attributions (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md)  | [Displaynames](displaynames.md)  | [Fileases](fileases.md)  | [Fileasids](fileasids.md)  | [Displaynameprefixes](displaynameprefixes.md)  | 与えた[名前](givennames.md)  | [MiddleNames](middlenames.md)  | [Surnames](surnames.md)  | [Generation](generations.md)  | [ニックネーム](nicknames.md)  | [イニシャル (ArrayOfStringAttributedValuesType)](initials-arrayofstringattributedvaluestype.md)  | [YomiCompanyNames](yomicompanynames.md)  | [ヨーク Mifirstnames](yomifirstnames.md)  | [YomiLastNames](yomilastnames.md)  | [BusinessPhoneNumbers](businessphonenumbers.md)  | [BusinessPhoneNumbers2](businessphonenumbers2.md)  | [ホーム電話](homephones.md)  | [HomePhones2](homephones2.md)  | [MobilePhones](mobilephones.md)  | [MobilePhones2](mobilephones2.md)  | [AssistantPhoneNumbers](assistantphonenumbers.md)  | [電話機](callbackphones.md)  | [カーフォン](carphones.md)  | [ホーム fax](homefaxes.md)  | [組織のメイン電話](organizationmainphones.md)  | その[他の fax](otherfaxes.md)  | [Othertelephones](othertelephones.md)  | [OtherPhones2](otherphones2.md)  | [ポケットベル](pagers.md)  | [RadioPhones](radiophones.md)  | [Telexnumbers](telexnumbers.md)  | [TTYTDDPhoneNumbers](ttytddphonenumbers.md)  | [ファックス](workfaxes.md)  | [Emails1](emails1.md)  | [Emails2](emails2.md)  | [Emails3](emails3.md)  | [BusinessHomePages](businesshomepages.md)  | [PersonalHomePages](personalhomepages.md)  | [Officelocations 場所](officelocations.md)  | [Imaddresses (ArrayOfStringAttributedValuesType)](imaddresses-arrayofstringattributedvaluestype.md)  | [ImAddresses2](imaddresses2.md)  | [ImAddresses3](imaddresses3.md)  | [Businessaddresses](businessaddresses.md)  | [ホームアドレス](homeaddresses.md)  | [Otheraddresses](otheraddresses.md)  | [タイトル](titles.md)  | [部門](departments.md)  | 会社[名](companynames.md)  | [マネージャー](managers.md)  | [AssistantNames](assistantnames.md)  | [Professions](professions.md)  | [Spousenames](spousenames.md)  |  場合[子 (ArrayOfStringArrayAttributedValuesType)](children-arrayofstringarrayattributedvaluestype.md)  | [教育機関](schools.md)  | [趣味](hobbies.md)  | [Weddinganniversaries 日](weddinganniversaries.md)  | [誕生日](birthdays.md)  | [場所](locations.md)  | [Extendedproperties (ArrayOfExtendedPropertyAttributedValueType)](extendedproperties-arrayofextendedpropertyattributedvaluetype.md)
  
### <a name="parent-elements"></a>親要素

[AddNewImContactToGroupResponse](addnewimcontacttogroupresponse.md)  | [AddNewTelUriContactToGroupResponse](addnewteluricontacttogroupresponse.md)  | [GetPersonaResponseMessage](getpersonaresponsemessage.md)  | [ユーザー](people.md)  | [ペルソナ](personas-ex15websvcsotherref.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

