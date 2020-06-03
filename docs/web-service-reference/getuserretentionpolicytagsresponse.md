---
title: GetUserRetentionPolicyTagsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 12ba4528-60e9-4c0a-a5b2-eed3a2cb1509
description: GetUserRetentionPolicyTagsResponse 要素には、GetRetentionPolicyTags 要求への応答が含まれます。
ms.openlocfilehash: a8cfdc1aaaf47f3a66e541537381edf92bb024a9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530826"
---
# <a name="getuserretentionpolicytagsresponse"></a><span data-ttu-id="8e8e9-103">GetUserRetentionPolicyTagsResponse</span><span class="sxs-lookup"><span data-stu-id="8e8e9-103">GetUserRetentionPolicyTagsResponse</span></span>

<span data-ttu-id="8e8e9-104">[GetUserRetentionPolicyTagsResponse](getuserretentionpolicytagsresponse.md)要素には、 **GetRetentionPolicyTags**要求への応答が含まれます。</span><span class="sxs-lookup"><span data-stu-id="8e8e9-104">The [GetUserRetentionPolicyTagsResponse](getuserretentionpolicytagsresponse.md) element contains the response to a **GetRetentionPolicyTags** request.</span></span> 
  
```XML
<GetUserRetentionPolicyTagsResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RetentionPolicyTags/>
</GetUserRetentionPolicyTagsResponse>
```

 <span data-ttu-id="8e8e9-105">**GetUserRetentionPolicyTagsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="8e8e9-105">**GetUserRetentionPolicyTagsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8e8e9-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8e8e9-106">Attributes and elements</span></span>

<span data-ttu-id="8e8e9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8e8e9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8e8e9-108">属性</span><span class="sxs-lookup"><span data-stu-id="8e8e9-108">Attributes</span></span>

<span data-ttu-id="8e8e9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8e8e9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8e8e9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8e8e9-110">Child elements</span></span>

<span data-ttu-id="8e8e9-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)  | [RetentionPolicyTags](retentionpolicytags.md)</span><span class="sxs-lookup"><span data-stu-id="8e8e9-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [RetentionPolicyTags](retentionpolicytags.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8e8e9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8e8e9-112">Parent elements</span></span>

<span data-ttu-id="8e8e9-113">なし。</span><span class="sxs-lookup"><span data-stu-id="8e8e9-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8e8e9-114">注釈</span><span class="sxs-lookup"><span data-stu-id="8e8e9-114">Remarks</span></span>

<span data-ttu-id="8e8e9-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8e8e9-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8e8e9-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8e8e9-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8e8e9-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8e8e9-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8e8e9-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="8e8e9-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8e8e9-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8e8e9-119">Schema name</span></span>  <br/> |<span data-ttu-id="8e8e9-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="8e8e9-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8e8e9-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8e8e9-121">Validation file</span></span>  <br/> |<span data-ttu-id="8e8e9-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="8e8e9-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8e8e9-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8e8e9-123">Can be empty</span></span>  <br/> |<span data-ttu-id="8e8e9-124">false</span><span class="sxs-lookup"><span data-stu-id="8e8e9-124">false</span></span>  <br/> |
   

