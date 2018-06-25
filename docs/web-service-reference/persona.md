---
title: ペルソナ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b115c990-3a2d-4536-9af3-ac1fd06d00dc
description: ペルソナの要素は、GetPersona の要求によって返されるペルソナ データのセットを指定します。
ms.openlocfilehash: 15af72eb0e25e424aa7293ce0cbc2dd31e76abda
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832736"
---
# <a name="persona"></a><span data-ttu-id="742aa-103">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="742aa-103">Persona</span></span>

<span data-ttu-id="742aa-104">**ペルソナ**の要素は、 **GetPersona**の要求によって返されるペルソナ データのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="742aa-104">The **Persona** element specifies a set of persona data returned by a **GetPersona** request.</span></span> 
  
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

 <span data-ttu-id="742aa-105">**PersonaType**</span><span class="sxs-lookup"><span data-stu-id="742aa-105">**PersonaType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="742aa-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="742aa-106">Attributes and elements</span></span>

<span data-ttu-id="742aa-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="742aa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="742aa-108">属性</span><span class="sxs-lookup"><span data-stu-id="742aa-108">Attributes</span></span>

<span data-ttu-id="742aa-109">なし。</span><span class="sxs-lookup"><span data-stu-id="742aa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="742aa-110">子要素</span><span class="sxs-lookup"><span data-stu-id="742aa-110">Child elements</span></span>

<span data-ttu-id="742aa-111">[PersonaId](personaid.md) | [PersonaType](personatype.md) | [PersonaObjectStatus](personaobjectstatus.md) | [CreationTime](creationtime.md) | [本文](bodies.md) | [DisplayNameFirstLastSortKey](displaynamefirstlastsortkey.md) | [DisplayNameLastFirstSortKey](displaynamelastfirstsortkey.md)  |  [CompanyNameSortKey](companynamesortkey.md) | [HomeCitySortKey](homecitysortkey.md) | [WorkCitySortKey](workcitysortkey.md) | [DisplayNameFirstLastHeader](displaynamefirstlastheader.md) | [DisplayNameLastFirstHeader](displaynamelastfirstheader.md)  |  [FileAsHeader](fileasheader.md) | [表示名 (文字列)](displayname-string.md) | [DisplayNameFirstLast](displaynamefirstlast.md) | [DisplayNameLastFirst](displaynamelastfirst.md) | [表題](fileas.md) | [FileAsId](fileasid.md)  | [DisplayNamePrefix](displaynameprefix.md) | [名](givenname.md) | [ミドル](middlename.md) | [姓](surname.md) | [生成](generation.md) | [ニックネーム](nickname.md) | [YomiCompanyName](yomicompanyname.md) | [YomiFirstName](yomifirstname.md)  |  [YomiLastName](yomilastname.md) | [タイトル](title.md) | [部門](department.md) | [[得意先名]](companyname.md) | [の場所](location.md) | [EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md)  | [EmailAddresses (ArrayOfEmailAddressesType)](emailaddresses-arrayofemailaddressestype.md) | [電話番号](phonenumber.md) | [ImAddress (文字列)](imaddress-string.md) | [HomeCity](homecity.md) | [WorkCity](workcity.md) | [RelevanceScore](relevancescore.md) | [FolderIds (ArrayOfFolderIdType)](folderids-arrayoffolderidtype.md)  | [帰属 (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md) | [の表示名](displaynames.md) | [FileAses](fileases.md) | [FileAsIds](fileasids.md) | [DisplayNamePrefixes](displaynameprefixes.md) | [GivenNames](givennames.md)  |  [MiddleNames](middlenames.md) | [姓](surnames.md) | [代](generations.md) | [ニックネーム](nicknames.md) | [頭文字 (ArrayOfStringAttributedValuesType)](initials-arrayofstringattributedvaluestype.md)  |  [YomiCompanyNames](yomicompanynames.md) | [YomiFirstNames](yomifirstnames.md) | [YomiLastNames](yomilastnames.md) | [BusinessPhoneNumbers](businessphonenumbers.md) | [BusinessPhoneNumbers2](businessphonenumbers2.md) | [HomePhones](homephones.md)  |  [HomePhones2](homephones2.md) | [MobilePhones](mobilephones.md) | [MobilePhones2](mobilephones2.md) | [AssistantPhoneNumbers](assistantphonenumbers.md) | [CallbackPhones](callbackphones.md)  | [CarPhones](carphones.md) |  [HomeFaxes](homefaxes.md) | [OrganizationMainPhones](organizationmainphones.md) | [OtherFaxes](otherfaxes.md) | [OtherTelephones](othertelephones.md) | [OtherPhones2](otherphones2.md) | [ポケットベル](pagers.md)  |  [RadioPhones](radiophones.md) | [TelexNumbers](telexnumbers.md) | [TTYTDDPhoneNumbers](ttytddphonenumbers.md) | [WorkFaxes](workfaxes.md) | [Emails1](emails1.md) | [Emails2](emails2.md)  |  [Emails3](emails3.md) | [BusinessHomePages](businesshomepages.md) | [PersonalHomePages](personalhomepages.md) | [OfficeLocations](officelocations.md) | [ImAddresses (ArrayOfStringAttributedValuesType)](imaddresses-arrayofstringattributedvaluestype.md) | [ImAddresses2](imaddresses2.md) | [ImAddresses3](imaddresses3.md) | [BusinessAddresses](businessaddresses.md) | [HomeAddresses](homeaddresses.md)  |  [OtherAddresses](otheraddresses.md) | [タイトル](titles.md) | [部門](departments.md) | [CompanyNames](companynames.md) | [マネージャー](managers.md) | [AssistantNames](assistantnames.md)  |  [職業](professions.md) | [SpouseNames](spousenames.md) | [(ArrayOfStringArrayAttributedValuesType) の子](children-arrayofstringarrayattributedvaluestype.md) | [学校](schools.md) | [趣味](hobbies.md) |  [WeddingAnniversaries](weddinganniversaries.md) | [誕生日](birthdays.md) | [の場所](locations.md) | [ExtendedProperties (ArrayOfExtendedPropertyAttributedValueType)](extendedproperties-arrayofextendedpropertyattributedvaluetype.md)</span><span class="sxs-lookup"><span data-stu-id="742aa-111">[PersonaId](personaid.md) | [PersonaType](personatype.md) | [PersonaObjectStatus](personaobjectstatus.md) | [CreationTime](creationtime.md) | [Bodies](bodies.md) | [DisplayNameFirstLastSortKey](displaynamefirstlastsortkey.md) | [DisplayNameLastFirstSortKey](displaynamelastfirstsortkey.md) | [CompanyNameSortKey](companynamesortkey.md) | [HomeCitySortKey](homecitysortkey.md) | [WorkCitySortKey](workcitysortkey.md) | [DisplayNameFirstLastHeader](displaynamefirstlastheader.md) | [DisplayNameLastFirstHeader](displaynamelastfirstheader.md) | [FileAsHeader](fileasheader.md) | [DisplayName (string)](displayname-string.md) | [DisplayNameFirstLast](displaynamefirstlast.md) | [DisplayNameLastFirst](displaynamelastfirst.md) | [FileAs](fileas.md) | [FileAsId](fileasid.md) | [DisplayNamePrefix](displaynameprefix.md) | [GivenName](givenname.md) | [MiddleName](middlename.md) | [Surname](surname.md) | [Generation](generation.md) | [Nickname](nickname.md) | [YomiCompanyName](yomicompanyname.md) | [YomiFirstName](yomifirstname.md) | [YomiLastName](yomilastname.md) | [Title](title.md) | [Department](department.md) | [CompanyName](companyname.md) | [Location](location.md) | [EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md) | [EmailAddresses (ArrayOfEmailAddressesType)](emailaddresses-arrayofemailaddressestype.md) | [PhoneNumber](phonenumber.md) | [ImAddress (String)](imaddress-string.md) | [HomeCity](homecity.md) | [WorkCity](workcity.md) | [RelevanceScore](relevancescore.md) | [FolderIds (ArrayOfFolderIdType)](folderids-arrayoffolderidtype.md) | [Attributions (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md) | [DisplayNames](displaynames.md) | [FileAses](fileases.md) | [FileAsIds](fileasids.md) | [DisplayNamePrefixes](displaynameprefixes.md) | [GivenNames](givennames.md) | [MiddleNames](middlenames.md) | [Surnames](surnames.md) | [Generations](generations.md) | [Nicknames](nicknames.md) | [Initials (ArrayOfStringAttributedValuesType)](initials-arrayofstringattributedvaluestype.md) | [YomiCompanyNames](yomicompanynames.md) | [YomiFirstNames](yomifirstnames.md) | [YomiLastNames](yomilastnames.md) | [BusinessPhoneNumbers](businessphonenumbers.md) | [BusinessPhoneNumbers2](businessphonenumbers2.md) | [HomePhones](homephones.md) | [HomePhones2](homephones2.md) | [MobilePhones](mobilephones.md) | [MobilePhones2](mobilephones2.md) | [AssistantPhoneNumbers](assistantphonenumbers.md) | [CallbackPhones](callbackphones.md) | [CarPhones](carphones.md) | [HomeFaxes](homefaxes.md) | [OrganizationMainPhones](organizationmainphones.md) | [OtherFaxes](otherfaxes.md) | [OtherTelephones](othertelephones.md) | [OtherPhones2](otherphones2.md) | [Pagers](pagers.md) | [RadioPhones](radiophones.md) | [TelexNumbers](telexnumbers.md) | [TTYTDDPhoneNumbers](ttytddphonenumbers.md) | [WorkFaxes](workfaxes.md) | [Emails1](emails1.md) | [Emails2](emails2.md) | [Emails3](emails3.md) | [BusinessHomePages](businesshomepages.md) | [PersonalHomePages](personalhomepages.md) | [OfficeLocations](officelocations.md) | [ImAddresses (ArrayOfStringAttributedValuesType)](imaddresses-arrayofstringattributedvaluestype.md) | [ImAddresses2](imaddresses2.md) | [ImAddresses3](imaddresses3.md) | [BusinessAddresses](businessaddresses.md) | [HomeAddresses](homeaddresses.md) | [OtherAddresses](otheraddresses.md) | [Titles](titles.md) | [Departments](departments.md) | [CompanyNames](companynames.md) | [Managers](managers.md) | [AssistantNames](assistantnames.md) | [Professions](professions.md) | [SpouseNames](spousenames.md) | [Children (ArrayOfStringArrayAttributedValuesType)](children-arrayofstringarrayattributedvaluestype.md) | [Schools](schools.md) | [Hobbies](hobbies.md) | [WeddingAnniversaries](weddinganniversaries.md) | [Birthdays](birthdays.md) | [Locations](locations.md) | [ExtendedProperties (ArrayOfExtendedPropertyAttributedValueType)](extendedproperties-arrayofextendedpropertyattributedvaluetype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="742aa-112">親要素</span><span class="sxs-lookup"><span data-stu-id="742aa-112">Parent elements</span></span>

<span data-ttu-id="742aa-113">[AddNewImContactToGroupResponse](addnewimcontacttogroupresponse.md) | [AddNewTelUriContactToGroupResponse](addnewteluricontacttogroupresponse.md) | [GetPersonaResponseMessage](getpersonaresponsemessage.md) | [人](people.md) | [ペルソナ](personas-ex15websvcsotherref.md)</span><span class="sxs-lookup"><span data-stu-id="742aa-113">[AddNewImContactToGroupResponse](addnewimcontacttogroupresponse.md) | [AddNewTelUriContactToGroupResponse](addnewteluricontacttogroupresponse.md) | [GetPersonaResponseMessage](getpersonaresponsemessage.md) | [People](people.md) | [Personas](personas-ex15websvcsotherref.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="742aa-114">備考</span><span class="sxs-lookup"><span data-stu-id="742aa-114">Remarks</span></span>

<span data-ttu-id="742aa-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="742aa-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="742aa-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="742aa-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="742aa-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="742aa-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="742aa-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="742aa-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="742aa-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="742aa-119">Schema name</span></span>  <br/> |<span data-ttu-id="742aa-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="742aa-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="742aa-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="742aa-121">Validation file</span></span>  <br/> |<span data-ttu-id="742aa-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="742aa-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="742aa-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="742aa-123">Can be empty</span></span>  <br/> |<span data-ttu-id="742aa-124">false</span><span class="sxs-lookup"><span data-stu-id="742aa-124">false</span></span>  <br/> |
   

