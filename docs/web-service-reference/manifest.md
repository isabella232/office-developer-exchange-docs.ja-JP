---
title: マニフェスト
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: af0d7435-fef6-4f0d-bd22-00e3fa576315
description: マニフェストの要素には、base64 でエンコードされたアプリケーション マニフェスト ファイルが含まれています。
ms.openlocfilehash: 7388e40a96a082666519d1c67af5b218b2b9ab01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832343"
---
# <a name="manifest"></a><span data-ttu-id="3a1b4-103">マニフェスト</span><span class="sxs-lookup"><span data-stu-id="3a1b4-103">Manifest</span></span>

<span data-ttu-id="3a1b4-104">**マニフェスト**の要素には、base64 でエンコードされたアプリケーション マニフェスト ファイルが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3a1b4-104">The **Manifest** element contains the base64-encoded app manifest file.</span></span> 
  
```XML
<Manifest></Manifest>
```

 <span data-ttu-id="3a1b4-105">**base64Binary**</span><span class="sxs-lookup"><span data-stu-id="3a1b4-105">**base64Binary**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a1b4-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3a1b4-106">Attributes and elements</span></span>

<span data-ttu-id="3a1b4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3a1b4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a1b4-108">属性</span><span class="sxs-lookup"><span data-stu-id="3a1b4-108">Attributes</span></span>

<span data-ttu-id="3a1b4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3a1b4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a1b4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3a1b4-110">Child elements</span></span>

<span data-ttu-id="3a1b4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="3a1b4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3a1b4-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3a1b4-112">Parent elements</span></span>

<span data-ttu-id="3a1b4-113">[マニフェスト](manifests.md) | [InstallApp](installapp.md) | [ClientExtension](clientextension.md)</span><span class="sxs-lookup"><span data-stu-id="3a1b4-113">[Manifests](manifests.md) | [InstallApp](installapp.md) | [ClientExtension](clientextension.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3a1b4-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3a1b4-114">Text value</span></span>

<span data-ttu-id="3a1b4-115">マニフェストの要素のテキスト値は、クライアント アプリケーションのマニフェスト ファイルの ASCII エンコードされた base64 をバイナリの表現形式です。</span><span class="sxs-lookup"><span data-stu-id="3a1b4-115">The text value of the Manifest element is an ASCII representation of the base64 binary encoded form of the client app manifest file.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3a1b4-116">備考</span><span class="sxs-lookup"><span data-stu-id="3a1b4-116">Remarks</span></span>

<span data-ttu-id="3a1b4-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3a1b4-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3a1b4-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3a1b4-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

