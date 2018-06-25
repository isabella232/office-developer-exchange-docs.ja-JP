---
title: RetentionPolicyTags
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8ed4a48a-d510-4cbe-a172-145c33ffb297
description: RetentionPolicyTags 要素には、GetUserRetentionPolicyTags の WSDL 操作の応答で返される保持タグの一覧が含まれています。
ms.openlocfilehash: 60fbb3ad34c9ba34e96c91da99d44a17843c0138
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833230"
---
# <a name="retentionpolicytags"></a><span data-ttu-id="71878-103">RetentionPolicyTags</span><span class="sxs-lookup"><span data-stu-id="71878-103">RetentionPolicyTags</span></span>

<span data-ttu-id="71878-104">**RetentionPolicyTags**要素には、 **GetUserRetentionPolicyTags**の WSDL 操作の応答で返される保持タグの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="71878-104">The **RetentionPolicyTags** element contains a list of retention tags returned in the response of the **GetUserRetentionPolicyTags** WSDL operation.</span></span> 
  
```XML
<RetentionPolicyTags>
   <RetentionPolicyTag/>
</RetentionPolicyTags>
```

 <span data-ttu-id="71878-105">**ArrayOfRetentionPolicyTagsType**</span><span class="sxs-lookup"><span data-stu-id="71878-105">**ArrayOfRetentionPolicyTagsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="71878-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="71878-106">Attributes and elements</span></span>

<span data-ttu-id="71878-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="71878-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71878-108">属性</span><span class="sxs-lookup"><span data-stu-id="71878-108">Attributes</span></span>

<span data-ttu-id="71878-109">なし。</span><span class="sxs-lookup"><span data-stu-id="71878-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="71878-110">子要素</span><span class="sxs-lookup"><span data-stu-id="71878-110">Child elements</span></span>

[<span data-ttu-id="71878-111">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="71878-111">RetentionPolicyTag</span></span>](retentionpolicytag.md)
  
### <a name="parent-elements"></a><span data-ttu-id="71878-112">親要素</span><span class="sxs-lookup"><span data-stu-id="71878-112">Parent elements</span></span>

[<span data-ttu-id="71878-113">GetUserRetentionPolicyTagsResponse</span><span class="sxs-lookup"><span data-stu-id="71878-113">GetUserRetentionPolicyTagsResponse</span></span>](getuserretentionpolicytagsresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="71878-114">備考</span><span class="sxs-lookup"><span data-stu-id="71878-114">Remarks</span></span>

<span data-ttu-id="71878-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="71878-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="71878-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="71878-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="71878-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="71878-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71878-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="71878-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="71878-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="71878-119">Schema name</span></span>  <br/> |<span data-ttu-id="71878-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="71878-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="71878-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="71878-121">Validation file</span></span>  <br/> |<span data-ttu-id="71878-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="71878-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="71878-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="71878-123">Can be empty</span></span>  <br/> |<span data-ttu-id="71878-124">false</span><span class="sxs-lookup"><span data-stu-id="71878-124">false</span></span>  <br/> |
   

