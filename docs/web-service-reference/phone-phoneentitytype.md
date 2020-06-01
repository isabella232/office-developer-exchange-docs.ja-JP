---
title: Phone (通し Entitytype)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f6925cc9-7f22-478f-b9ba-b77575772471
description: Phone 要素は、電話番号エンティティの抽出によって得られる1つの電話番号を指定します。
ms.openlocfilehash: eec05fbb1cbbfa5c9b47cdb3cef1af6085ab51b6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457558"
---
# <a name="phone-phoneentitytype"></a><span data-ttu-id="3adaa-103">Phone (通し Entitytype)</span><span class="sxs-lookup"><span data-stu-id="3adaa-103">Phone (PhoneEntityType)</span></span>

<span data-ttu-id="3adaa-104">**Phone**要素は、電話番号エンティティの抽出によって得られる1つの電話番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="3adaa-104">The **Phone** element specifies a single phone number that results from a phone number entity extraction.</span></span> 
  
```XML
<Phone>
   <Position/>
   <OriginalPhoneString/>
   <PhoneString/>
   <Type/>
</Phone>
```

 <span data-ttu-id="3adaa-105">**電話の Entitytype**</span><span class="sxs-lookup"><span data-stu-id="3adaa-105">**PhoneEntityType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3adaa-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3adaa-106">Attributes and elements</span></span>

<span data-ttu-id="3adaa-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3adaa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3adaa-108">属性</span><span class="sxs-lookup"><span data-stu-id="3adaa-108">Attributes</span></span>

<span data-ttu-id="3adaa-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3adaa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3adaa-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3adaa-110">Child elements</span></span>

<span data-ttu-id="3adaa-111">[Position](position.md)  | [Phonenumber.originalphonestring](originalphonestring.md)  | [電話テキスト](phonestring.md)  | [型 (string)](type-string.md)</span><span class="sxs-lookup"><span data-stu-id="3adaa-111">[Position](position.md) | [OriginalPhoneString](originalphonestring.md) | [PhoneString](phonestring.md) | [Type (string)](type-string.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3adaa-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3adaa-112">Parent elements</span></span>

[<span data-ttu-id="3adaa-113">PhoneNumbers (ArrayOfPhoneEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="3adaa-113">PhoneNumbers (ArrayOfPhoneEntitiesType)</span></span>](phonenumbers-arrayofphoneentitiestype.md)
  
## <a name="remarks"></a><span data-ttu-id="3adaa-114">注釈</span><span class="sxs-lookup"><span data-stu-id="3adaa-114">Remarks</span></span>

<span data-ttu-id="3adaa-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3adaa-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3adaa-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3adaa-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3adaa-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3adaa-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3adaa-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="3adaa-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3adaa-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3adaa-119">Schema name</span></span>  <br/> |<span data-ttu-id="3adaa-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="3adaa-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="3adaa-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3adaa-121">Validation file</span></span>  <br/> |<span data-ttu-id="3adaa-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="3adaa-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3adaa-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3adaa-123">Can be empty</span></span>  <br/> ||
   

