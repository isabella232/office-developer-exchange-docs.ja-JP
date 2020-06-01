---
title: ClientExtensions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0073d195-75fd-4c89-97e0-2ad6d91f99f9
description: ClientExtensions 要素には、アプリに関するユーザーおよび構成情報の配列が含まれています。
ms.openlocfilehash: 016b4c910f3c21a20d72b926a1c568925aa9d37e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461458"
---
# <a name="clientextensions"></a><span data-ttu-id="0843e-103">ClientExtensions</span><span class="sxs-lookup"><span data-stu-id="0843e-103">ClientExtensions</span></span>

<span data-ttu-id="0843e-104">**Clientextensions**要素には、アプリに関するユーザーおよび構成情報の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0843e-104">The **ClientExtensions** element contains an array of user and configuration information about apps.</span></span> 
  
```XML
<ClientExtensions>
   <ClientExtension/>
</ClientExtensions>
```

 <span data-ttu-id="0843e-105">**ArrayOfClientExtensionsType**</span><span class="sxs-lookup"><span data-stu-id="0843e-105">**ArrayOfClientExtensionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0843e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0843e-106">Attributes and elements</span></span>

<span data-ttu-id="0843e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0843e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0843e-108">属性</span><span class="sxs-lookup"><span data-stu-id="0843e-108">Attributes</span></span>

<span data-ttu-id="0843e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0843e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0843e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0843e-110">Child elements</span></span>

|<span data-ttu-id="0843e-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="0843e-111">**Element**</span></span>|<span data-ttu-id="0843e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="0843e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0843e-113">ClientExtension</span><span class="sxs-lookup"><span data-stu-id="0843e-113">ClientExtension</span></span>](clientextension.md) <br/> |<span data-ttu-id="0843e-114">アプリに関するユーザーおよび構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0843e-114">Contains user and configuration information about an app.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0843e-115">親要素</span><span class="sxs-lookup"><span data-stu-id="0843e-115">Parent elements</span></span>

|<span data-ttu-id="0843e-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="0843e-116">**Element**</span></span>|<span data-ttu-id="0843e-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="0843e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0843e-118">GetClientExtensionResponse</span><span class="sxs-lookup"><span data-stu-id="0843e-118">GetClientExtensionResponse</span></span>](getclientextensionresponse.md) <br/> |<span data-ttu-id="0843e-119">アプリの構成情報を取得するための応答を表します。</span><span class="sxs-lookup"><span data-stu-id="0843e-119">Represents a response to get configuration information about an app.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0843e-120">注釈</span><span class="sxs-lookup"><span data-stu-id="0843e-120">Remarks</span></span>

<span data-ttu-id="0843e-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0843e-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0843e-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0843e-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0843e-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0843e-123">Element information</span></span>

||
|:-----|
|<span data-ttu-id="0843e-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="0843e-124">Namespace</span></span>  <br/> |
|<span data-ttu-id="0843e-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0843e-125">Schema Name</span></span>  <br/> |
|<span data-ttu-id="0843e-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0843e-126">Validation File</span></span>  <br/> |
|<span data-ttu-id="0843e-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0843e-127">Can be Empty</span></span>  <br/> |
   

