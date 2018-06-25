---
title: ProgrammaticAccessAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a1fc7dff-a303-4809-b7f4-9672f86c183c
description: ProgrammaticAccessAllowed 要素は、権限の管理対象データのプログラムによるアクセスが有効になっているかどうかを指定します。
ms.openlocfilehash: 50bcce745bd94bf9c2e5ced93825722307e0a096
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832889"
---
# <a name="programmaticaccessallowed"></a><span data-ttu-id="16610-103">ProgrammaticAccessAllowed</span><span class="sxs-lookup"><span data-stu-id="16610-103">ProgrammaticAccessAllowed</span></span>

<span data-ttu-id="16610-104">**ProgrammaticAccessAllowed**要素は、権限の管理対象データのプログラムによるアクセスが有効になっているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="16610-104">The **ProgrammaticAccessAllowed** element specifies whether programmatic access is enabled for rights managed data.</span></span> 
  
```XML
<ProgrammaticAccessAllowed> true | false </ProgrammaticAccessAllowed>
```

 <span data-ttu-id="16610-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="16610-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="16610-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="16610-106">Attributes and elements</span></span>

<span data-ttu-id="16610-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="16610-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="16610-108">属性</span><span class="sxs-lookup"><span data-stu-id="16610-108">Attributes</span></span>

<span data-ttu-id="16610-109">なし。</span><span class="sxs-lookup"><span data-stu-id="16610-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="16610-110">子要素</span><span class="sxs-lookup"><span data-stu-id="16610-110">Child elements</span></span>

<span data-ttu-id="16610-111">なし。</span><span class="sxs-lookup"><span data-stu-id="16610-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="16610-112">親要素</span><span class="sxs-lookup"><span data-stu-id="16610-112">Parent elements</span></span>

[<span data-ttu-id="16610-113">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="16610-113">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md)
  
## <a name="text-value"></a><span data-ttu-id="16610-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="16610-114">Text value</span></span>

<span data-ttu-id="16610-115">の**場合は true** 、 **ProgrammaticAccessAllowed**要素のテキスト値は、データがプログラムでアクセスできることを示します。</span><span class="sxs-lookup"><span data-stu-id="16610-115">A text value of **true** for the **ProgrammaticAccessAllowed** element indicates that the data is programmatically accessible.</span></span> <span data-ttu-id="16610-116">**False**の値は、データがプログラムによってアクセス可能ではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="16610-116">A value of **false** indicates that the data is not programmatically accessible.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="16610-117">備考</span><span class="sxs-lookup"><span data-stu-id="16610-117">Remarks</span></span>

<span data-ttu-id="16610-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="16610-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="16610-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="16610-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="16610-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="16610-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="16610-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="16610-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="16610-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="16610-122">Schema name</span></span>  <br/> |<span data-ttu-id="16610-123">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="16610-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="16610-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="16610-124">Validation file</span></span>  <br/> |<span data-ttu-id="16610-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="16610-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="16610-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="16610-126">Can be empty</span></span>  <br/> |<span data-ttu-id="16610-127">false</span><span class="sxs-lookup"><span data-stu-id="16610-127">false</span></span>  <br/> |
   

