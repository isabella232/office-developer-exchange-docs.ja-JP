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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465626"
---
# <a name="phonenumberattributedvalue"></a><span data-ttu-id="115ae-103">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="115ae-103">PhoneNumberAttributedValue</span></span>

<span data-ttu-id="115ae-104">**PhoneNumberAttributedValue**要素は、電話番号の配列のインスタンスと、それに関連付けられている attributions を指定します。</span><span class="sxs-lookup"><span data-stu-id="115ae-104">The **PhoneNumberAttributedValue** element specifies an instance of an array of phone numbers and their associated attributions.</span></span> 
  
```XML
<PhoneNumberAttributedValue>
   <Value/>
   <Attributions/>
</PhoneNumberAttributedValue>
```

 <span data-ttu-id="115ae-105">**PhoneNumberAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="115ae-105">**PhoneNumberAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="115ae-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="115ae-106">Attributes and elements</span></span>

<span data-ttu-id="115ae-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="115ae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="115ae-108">属性</span><span class="sxs-lookup"><span data-stu-id="115ae-108">Attributes</span></span>

<span data-ttu-id="115ae-109">なし。</span><span class="sxs-lookup"><span data-stu-id="115ae-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="115ae-110">子要素</span><span class="sxs-lookup"><span data-stu-id="115ae-110">Child elements</span></span>

<span data-ttu-id="115ae-111">[Value (PersonaPhoneNumberType)](value-personaphonenumbertype.md)  | [Attributions (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md)</span><span class="sxs-lookup"><span data-stu-id="115ae-111">[Value (PersonaPhoneNumberType)](value-personaphonenumbertype.md) | [Attributions (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="115ae-112">親要素</span><span class="sxs-lookup"><span data-stu-id="115ae-112">Parent elements</span></span>

<span data-ttu-id="115ae-113">[BusinessPhoneNumbers](businessphonenumbers.md)  | [BusinessPhoneNumbers2](businessphonenumbers2.md)  | [ホーム電話](homephones.md)  | [HomePhones2](homephones2.md)  | [MobilePhones](mobilephones.md)  | [MobilePhones2](mobilephones2.md)  | [AssistantPhoneNumbers](assistantphonenumbers.md)  | [電話機](callbackphones.md)  | [カーフォン](carphones.md)  | [ホーム fax](homefaxes.md)  | [組織のメイン電話](organizationmainphones.md)  | その[他の fax](otherfaxes.md)  | [Othertelephones](othertelephones.md)  | [OtherPhones2](otherphones2.md)  | [ポケットベル](pagers.md)  | [RadioPhones](radiophones.md)  | [Telexnumbers](telexnumbers.md)  | [TTYTDDPhoneNumbers](ttytddphonenumbers.md)  | [ファックス](workfaxes.md)</span><span class="sxs-lookup"><span data-stu-id="115ae-113">[BusinessPhoneNumbers](businessphonenumbers.md) | [BusinessPhoneNumbers2](businessphonenumbers2.md) | [HomePhones](homephones.md) | [HomePhones2](homephones2.md) | [MobilePhones](mobilephones.md) | [MobilePhones2](mobilephones2.md) | [AssistantPhoneNumbers](assistantphonenumbers.md) | [CallbackPhones](callbackphones.md) | [CarPhones](carphones.md) | [HomeFaxes](homefaxes.md) | [OrganizationMainPhones](organizationmainphones.md) | [OtherFaxes](otherfaxes.md) | [OtherTelephones](othertelephones.md) | [OtherPhones2](otherphones2.md) | [Pagers](pagers.md) | [RadioPhones](radiophones.md) | [TelexNumbers](telexnumbers.md) | [TTYTDDPhoneNumbers](ttytddphonenumbers.md) | [WorkFaxes](workfaxes.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="115ae-114">注釈</span><span class="sxs-lookup"><span data-stu-id="115ae-114">Remarks</span></span>

<span data-ttu-id="115ae-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="115ae-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="115ae-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="115ae-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="115ae-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="115ae-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="115ae-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="115ae-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="115ae-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="115ae-119">Schema name</span></span>  <br/> |<span data-ttu-id="115ae-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="115ae-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="115ae-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="115ae-121">Validation file</span></span>  <br/> |<span data-ttu-id="115ae-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="115ae-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="115ae-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="115ae-123">Can be empty</span></span>  <br/> ||
   

