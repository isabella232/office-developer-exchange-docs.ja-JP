---
title: PlayOnPhoneEnabled
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
description: PlayOnPhoneEnabled 要素は、電話での再生機能が有効になっているかどうかを示します。
ms.openlocfilehash: 1a6c5c41a4fe723f37d07ad0151dfbd6512cf4f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832829"
---
# <a name="playonphoneenabled"></a><span data-ttu-id="8ed05-103">PlayOnPhoneEnabled</span><span class="sxs-lookup"><span data-stu-id="8ed05-103">PlayOnPhoneEnabled</span></span>

<span data-ttu-id="8ed05-104">**PlayOnPhoneEnabled**要素は、電話での再生機能が有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8ed05-104">The **PlayOnPhoneEnabled** element indicates whether the Play-on-Phone feature is enabled.</span></span> 
  
```XML
<PlayOnPhoneEnabled>true | false</PlayOnPhoneEnabled>
```

 <span data-ttu-id="8ed05-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="8ed05-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8ed05-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8ed05-106">Attributes and elements</span></span>

<span data-ttu-id="8ed05-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8ed05-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8ed05-108">属性</span><span class="sxs-lookup"><span data-stu-id="8ed05-108">Attributes</span></span>

<span data-ttu-id="8ed05-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8ed05-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8ed05-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8ed05-110">Child elements</span></span>

<span data-ttu-id="8ed05-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8ed05-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8ed05-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8ed05-112">Parent elements</span></span>

|<span data-ttu-id="8ed05-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="8ed05-113">**Element**</span></span>|<span data-ttu-id="8ed05-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="8ed05-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8ed05-115">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ed05-115">UnifiedMessagingConfiguration</span></span>](unifiedmessagingconfiguration.md) <br/> |<span data-ttu-id="8ed05-116">ユニファイド メッセージング サービスの構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8ed05-116">Contains configuration information for the Unified Messaging service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8ed05-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8ed05-117">Text value</span></span>

<span data-ttu-id="8ed05-118">アカウントの電話での再生が有効になっている場合、 **PlayOnPhoneEnabled**要素が**true**の場合それ以外の場合、値が**false**にします。</span><span class="sxs-lookup"><span data-stu-id="8ed05-118">The **PlayOnPhoneEnabled** element has a value of **true** if play-on-phone is enabled for the account; otherwise, the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8ed05-119">備考</span><span class="sxs-lookup"><span data-stu-id="8ed05-119">Remarks</span></span>

<span data-ttu-id="8ed05-120">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="8ed05-120">This element is required.</span></span>
  
<span data-ttu-id="8ed05-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8ed05-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8ed05-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="8ed05-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8ed05-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="8ed05-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8ed05-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8ed05-124">Schema Name</span></span>  <br/> |<span data-ttu-id="8ed05-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8ed05-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="8ed05-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8ed05-126">Validation File</span></span>  <br/> |<span data-ttu-id="8ed05-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8ed05-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8ed05-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8ed05-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="8ed05-129">False</span><span class="sxs-lookup"><span data-stu-id="8ed05-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8ed05-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="8ed05-130">See also</span></span>



- [<span data-ttu-id="8ed05-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="8ed05-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

