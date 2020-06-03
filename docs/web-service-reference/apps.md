---
title: アプリ
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f6f0a2ca-22dd-4789-9eed-f0c1ec9036c4
description: Apps 要素には、メールボックスにインストールされたアプリのすべての XML マニフェストファイルに関する情報が含まれています。
ms.openlocfilehash: b2d6f13241f68cbed449a9f9821f9a6ec6ff687a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527447"
---
# <a name="apps"></a><span data-ttu-id="024eb-103">アプリ</span><span class="sxs-lookup"><span data-stu-id="024eb-103">Apps</span></span>

<span data-ttu-id="024eb-104">**Apps**要素には、メールボックスにインストールされたアプリのすべての XML マニフェストファイルに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="024eb-104">The **Apps** element contains information about all the XML manifest files for apps installed in a mailbox.</span></span> 
  
```XML
<Apps>
    <App/>
</Apps>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="024eb-105">属性と要素</span><span class="sxs-lookup"><span data-stu-id="024eb-105">Attributes and elements</span></span>

<span data-ttu-id="024eb-106">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="024eb-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="024eb-107">属性</span><span class="sxs-lookup"><span data-stu-id="024eb-107">Attributes</span></span>

<span data-ttu-id="024eb-108">なし。</span><span class="sxs-lookup"><span data-stu-id="024eb-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="024eb-109">子要素</span><span class="sxs-lookup"><span data-stu-id="024eb-109">Child elements</span></span>

[<span data-ttu-id="024eb-110">App</span><span class="sxs-lookup"><span data-stu-id="024eb-110">App</span></span>](app.md)
  
### <a name="parent-elements"></a><span data-ttu-id="024eb-111">親要素</span><span class="sxs-lookup"><span data-stu-id="024eb-111">Parent elements</span></span>

[<span data-ttu-id="024eb-112">GetAppManifestsResponse</span><span class="sxs-lookup"><span data-stu-id="024eb-112">GetAppManifestsResponse</span></span>](getappmanifestsresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="024eb-113">注釈</span><span class="sxs-lookup"><span data-stu-id="024eb-113">Remarks</span></span>

<span data-ttu-id="024eb-114">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="024eb-114">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="024eb-115">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="024eb-115">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="024eb-116">要素の情報</span><span class="sxs-lookup"><span data-stu-id="024eb-116">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="024eb-117">Namespace</span><span class="sxs-lookup"><span data-stu-id="024eb-117">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="024eb-118">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="024eb-118">Schema Name</span></span>  <br/> |<span data-ttu-id="024eb-119">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="024eb-119">Messages schema</span></span>  <br/> |
|<span data-ttu-id="024eb-120">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="024eb-120">Validation File</span></span>  <br/> |<span data-ttu-id="024eb-121">該当なし</span><span class="sxs-lookup"><span data-stu-id="024eb-121">Not applicable</span></span>  <br/> |
|<span data-ttu-id="024eb-122">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="024eb-122">Can be Empty</span></span>  <br/> |<span data-ttu-id="024eb-123">正しくない</span><span class="sxs-lookup"><span data-stu-id="024eb-123">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="024eb-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="024eb-124">See also</span></span>

- [<span data-ttu-id="024eb-125">App</span><span class="sxs-lookup"><span data-stu-id="024eb-125">App</span></span>](app.md)
- [<span data-ttu-id="024eb-126">GetAppManifestsResponse</span><span class="sxs-lookup"><span data-stu-id="024eb-126">GetAppManifestsResponse</span></span>](getappmanifestsresponse.md)
- [<span data-ttu-id="024eb-127">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="024eb-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

