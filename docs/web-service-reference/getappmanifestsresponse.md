---
title: GetAppManifestsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 86cf88f4-09c4-436a-a100-ac5cba0c4388
description: GetAppManifestsResponse 要素は、GetAppManifests 操作要求に対する応答を定義します。
ms.openlocfilehash: a01f6265d6d534e2f7868b17acf19f0f5d52a01f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462965"
---
# <a name="getappmanifestsresponse"></a><span data-ttu-id="4378b-103">GetAppManifestsResponse</span><span class="sxs-lookup"><span data-stu-id="4378b-103">GetAppManifestsResponse</span></span>

<span data-ttu-id="4378b-104">**GetAppManifestsResponse**要素は、 **getappmanifests**操作要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="4378b-104">The **GetAppManifestsResponse** element defines the response for a **GetAppManifests** operation request.</span></span> 
  
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

<span data-ttu-id="4378b-105">**GetAppManifestsResponseType**</span><span class="sxs-lookup"><span data-stu-id="4378b-105">**GetAppManifestsResponseType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4378b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4378b-106">Attributes and elements</span></span>

<span data-ttu-id="4378b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4378b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4378b-108">属性</span><span class="sxs-lookup"><span data-stu-id="4378b-108">Attributes</span></span>

<span data-ttu-id="4378b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4378b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4378b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4378b-110">Child elements</span></span>

<span data-ttu-id="4378b-111">応答[Secmode](responsecode.md)  | [マニフェスト](manifests.md)  | [アプリ](apps.md)</span><span class="sxs-lookup"><span data-stu-id="4378b-111">[ResponseCode](responsecode.md) | [Manifests](manifests.md) | [Apps](apps.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4378b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4378b-112">Parent elements</span></span>

<span data-ttu-id="4378b-113">なし。</span><span class="sxs-lookup"><span data-stu-id="4378b-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4378b-114">注釈</span><span class="sxs-lookup"><span data-stu-id="4378b-114">Remarks</span></span>

<span data-ttu-id="4378b-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4378b-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4378b-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4378b-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4378b-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4378b-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4378b-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="4378b-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4378b-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4378b-119">Schema Name</span></span>  <br/> |<span data-ttu-id="4378b-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="4378b-120">Message schema</span></span>  <br/> |
|<span data-ttu-id="4378b-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4378b-121">Validation File</span></span>  <br/> |<span data-ttu-id="4378b-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="4378b-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4378b-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4378b-123">Can Be Empty</span></span>  <br/> |<span data-ttu-id="4378b-124">正しくない</span><span class="sxs-lookup"><span data-stu-id="4378b-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4378b-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="4378b-125">See also</span></span>

- [<span data-ttu-id="4378b-126">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="4378b-126">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

