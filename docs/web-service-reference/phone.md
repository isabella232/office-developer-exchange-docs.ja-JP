---
title: 電話
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9381d8e0-b705-49fd-a822-00fb485bdbab
description: 電話要素では、取引先担当者エンティティの展開から得られる 1 つの電話番号を指定します。
ms.openlocfilehash: b10a3af65784dafc4445dfcac33fb4b6372c02ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832747"
---
# <a name="phone"></a><span data-ttu-id="67260-103">電話</span><span class="sxs-lookup"><span data-stu-id="67260-103">Phone</span></span>

<span data-ttu-id="67260-104">**電話**要素では、取引先担当者エンティティの展開から得られる 1 つの電話番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="67260-104">The **Phone** element specifies a single phone number that results from a contact entity extraction.</span></span> 
  
```XML
<Phone>
   <OriginalPhoneString/>
   <PhoneString/>
   <Type/>
</Phone>
```

 <span data-ttu-id="67260-105">**PhoneType**</span><span class="sxs-lookup"><span data-stu-id="67260-105">**PhoneType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="67260-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="67260-106">Attributes and elements</span></span>

<span data-ttu-id="67260-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="67260-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="67260-108">属性</span><span class="sxs-lookup"><span data-stu-id="67260-108">Attributes</span></span>

<span data-ttu-id="67260-109">なし。</span><span class="sxs-lookup"><span data-stu-id="67260-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="67260-110">子要素</span><span class="sxs-lookup"><span data-stu-id="67260-110">Child elements</span></span>

<span data-ttu-id="67260-111">[OriginalPhoneString](originalphonestring.md) | [PhoneString](phonestring.md) | [型 (文字列)](type-string.md)</span><span class="sxs-lookup"><span data-stu-id="67260-111">[OriginalPhoneString](originalphonestring.md) | [PhoneString](phonestring.md) | [Type (string)](type-string.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="67260-112">親要素</span><span class="sxs-lookup"><span data-stu-id="67260-112">Parent elements</span></span>

[<span data-ttu-id="67260-113">PhoneNumbers (ArrayOfPhonesType)</span><span class="sxs-lookup"><span data-stu-id="67260-113">PhoneNumbers (ArrayOfPhonesType)</span></span>](phonenumbers-arrayofphonestype.md)
  
## <a name="remarks"></a><span data-ttu-id="67260-114">備考</span><span class="sxs-lookup"><span data-stu-id="67260-114">Remarks</span></span>

<span data-ttu-id="67260-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="67260-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="67260-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="67260-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="67260-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="67260-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="67260-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="67260-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="67260-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="67260-119">Schema name</span></span>  <br/> |<span data-ttu-id="67260-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="67260-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="67260-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="67260-121">Validation file</span></span>  <br/> |<span data-ttu-id="67260-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="67260-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="67260-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="67260-123">Can be empty</span></span>  <br/> ||
   

