---
title: InstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc2ca69e-eea7-4334-b046-ec0b04d8f8c6
description: InstallApp 要素は、アプリケーションをインストールするのには要求を指定します。
ms.openlocfilehash: d9b7412865c003b89eccbdd92aa6ff9968048191
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831949"
---
# <a name="installapp"></a><span data-ttu-id="faa5d-103">InstallApp</span><span class="sxs-lookup"><span data-stu-id="faa5d-103">InstallApp</span></span>

<span data-ttu-id="faa5d-104">**InstallApp**要素は、アプリケーションをインストールするのには要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="faa5d-104">The **InstallApp** element specifies the request to install an app.</span></span> 
  
```XML
<InstallApp>
    <Manifest/>
</InstallApp>
```

 <span data-ttu-id="faa5d-105">**InstallAppType**</span><span class="sxs-lookup"><span data-stu-id="faa5d-105">**InstallAppType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="faa5d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="faa5d-106">Attributes and elements</span></span>

<span data-ttu-id="faa5d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="faa5d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="faa5d-108">属性</span><span class="sxs-lookup"><span data-stu-id="faa5d-108">Attributes</span></span>

<span data-ttu-id="faa5d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="faa5d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="faa5d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="faa5d-110">Child elements</span></span>

|<span data-ttu-id="faa5d-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="faa5d-111">**Element**</span></span>|<span data-ttu-id="faa5d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="faa5d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="faa5d-113">Manifest</span><span class="sxs-lookup"><span data-stu-id="faa5d-113">Manifest</span></span>](manifest.md) <br/> |<span data-ttu-id="faa5d-114">Base64 でエンコードされたアプリケーション マニフェスト ファイルが含まれています。</span><span class="sxs-lookup"><span data-stu-id="faa5d-114">Contains the base64-encoded app manifest file.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="faa5d-115">親要素</span><span class="sxs-lookup"><span data-stu-id="faa5d-115">Parent elements</span></span>

<span data-ttu-id="faa5d-116">なし。</span><span class="sxs-lookup"><span data-stu-id="faa5d-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="faa5d-117">備考</span><span class="sxs-lookup"><span data-stu-id="faa5d-117">Remarks</span></span>

<span data-ttu-id="faa5d-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="faa5d-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="faa5d-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="faa5d-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="faa5d-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="faa5d-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="faa5d-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="faa5d-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="faa5d-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="faa5d-122">Schema Name</span></span>  <br/> |<span data-ttu-id="faa5d-123">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="faa5d-123">Message schema</span></span>  <br/> |
|<span data-ttu-id="faa5d-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="faa5d-124">Validation File</span></span>  <br/> |<span data-ttu-id="faa5d-125">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="faa5d-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="faa5d-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="faa5d-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="faa5d-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="faa5d-127">See also</span></span>



- [<span data-ttu-id="faa5d-128">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="faa5d-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

