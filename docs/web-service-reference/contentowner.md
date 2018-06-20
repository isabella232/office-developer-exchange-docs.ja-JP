---
title: ContentOwner
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a1741eda-c232-4d89-8abc-50b2627ad29b
description: ContentOwner 要素は、コンテンツの所有者の名前を指定します。
ms.openlocfilehash: bbc5e69918e31fca639a0fab4987cf7d3541848d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759739"
---
# <a name="contentowner"></a><span data-ttu-id="cab70-103">ContentOwner</span><span class="sxs-lookup"><span data-stu-id="cab70-103">ContentOwner</span></span>

<span data-ttu-id="cab70-104">**ContentOwner**要素は、コンテンツの所有者の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="cab70-104">The **ContentOwner** element specifies the name of the content owner.</span></span> 
  
```XML
<ContentOwner></ContentOwner>
```

 <span data-ttu-id="cab70-105">**string**</span><span class="sxs-lookup"><span data-stu-id="cab70-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cab70-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="cab70-106">Attributes and elements</span></span>

<span data-ttu-id="cab70-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cab70-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cab70-108">属性</span><span class="sxs-lookup"><span data-stu-id="cab70-108">Attributes</span></span>

<span data-ttu-id="cab70-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cab70-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cab70-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cab70-110">Child elements</span></span>

<span data-ttu-id="cab70-111">なし。</span><span class="sxs-lookup"><span data-stu-id="cab70-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cab70-112">親要素</span><span class="sxs-lookup"><span data-stu-id="cab70-112">Parent elements</span></span>

|<span data-ttu-id="cab70-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="cab70-113">**Element**</span></span>|<span data-ttu-id="cab70-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="cab70-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cab70-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="cab70-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="cab70-116">権限管理のライセンスについての情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="cab70-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cab70-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="cab70-117">Text value</span></span>

<span data-ttu-id="cab70-118">ContentOwner 要素のテキスト値は、コンテンツの有効期限の日付を指定する文字列です。</span><span class="sxs-lookup"><span data-stu-id="cab70-118">The text value of the ContentOwner element is a string that specifies the expiration date of the content.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cab70-119">備考</span><span class="sxs-lookup"><span data-stu-id="cab70-119">Remarks</span></span>

<span data-ttu-id="cab70-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="cab70-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cab70-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="cab70-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cab70-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="cab70-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cab70-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="cab70-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cab70-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cab70-124">Schema Name</span></span>  <br/> |<span data-ttu-id="cab70-125">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="cab70-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="cab70-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cab70-126">Validation File</span></span>  <br/> |<span data-ttu-id="cab70-127">types.xsd</span><span class="sxs-lookup"><span data-stu-id="cab70-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="cab70-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="cab70-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="cab70-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="cab70-129">See also</span></span>



- [<span data-ttu-id="cab70-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="cab70-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

