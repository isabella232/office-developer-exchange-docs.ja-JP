---
title: RetentionPolicyTags
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8ed4a48a-d510-4cbe-a172-145c33ffb297
description: RetentionPolicyTags 要素には、GetUserRetentionPolicyTags WSDL 操作の応答で返される保持タグのリストが含まれています。
ms.openlocfilehash: c3a5a165db242092132b4ff0b322dbad2029da36
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462879"
---
# <a name="retentionpolicytags"></a><span data-ttu-id="c4354-103">RetentionPolicyTags</span><span class="sxs-lookup"><span data-stu-id="c4354-103">RetentionPolicyTags</span></span>

<span data-ttu-id="c4354-104">**RetentionPolicyTags**要素には、 **GetUserRetentionPolicyTags** WSDL 操作の応答で返される保持タグのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c4354-104">The **RetentionPolicyTags** element contains a list of retention tags returned in the response of the **GetUserRetentionPolicyTags** WSDL operation.</span></span> 
  
```XML
<RetentionPolicyTags>
   <RetentionPolicyTag/>
</RetentionPolicyTags>
```

 <span data-ttu-id="c4354-105">**ArrayOfRetentionPolicyTagsType**</span><span class="sxs-lookup"><span data-stu-id="c4354-105">**ArrayOfRetentionPolicyTagsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c4354-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c4354-106">Attributes and elements</span></span>

<span data-ttu-id="c4354-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c4354-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c4354-108">属性</span><span class="sxs-lookup"><span data-stu-id="c4354-108">Attributes</span></span>

<span data-ttu-id="c4354-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c4354-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c4354-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c4354-110">Child elements</span></span>

[<span data-ttu-id="c4354-111">New-retentionpolicytag</span><span class="sxs-lookup"><span data-stu-id="c4354-111">RetentionPolicyTag</span></span>](retentionpolicytag.md)
  
### <a name="parent-elements"></a><span data-ttu-id="c4354-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c4354-112">Parent elements</span></span>

[<span data-ttu-id="c4354-113">GetUserRetentionPolicyTagsResponse</span><span class="sxs-lookup"><span data-stu-id="c4354-113">GetUserRetentionPolicyTagsResponse</span></span>](getuserretentionpolicytagsresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="c4354-114">注釈</span><span class="sxs-lookup"><span data-stu-id="c4354-114">Remarks</span></span>

<span data-ttu-id="c4354-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c4354-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c4354-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c4354-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c4354-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c4354-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c4354-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="c4354-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c4354-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c4354-119">Schema name</span></span>  <br/> |<span data-ttu-id="c4354-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="c4354-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c4354-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c4354-121">Validation file</span></span>  <br/> |<span data-ttu-id="c4354-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="c4354-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c4354-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c4354-123">Can be empty</span></span>  <br/> |<span data-ttu-id="c4354-124">false</span><span class="sxs-lookup"><span data-stu-id="c4354-124">false</span></span>  <br/> |
   

