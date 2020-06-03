---
title: マニフェスト
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: af0d7435-fef6-4f0d-bd22-00e3fa576315
description: Manifest 要素には、base64 でエンコードされたアプリマニフェストファイルが含まれています。
ms.openlocfilehash: faac517bf8a8f03c6ae8abffddaf10421eed1699
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530538"
---
# <a name="manifest"></a><span data-ttu-id="e4ec3-103">マニフェスト</span><span class="sxs-lookup"><span data-stu-id="e4ec3-103">Manifest</span></span>

<span data-ttu-id="e4ec3-104">**Manifest**要素には、base64 でエンコードされたアプリマニフェストファイルが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e4ec3-104">The **Manifest** element contains the base64-encoded app manifest file.</span></span> 
  
```XML
<Manifest></Manifest>
```

 <span data-ttu-id="e4ec3-105">**base64Binary**</span><span class="sxs-lookup"><span data-stu-id="e4ec3-105">**base64Binary**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e4ec3-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e4ec3-106">Attributes and elements</span></span>

<span data-ttu-id="e4ec3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e4ec3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e4ec3-108">属性</span><span class="sxs-lookup"><span data-stu-id="e4ec3-108">Attributes</span></span>

<span data-ttu-id="e4ec3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e4ec3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e4ec3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e4ec3-110">Child elements</span></span>

<span data-ttu-id="e4ec3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e4ec3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e4ec3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e4ec3-112">Parent elements</span></span>

<span data-ttu-id="e4ec3-113">[マニフェスト](manifests.md)  | [Installapp](installapp.md)  | [Clientextension](clientextension.md)</span><span class="sxs-lookup"><span data-stu-id="e4ec3-113">[Manifests](manifests.md) | [InstallApp](installapp.md) | [ClientExtension](clientextension.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="e4ec3-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e4ec3-114">Text value</span></span>

<span data-ttu-id="e4ec3-115">Manifest 要素のテキスト値は、クライアントアプリケーションマニフェストファイルの base64 バイナリエンコード形式を ASCII で表現したものです。</span><span class="sxs-lookup"><span data-stu-id="e4ec3-115">The text value of the Manifest element is an ASCII representation of the base64 binary encoded form of the client app manifest file.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e4ec3-116">注釈</span><span class="sxs-lookup"><span data-stu-id="e4ec3-116">Remarks</span></span>

<span data-ttu-id="e4ec3-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e4ec3-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e4ec3-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e4ec3-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

