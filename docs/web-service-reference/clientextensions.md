---
title: ClientExtensions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0073d195-75fd-4c89-97e0-2ad6d91f99f9
description: ClientExtensions 要素には、アプリケーションのユーザーおよび構成情報の配列が含まれています。
ms.openlocfilehash: c2f2511154daaded09ba0e8d811baf9ce30ca138
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759630"
---
# <a name="clientextensions"></a><span data-ttu-id="345e0-103">ClientExtensions</span><span class="sxs-lookup"><span data-stu-id="345e0-103">ClientExtensions</span></span>

<span data-ttu-id="345e0-104">**ClientExtensions**要素には、アプリケーションのユーザーおよび構成情報の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="345e0-104">The **ClientExtensions** element contains an array of user and configuration information about apps.</span></span> 
  
```XML
<ClientExtensions>
   <ClientExtension/>
</ClientExtensions>
```

 <span data-ttu-id="345e0-105">**ArrayOfClientExtensionsType**</span><span class="sxs-lookup"><span data-stu-id="345e0-105">**ArrayOfClientExtensionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="345e0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="345e0-106">Attributes and elements</span></span>

<span data-ttu-id="345e0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="345e0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="345e0-108">属性</span><span class="sxs-lookup"><span data-stu-id="345e0-108">Attributes</span></span>

<span data-ttu-id="345e0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="345e0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="345e0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="345e0-110">Child elements</span></span>

|<span data-ttu-id="345e0-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="345e0-111">**Element**</span></span>|<span data-ttu-id="345e0-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="345e0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="345e0-113">ClientExtension</span><span class="sxs-lookup"><span data-stu-id="345e0-113">ClientExtension</span></span>](clientextension.md) <br/> |<span data-ttu-id="345e0-114">アプリケーションのユーザーおよび構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="345e0-114">Contains user and configuration information about an app.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="345e0-115">親要素</span><span class="sxs-lookup"><span data-stu-id="345e0-115">Parent elements</span></span>

|<span data-ttu-id="345e0-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="345e0-116">**Element**</span></span>|<span data-ttu-id="345e0-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="345e0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="345e0-118">GetClientExtensionResponse</span><span class="sxs-lookup"><span data-stu-id="345e0-118">GetClientExtensionResponse</span></span>](getclientextensionresponse.md) <br/> |<span data-ttu-id="345e0-119">アプリケーションに関する構成情報を取得するのには応答を表します。</span><span class="sxs-lookup"><span data-stu-id="345e0-119">Represents a response to get configuration information about an app.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="345e0-120">備考</span><span class="sxs-lookup"><span data-stu-id="345e0-120">Remarks</span></span>

<span data-ttu-id="345e0-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="345e0-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="345e0-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="345e0-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="345e0-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="345e0-123">Element information</span></span>

||
|:-----|
|<span data-ttu-id="345e0-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="345e0-124">Namespace</span></span>  <br/> |
|<span data-ttu-id="345e0-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="345e0-125">Schema Name</span></span>  <br/> |
|<span data-ttu-id="345e0-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="345e0-126">Validation File</span></span>  <br/> |
|<span data-ttu-id="345e0-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="345e0-127">Can be Empty</span></span>  <br/> |
   

