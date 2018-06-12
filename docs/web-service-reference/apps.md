---
title: アプリ
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f6f0a2ca-22dd-4789-9eed-f0c1ec9036c4
description: アプリケーション要素には、メールボックスにインストールされているアプリケーションのすべての XML マニフェスト ファイルに関する情報が含まれています。
ms.openlocfilehash: 81b0cb76b02fcc9145f6d70eff12a0a0ac0ad51f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759426"
---
# <a name="apps"></a><span data-ttu-id="ad93a-103">アプリ</span><span class="sxs-lookup"><span data-stu-id="ad93a-103">Apps</span></span>

<span data-ttu-id="ad93a-104">**アプリケーション**要素には、メールボックスにインストールされているアプリケーションのすべての XML マニフェスト ファイルに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ad93a-104">The **Apps** element contains information about all the XML manifest files for apps installed in a mailbox.</span></span> 
  
```XML
<Apps>
    <App/>
</Apps>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="ad93a-105">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ad93a-105">Attributes and elements</span></span>

<span data-ttu-id="ad93a-106">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ad93a-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad93a-107">属性</span><span class="sxs-lookup"><span data-stu-id="ad93a-107">Attributes</span></span>

<span data-ttu-id="ad93a-108">なし。</span><span class="sxs-lookup"><span data-stu-id="ad93a-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad93a-109">子要素</span><span class="sxs-lookup"><span data-stu-id="ad93a-109">Child elements</span></span>

[<span data-ttu-id="ad93a-110">App</span><span class="sxs-lookup"><span data-stu-id="ad93a-110">App</span></span>](app.md)
  
### <a name="parent-elements"></a><span data-ttu-id="ad93a-111">親要素</span><span class="sxs-lookup"><span data-stu-id="ad93a-111">Parent elements</span></span>

[<span data-ttu-id="ad93a-112">GetAppManifestsResponse</span><span class="sxs-lookup"><span data-stu-id="ad93a-112">GetAppManifestsResponse</span></span>](getappmanifestsresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="ad93a-113">Remarks</span><span class="sxs-lookup"><span data-stu-id="ad93a-113">Remarks</span></span>

<span data-ttu-id="ad93a-114">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ad93a-114">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="ad93a-115">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ad93a-115">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad93a-116">要素情報</span><span class="sxs-lookup"><span data-stu-id="ad93a-116">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad93a-117">名前空間</span><span class="sxs-lookup"><span data-stu-id="ad93a-117">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ad93a-118">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ad93a-118">Schema Name</span></span>  <br/> |<span data-ttu-id="ad93a-119">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="ad93a-119">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ad93a-120">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ad93a-120">Validation File</span></span>  <br/> |<span data-ttu-id="ad93a-121">該当しない</span><span class="sxs-lookup"><span data-stu-id="ad93a-121">Not applicable</span></span>  <br/> |
|<span data-ttu-id="ad93a-122">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ad93a-122">Can be Empty</span></span>  <br/> |<span data-ttu-id="ad93a-123">False</span><span class="sxs-lookup"><span data-stu-id="ad93a-123">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ad93a-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="ad93a-124">See also</span></span>

- [<span data-ttu-id="ad93a-125">App</span><span class="sxs-lookup"><span data-stu-id="ad93a-125">App</span></span>](app.md)
- [<span data-ttu-id="ad93a-126">GetAppManifestsResponse</span><span class="sxs-lookup"><span data-stu-id="ad93a-126">GetAppManifestsResponse</span></span>](getappmanifestsresponse.md)
- [<span data-ttu-id="ad93a-127">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ad93a-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

