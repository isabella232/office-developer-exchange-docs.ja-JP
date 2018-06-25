---
title: AddDistributionGroupToImListResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 70fe6730-1c9a-4550-acc4-7737ff407871
description: AddDistributionGroupToImListResponse 要素は、AddDistributionGroupToImList 要求への応答を定義します。
ms.openlocfilehash: b037ea4d2d3b3f28b466345d82d836b936cdbf2b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759282"
---
# <a name="adddistributiongrouptoimlistresponse"></a><span data-ttu-id="ff09d-103">AddDistributionGroupToImListResponse</span><span class="sxs-lookup"><span data-stu-id="ff09d-103">AddDistributionGroupToImListResponse</span></span>

<span data-ttu-id="ff09d-104">**AddDistributionGroupToImListResponse**要素は、 **AddDistributionGroupToImList**要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="ff09d-104">The **AddDistributionGroupToImListResponse** element defines a response to a **AddDistributionGroupToImList** request.</span></span> 
  
```XML
<AddNewImContactToGroupResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ImGroup/>
</AddNewImContactToGroupResponse>
```

 <span data-ttu-id="ff09d-105">**AddDistributionGroupToImListResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="ff09d-105">**AddDistributionGroupToImListResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ff09d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ff09d-106">Attributes and elements</span></span>

<span data-ttu-id="ff09d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ff09d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff09d-108">属性</span><span class="sxs-lookup"><span data-stu-id="ff09d-108">Attributes</span></span>

<span data-ttu-id="ff09d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ff09d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ff09d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ff09d-110">Child elements</span></span>

<span data-ttu-id="ff09d-111">[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [ImGroup](imgroup.md)</span><span class="sxs-lookup"><span data-stu-id="ff09d-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [ImGroup](imgroup.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ff09d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ff09d-112">Parent elements</span></span>

<span data-ttu-id="ff09d-113">なし。</span><span class="sxs-lookup"><span data-stu-id="ff09d-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ff09d-114">備考</span><span class="sxs-lookup"><span data-stu-id="ff09d-114">Remarks</span></span>

<span data-ttu-id="ff09d-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ff09d-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ff09d-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ff09d-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff09d-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="ff09d-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff09d-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="ff09d-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ff09d-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ff09d-119">Schema name</span></span>  <br/> |<span data-ttu-id="ff09d-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="ff09d-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ff09d-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ff09d-121">Validation file</span></span>  <br/> |<span data-ttu-id="ff09d-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ff09d-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ff09d-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ff09d-123">Can be empty</span></span>  <br/> |<span data-ttu-id="ff09d-124">false</span><span class="sxs-lookup"><span data-stu-id="ff09d-124">false</span></span>  <br/> |
   

