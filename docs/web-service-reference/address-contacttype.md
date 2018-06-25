---
title: アドレス (ContactType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c39f37bf-5cf5-47a7-8a2a-337b5e68f94f
description: アドレス要素は、連絡先のアドレスを指定します。
ms.openlocfilehash: 75fee4bd793497b1758bb848c7aa7dcc4d1a4e8e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759297"
---
# <a name="address-contacttype"></a><span data-ttu-id="646b8-103">アドレス (ContactType)</span><span class="sxs-lookup"><span data-stu-id="646b8-103">Address (ContactType)</span></span>

<span data-ttu-id="646b8-104">**アドレス**要素は、連絡先のアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="646b8-104">The **Address** element specifies the address of a contact.</span></span> 
  
```XML
<Address></Address>
```

 <span data-ttu-id="646b8-105">**使用されています**</span><span class="sxs-lookup"><span data-stu-id="646b8-105">**xs:string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="646b8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="646b8-106">Attributes and elements</span></span>

<span data-ttu-id="646b8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="646b8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="646b8-108">属性</span><span class="sxs-lookup"><span data-stu-id="646b8-108">Attributes</span></span>

<span data-ttu-id="646b8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="646b8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="646b8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="646b8-110">Child elements</span></span>

<span data-ttu-id="646b8-111">なし。</span><span class="sxs-lookup"><span data-stu-id="646b8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="646b8-112">親要素</span><span class="sxs-lookup"><span data-stu-id="646b8-112">Parent elements</span></span>

|<span data-ttu-id="646b8-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="646b8-113">**Element**</span></span>|<span data-ttu-id="646b8-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="646b8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="646b8-115">アドレス (ArrayOfAddressesType)</span><span class="sxs-lookup"><span data-stu-id="646b8-115">Addresses (ArrayOfAddressesType)</span></span>](addresses-arrayofaddressestype.md) <br/> |<span data-ttu-id="646b8-116">**アドレス**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="646b8-116">Specifies an array of **Address** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="646b8-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="646b8-117">Text value</span></span>

<span data-ttu-id="646b8-118">**アドレス**要素のテキスト値は、連絡先の郵送先住所です。</span><span class="sxs-lookup"><span data-stu-id="646b8-118">The text value of the **Address** element is the contact's postal address.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="646b8-119">備考</span><span class="sxs-lookup"><span data-stu-id="646b8-119">Remarks</span></span>

<span data-ttu-id="646b8-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="646b8-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="646b8-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="646b8-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="646b8-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="646b8-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="646b8-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="646b8-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="646b8-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="646b8-124">Schema Name</span></span>  <br/> |<span data-ttu-id="646b8-125">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="646b8-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="646b8-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="646b8-126">Validation File</span></span>  <br/> |<span data-ttu-id="646b8-127">types.xsd</span><span class="sxs-lookup"><span data-stu-id="646b8-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="646b8-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="646b8-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="646b8-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="646b8-129">See also</span></span>

- [<span data-ttu-id="646b8-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="646b8-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

