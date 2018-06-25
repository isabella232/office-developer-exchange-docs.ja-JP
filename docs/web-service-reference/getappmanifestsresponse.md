---
title: GetAppManifestsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 86cf88f4-09c4-436a-a100-ac5cba0c4388
description: GetAppManifestsResponse 要素は、GetAppManifests 操作の要求に対する応答を定義します。
ms.openlocfilehash: b5eac7c06c39c0ed80a362080db6b0cb37f8f4ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760630"
---
# <a name="getappmanifestsresponse"></a><span data-ttu-id="4bc33-103">GetAppManifestsResponse</span><span class="sxs-lookup"><span data-stu-id="4bc33-103">GetAppManifestsResponse</span></span>

<span data-ttu-id="4bc33-104">**GetAppManifestsResponse**要素は、 **GetAppManifests**操作の要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="4bc33-104">The **GetAppManifestsResponse** element defines the response for a **GetAppManifests** operation request.</span></span> 
  
```XML
<GetAppManifestsResponse>
    <ResponseCode/>
    <Manifests/>
</GetAppManifestsResponse>
```

 <span data-ttu-id="4bc33-105">**GetAppManifestsResponseType**</span><span class="sxs-lookup"><span data-stu-id="4bc33-105">**GetAppManifestsResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4bc33-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4bc33-106">Attributes and elements</span></span>

<span data-ttu-id="4bc33-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4bc33-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4bc33-108">属性</span><span class="sxs-lookup"><span data-stu-id="4bc33-108">Attributes</span></span>

<span data-ttu-id="4bc33-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4bc33-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4bc33-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4bc33-110">Child elements</span></span>

<span data-ttu-id="4bc33-111">[ResponseCode](responsecode.md) | [マニフェスト](manifests.md) | [アプリケーション](apps.md)</span><span class="sxs-lookup"><span data-stu-id="4bc33-111">[ResponseCode](responsecode.md) | [Manifests](manifests.md) | [Apps](apps.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4bc33-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4bc33-112">Parent elements</span></span>

<span data-ttu-id="4bc33-113">なし。</span><span class="sxs-lookup"><span data-stu-id="4bc33-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4bc33-114">備考</span><span class="sxs-lookup"><span data-stu-id="4bc33-114">Remarks</span></span>

<span data-ttu-id="4bc33-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4bc33-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4bc33-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4bc33-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4bc33-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="4bc33-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4bc33-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="4bc33-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4bc33-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4bc33-119">Schema Name</span></span>  <br/> |<span data-ttu-id="4bc33-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="4bc33-120">Message schema</span></span>  <br/> |
|<span data-ttu-id="4bc33-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4bc33-121">Validation File</span></span>  <br/> |<span data-ttu-id="4bc33-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4bc33-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4bc33-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4bc33-123">Can Be Empty</span></span>  <br/> |<span data-ttu-id="4bc33-124">False</span><span class="sxs-lookup"><span data-stu-id="4bc33-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4bc33-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="4bc33-125">See also</span></span>



- [<span data-ttu-id="4bc33-126">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4bc33-126">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

