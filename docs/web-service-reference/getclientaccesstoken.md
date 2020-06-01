---
title: GetClientAccessToken
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3704435b-9c84-4cff-a2a0-8288b4ca31ae
description: GetClientAccessToken 要素には、クライアントアクセストークンを取得する要求が含まれています。
ms.openlocfilehash: f0306f0d608300131ecbde500ed3b62eab0c7c66
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461094"
---
# <a name="getclientaccesstoken"></a><span data-ttu-id="b6840-103">GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="b6840-103">GetClientAccessToken</span></span>

<span data-ttu-id="b6840-104">**GetClientAccessToken**要素には、クライアントアクセストークンを取得する要求が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b6840-104">The **GetClientAccessToken** element contains a request to get a client access token.</span></span> 
  
```XML
<GetClientAccessToken>
   <TokenRequests/>
</GetClientAccessToken>
```

 <span data-ttu-id="b6840-105">**GetClientAccessTokenType**</span><span class="sxs-lookup"><span data-stu-id="b6840-105">**GetClientAccessTokenType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b6840-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b6840-106">Attributes and elements</span></span>

<span data-ttu-id="b6840-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b6840-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b6840-108">属性</span><span class="sxs-lookup"><span data-stu-id="b6840-108">Attributes</span></span>

<span data-ttu-id="b6840-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b6840-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b6840-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b6840-110">Child elements</span></span>

[<span data-ttu-id="b6840-111">TokenRequests</span><span class="sxs-lookup"><span data-stu-id="b6840-111">TokenRequests</span></span>](tokenrequests.md)
  
### <a name="parent-elements"></a><span data-ttu-id="b6840-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b6840-112">Parent elements</span></span>

<span data-ttu-id="b6840-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b6840-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b6840-114">注釈</span><span class="sxs-lookup"><span data-stu-id="b6840-114">Remarks</span></span>

<span data-ttu-id="b6840-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b6840-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b6840-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b6840-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b6840-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b6840-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6840-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="b6840-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b6840-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b6840-119">Schema name</span></span>  <br/> |<span data-ttu-id="b6840-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="b6840-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b6840-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b6840-121">Validation file</span></span>  <br/> |<span data-ttu-id="b6840-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b6840-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b6840-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b6840-123">Can be empty</span></span>  <br/> ||
   

