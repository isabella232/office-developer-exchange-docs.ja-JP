---
title: InstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc2ca69e-eea7-4334-b046-ec0b04d8f8c6
description: InstallApp 要素は、アプリをインストールする要求を指定します。
ms.openlocfilehash: 003a72507813677484b2d6ee75f8ff577df169e3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468006"
---
# <a name="installapp"></a><span data-ttu-id="11088-103">InstallApp</span><span class="sxs-lookup"><span data-stu-id="11088-103">InstallApp</span></span>

<span data-ttu-id="11088-104">**Installapp**要素は、アプリをインストールする要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="11088-104">The **InstallApp** element specifies the request to install an app.</span></span> 
  
```XML
<InstallApp>
    <Manifest/>
</InstallApp>
```

 <span data-ttu-id="11088-105">**InstallAppType**</span><span class="sxs-lookup"><span data-stu-id="11088-105">**InstallAppType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="11088-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="11088-106">Attributes and elements</span></span>

<span data-ttu-id="11088-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="11088-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="11088-108">属性</span><span class="sxs-lookup"><span data-stu-id="11088-108">Attributes</span></span>

<span data-ttu-id="11088-109">なし。</span><span class="sxs-lookup"><span data-stu-id="11088-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="11088-110">子要素</span><span class="sxs-lookup"><span data-stu-id="11088-110">Child elements</span></span>

|<span data-ttu-id="11088-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="11088-111">**Element**</span></span>|<span data-ttu-id="11088-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="11088-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11088-113">マニフェスト</span><span class="sxs-lookup"><span data-stu-id="11088-113">Manifest</span></span>](manifest.md) <br/> |<span data-ttu-id="11088-114">Base64 でエンコードされたアプリマニフェストファイルが保存されています。</span><span class="sxs-lookup"><span data-stu-id="11088-114">Contains the base64-encoded app manifest file.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="11088-115">親要素</span><span class="sxs-lookup"><span data-stu-id="11088-115">Parent elements</span></span>

<span data-ttu-id="11088-116">なし。</span><span class="sxs-lookup"><span data-stu-id="11088-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="11088-117">注釈</span><span class="sxs-lookup"><span data-stu-id="11088-117">Remarks</span></span>

<span data-ttu-id="11088-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="11088-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="11088-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="11088-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="11088-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="11088-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="11088-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="11088-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="11088-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="11088-122">Schema Name</span></span>  <br/> |<span data-ttu-id="11088-123">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="11088-123">Message schema</span></span>  <br/> |
|<span data-ttu-id="11088-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="11088-124">Validation File</span></span>  <br/> |<span data-ttu-id="11088-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="11088-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="11088-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="11088-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="11088-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="11088-127">See also</span></span>



- [<span data-ttu-id="11088-128">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="11088-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

