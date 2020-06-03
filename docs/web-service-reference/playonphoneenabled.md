---
title: Playon電話有効
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PlayOnPhoneEnabled
api_type:
- schema
ms.assetid: 6f800912-be4c-46f9-aa1e-dff0bbf877c5
description: Playonphone Enabled 要素は、電話での再生機能が有効になっているかどうかを示します。
ms.openlocfilehash: 8342e2bcc9c767903e0f6c180000a0f00eccc311
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529932"
---
# <a name="playonphoneenabled"></a><span data-ttu-id="061b6-103">Playon電話有効</span><span class="sxs-lookup"><span data-stu-id="061b6-103">PlayOnPhoneEnabled</span></span>

<span data-ttu-id="061b6-104">**Playonphone enabled**要素は、電話での再生機能が有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="061b6-104">The **PlayOnPhoneEnabled** element indicates whether the Play-on-Phone feature is enabled.</span></span> 
  
```XML
<PlayOnPhoneEnabled>true | false</PlayOnPhoneEnabled>
```

 <span data-ttu-id="061b6-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="061b6-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="061b6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="061b6-106">Attributes and elements</span></span>

<span data-ttu-id="061b6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="061b6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="061b6-108">属性</span><span class="sxs-lookup"><span data-stu-id="061b6-108">Attributes</span></span>

<span data-ttu-id="061b6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="061b6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="061b6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="061b6-110">Child elements</span></span>

<span data-ttu-id="061b6-111">なし。</span><span class="sxs-lookup"><span data-stu-id="061b6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="061b6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="061b6-112">Parent elements</span></span>

|<span data-ttu-id="061b6-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="061b6-113">**Element**</span></span>|<span data-ttu-id="061b6-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="061b6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="061b6-115">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="061b6-115">UnifiedMessagingConfiguration</span></span>](unifiedmessagingconfiguration.md) <br/> |<span data-ttu-id="061b6-116">ユニファイドメッセージングサービスの構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="061b6-116">Contains configuration information for the Unified Messaging service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="061b6-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="061b6-117">Text value</span></span>

<span data-ttu-id="061b6-118">Phone オン電話がアカウントに対して有効になっている場合、 **Playonphone enabled**要素の値は**true**になります。それ以外の場合、値は**false**になります。</span><span class="sxs-lookup"><span data-stu-id="061b6-118">The **PlayOnPhoneEnabled** element has a value of **true** if play-on-phone is enabled for the account; otherwise, the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="061b6-119">注釈</span><span class="sxs-lookup"><span data-stu-id="061b6-119">Remarks</span></span>

<span data-ttu-id="061b6-120">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="061b6-120">This element is required.</span></span>
  
<span data-ttu-id="061b6-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="061b6-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="061b6-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="061b6-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="061b6-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="061b6-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="061b6-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="061b6-124">Schema Name</span></span>  <br/> |<span data-ttu-id="061b6-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="061b6-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="061b6-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="061b6-126">Validation File</span></span>  <br/> |<span data-ttu-id="061b6-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="061b6-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="061b6-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="061b6-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="061b6-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="061b6-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="061b6-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="061b6-130">See also</span></span>



- [<span data-ttu-id="061b6-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="061b6-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

