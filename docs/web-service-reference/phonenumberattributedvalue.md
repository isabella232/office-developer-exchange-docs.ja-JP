---
title: PhoneNumberAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8bf16552-b672-424a-91b6-6470e20a49ad
description: PhoneNumberAttributedValue 要素は、関連付けられている帰属と電話番号の配列のインスタンスを指定します。
ms.openlocfilehash: a2cc2685e804b3bf6dd5f9083b31a4bd137f8aac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832771"
---
# <a name="phonenumberattributedvalue"></a><span data-ttu-id="9564f-103">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="9564f-103">PhoneNumberAttributedValue</span></span>

<span data-ttu-id="9564f-104">**PhoneNumberAttributedValue**要素は、関連付けられている帰属と電話番号の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="9564f-104">The **PhoneNumberAttributedValue** element specifies an instance of an array of phone numbers and their associated attributions.</span></span> 
  
```XML
<PhoneNumberAttributedValue>
   <Value/>
   <Attributions/>
</PhoneNumberAttributedValue>
```

 <span data-ttu-id="9564f-105">**PhoneNumberAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="9564f-105">**PhoneNumberAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9564f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9564f-106">Attributes and elements</span></span>

<span data-ttu-id="9564f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9564f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9564f-108">属性</span><span class="sxs-lookup"><span data-stu-id="9564f-108">Attributes</span></span>

<span data-ttu-id="9564f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9564f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9564f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9564f-110">Child elements</span></span>

<span data-ttu-id="9564f-111">[値 (PersonaPhoneNumberType)](value-personaphonenumbertype.md) | [(ArrayOfValueAttributionsType) の帰属](attributions-arrayofvalueattributionstype.md)</span><span class="sxs-lookup"><span data-stu-id="9564f-111">[Value (PersonaPhoneNumberType)](value-personaphonenumbertype.md) | [Attributions (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9564f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9564f-112">Parent elements</span></span>

<span data-ttu-id="9564f-113">[BusinessPhoneNumbers](businessphonenumbers.md) | [BusinessPhoneNumbers2](businessphonenumbers2.md) | [HomePhones](homephones.md) | [HomePhones2](homephones2.md) | [MobilePhones](mobilephones.md) | [MobilePhones2](mobilephones2.md) | [AssistantPhoneNumbers](assistantphonenumbers.md)  |  [CallbackPhones](callbackphones.md) | [CarPhones](carphones.md) | [HomeFaxes](homefaxes.md) | [OrganizationMainPhones](organizationmainphones.md) | [OtherFaxes](otherfaxes.md) | [OtherTelephones](othertelephones.md)  |  [OtherPhones2](otherphones2.md) | [ポケットベル](pagers.md) | [RadioPhones](radiophones.md) | [TelexNumbers](telexnumbers.md) | [TTYTDDPhoneNumbers](ttytddphonenumbers.md) | [WorkFaxes](workfaxes.md)</span><span class="sxs-lookup"><span data-stu-id="9564f-113">[BusinessPhoneNumbers](businessphonenumbers.md) | [BusinessPhoneNumbers2](businessphonenumbers2.md) | [HomePhones](homephones.md) | [HomePhones2](homephones2.md) | [MobilePhones](mobilephones.md) | [MobilePhones2](mobilephones2.md) | [AssistantPhoneNumbers](assistantphonenumbers.md) | [CallbackPhones](callbackphones.md) | [CarPhones](carphones.md) | [HomeFaxes](homefaxes.md) | [OrganizationMainPhones](organizationmainphones.md) | [OtherFaxes](otherfaxes.md) | [OtherTelephones](othertelephones.md) | [OtherPhones2](otherphones2.md) | [Pagers](pagers.md) | [RadioPhones](radiophones.md) | [TelexNumbers](telexnumbers.md) | [TTYTDDPhoneNumbers](ttytddphonenumbers.md) | [WorkFaxes](workfaxes.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9564f-114">備考</span><span class="sxs-lookup"><span data-stu-id="9564f-114">Remarks</span></span>

<span data-ttu-id="9564f-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9564f-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9564f-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9564f-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9564f-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="9564f-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9564f-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="9564f-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9564f-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9564f-119">Schema name</span></span>  <br/> |<span data-ttu-id="9564f-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9564f-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="9564f-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9564f-121">Validation file</span></span>  <br/> |<span data-ttu-id="9564f-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9564f-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9564f-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9564f-123">Can be empty</span></span>  <br/> ||
   

