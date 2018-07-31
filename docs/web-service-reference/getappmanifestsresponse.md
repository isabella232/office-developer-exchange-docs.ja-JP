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
ms.openlocfilehash: ae9d1d853023a5b42db2e8fee2ed57f585433f69
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354149"
---
# <a name="getappmanifestsresponse"></a><span data-ttu-id="96032-103">GetAppManifestsResponse</span><span class="sxs-lookup"><span data-stu-id="96032-103">GetAppManifestsResponse</span></span>

<span data-ttu-id="96032-104">**GetAppManifestsResponse**要素は、 **GetAppManifests**操作の要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="96032-104">The **GetAppManifestsResponse** element defines the response for a **GetAppManifests** operation request.</span></span> 
  
```xml
<GetAppManifestsResponse>
    <ResponseCode/>
    <Manifests/>
</GetAppManifestsResponse>
```

```xml
<GetAppManifestsResponse>
    <ResponseCode/>
    <Apps/>
</GetAppManifestsResponse>
```

<span data-ttu-id="96032-105">**GetAppManifestsResponseType**</span><span class="sxs-lookup"><span data-stu-id="96032-105">**GetAppManifestsResponseType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="96032-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="96032-106">Attributes and elements</span></span>

<span data-ttu-id="96032-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="96032-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96032-108">属性</span><span class="sxs-lookup"><span data-stu-id="96032-108">Attributes</span></span>

<span data-ttu-id="96032-109">なし。</span><span class="sxs-lookup"><span data-stu-id="96032-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="96032-110">子要素</span><span class="sxs-lookup"><span data-stu-id="96032-110">Child elements</span></span>

<span data-ttu-id="96032-111">[ResponseCode](responsecode.md) | [マニフェスト](manifests.md) | [アプリケーション](apps.md)</span><span class="sxs-lookup"><span data-stu-id="96032-111">[ResponseCode](responsecode.md) | [Manifests](manifests.md) | [Apps](apps.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="96032-112">親要素</span><span class="sxs-lookup"><span data-stu-id="96032-112">Parent elements</span></span>

<span data-ttu-id="96032-113">なし。</span><span class="sxs-lookup"><span data-stu-id="96032-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="96032-114">注釈</span><span class="sxs-lookup"><span data-stu-id="96032-114">Remarks</span></span>

<span data-ttu-id="96032-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="96032-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="96032-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="96032-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="96032-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="96032-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96032-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="96032-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="96032-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="96032-119">Schema Name</span></span>  <br/> |<span data-ttu-id="96032-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="96032-120">Message schema</span></span>  <br/> |
|<span data-ttu-id="96032-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="96032-121">Validation File</span></span>  <br/> |<span data-ttu-id="96032-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="96032-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="96032-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="96032-123">Can Be Empty</span></span>  <br/> |<span data-ttu-id="96032-124">False</span><span class="sxs-lookup"><span data-stu-id="96032-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96032-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="96032-125">See also</span></span>

- [<span data-ttu-id="96032-126">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="96032-126">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

