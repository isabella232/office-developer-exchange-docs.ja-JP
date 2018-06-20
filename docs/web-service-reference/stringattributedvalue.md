---
title: StringAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 911fec52-bde7-44a3-9231-04f327a42107
description: StringAttributedValue 要素は、ペルソナの要素に関連付けられている属性の配列のインスタンスを指定します。
ms.openlocfilehash: 54d4dbcec49ca80b4f4d79fb450773c19aef05d4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839616"
---
# <a name="stringattributedvalue"></a><span data-ttu-id="819dd-103">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="819dd-103">StringAttributedValue</span></span>

<span data-ttu-id="819dd-104">**StringAttributedValue**要素は、ペルソナの要素に関連付けられている属性の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="819dd-104">The **StringAttributedValue** element specifies an instance in an array of attributes associated with a persona element.</span></span> 
  
```XML
<StringAttributedValue>
   <Value/>
   <Attributions/>
</StringAttributedValue>
```

 <span data-ttu-id="819dd-105">**StringAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="819dd-105">**StringAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="819dd-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="819dd-106">Attributes and elements</span></span>

<span data-ttu-id="819dd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="819dd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="819dd-108">属性</span><span class="sxs-lookup"><span data-stu-id="819dd-108">Attributes</span></span>

<span data-ttu-id="819dd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="819dd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="819dd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="819dd-110">Child elements</span></span>

<span data-ttu-id="819dd-111">[値](value.md) | [(ArrayOfValueAttributionsType) の帰属](attributions-arrayofvalueattributionstype.md)</span><span class="sxs-lookup"><span data-stu-id="819dd-111">[Value](value.md) | [Attributions (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="819dd-112">親要素</span><span class="sxs-lookup"><span data-stu-id="819dd-112">Parent elements</span></span>

<span data-ttu-id="819dd-113">[表示名](displaynames.md) | [FileAses](fileases.md) | [FileAsIds](fileasids.md) | [DisplayNamePrefixes](displaynameprefixes.md) | [GivenNames](givennames.md) | [MiddleNames](middlenames.md) | [姓](surnames.md) | [代](generations.md)  | [ニックネーム](nicknames.md) | [頭文字](initials.md) | [YomiCompanyNames](yomicompanynames.md) | [YomiFirstNames](yomifirstnames.md) | [YomiLastNames](yomilastnames.md) | [BusinessHomePages](businesshomepages.md)  |  [PersonalHomePages](personalhomepages.md) | [OfficeLocations](officelocations.md) | [ImAddresses](imaddresses.md) | [ImAddresses2](imaddresses2.md) | [ImAddresses3](imaddresses3.md) | [タイトル](titles.md) |  [部門](departments.md) | [CompanyNames](companynames.md) | [マネージャー](managers.md) | [AssistantNames](assistantnames.md) | [職業](professions.md) | [SpouseNames](spousenames.md) | [学校](schools.md) | [趣味](hobbies.md) |  [WeddingAnniversaries](weddinganniversaries.md) | [誕生日](birthdays.md) | [の場所](locations.md)</span><span class="sxs-lookup"><span data-stu-id="819dd-113">[DisplayNames](displaynames.md) | [FileAses](fileases.md) | [FileAsIds](fileasids.md) | [DisplayNamePrefixes](displaynameprefixes.md) | [GivenNames](givennames.md) | [MiddleNames](middlenames.md) | [Surnames](surnames.md) | [Generations](generations.md) | [Nicknames](nicknames.md) | [Initials](initials.md) | [YomiCompanyNames](yomicompanynames.md) | [YomiFirstNames](yomifirstnames.md) | [YomiLastNames](yomilastnames.md) | [BusinessHomePages](businesshomepages.md) | [PersonalHomePages](personalhomepages.md) | [OfficeLocations](officelocations.md) | [ImAddresses](imaddresses.md) | [ImAddresses2](imaddresses2.md) | [ImAddresses3](imaddresses3.md) | [Titles](titles.md) | [Departments](departments.md) | [CompanyNames](companynames.md) | [Managers](managers.md) | [AssistantNames](assistantnames.md) | [Professions](professions.md) | [SpouseNames](spousenames.md) | [Schools](schools.md) | [Hobbies](hobbies.md) | [WeddingAnniversaries](weddinganniversaries.md) | [Birthdays](birthdays.md) | [Locations](locations.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="819dd-114">備考</span><span class="sxs-lookup"><span data-stu-id="819dd-114">Remarks</span></span>

<span data-ttu-id="819dd-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="819dd-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="819dd-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="819dd-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="819dd-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="819dd-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="819dd-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="819dd-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="819dd-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="819dd-119">Schema name</span></span>  <br/> |<span data-ttu-id="819dd-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="819dd-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="819dd-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="819dd-121">Validation file</span></span>  <br/> |<span data-ttu-id="819dd-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="819dd-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="819dd-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="819dd-123">Can be empty</span></span>  <br/> ||
   

