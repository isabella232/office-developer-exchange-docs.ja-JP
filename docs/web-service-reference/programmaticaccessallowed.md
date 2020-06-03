---
title: ProgrammaticAccessAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a1fc7dff-a303-4809-b7f4-9672f86c183c
description: ProgrammaticAccessAllowed 要素は、権限管理データのプログラムによるアクセスを有効にするかどうかを指定します。
ms.openlocfilehash: 8a5cf4e57a97807e5940a0402768d7123b9912d2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465640"
---
# <a name="programmaticaccessallowed"></a><span data-ttu-id="f76f1-103">ProgrammaticAccessAllowed</span><span class="sxs-lookup"><span data-stu-id="f76f1-103">ProgrammaticAccessAllowed</span></span>

<span data-ttu-id="f76f1-104">**ProgrammaticAccessAllowed**要素は、権限管理データのプログラムによるアクセスを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f76f1-104">The **ProgrammaticAccessAllowed** element specifies whether programmatic access is enabled for rights managed data.</span></span> 
  
```XML
<ProgrammaticAccessAllowed> true | false </ProgrammaticAccessAllowed>
```

 <span data-ttu-id="f76f1-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f76f1-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f76f1-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f76f1-106">Attributes and elements</span></span>

<span data-ttu-id="f76f1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f76f1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f76f1-108">属性</span><span class="sxs-lookup"><span data-stu-id="f76f1-108">Attributes</span></span>

<span data-ttu-id="f76f1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f76f1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f76f1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f76f1-110">Child elements</span></span>

<span data-ttu-id="f76f1-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f76f1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f76f1-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f76f1-112">Parent elements</span></span>

[<span data-ttu-id="f76f1-113">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="f76f1-113">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md)
  
## <a name="text-value"></a><span data-ttu-id="f76f1-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f76f1-114">Text value</span></span>

<span data-ttu-id="f76f1-115">**ProgrammaticAccessAllowed**要素のテキスト値が**true**の場合は、データがプログラムによってアクセス可能であることを示します。</span><span class="sxs-lookup"><span data-stu-id="f76f1-115">A text value of **true** for the **ProgrammaticAccessAllowed** element indicates that the data is programmatically accessible.</span></span> <span data-ttu-id="f76f1-116">値が**false**の場合は、データがプログラムでアクセスできないことを示します。</span><span class="sxs-lookup"><span data-stu-id="f76f1-116">A value of **false** indicates that the data is not programmatically accessible.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f76f1-117">注釈</span><span class="sxs-lookup"><span data-stu-id="f76f1-117">Remarks</span></span>

<span data-ttu-id="f76f1-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f76f1-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f76f1-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f76f1-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f76f1-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f76f1-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f76f1-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="f76f1-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f76f1-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f76f1-122">Schema name</span></span>  <br/> |<span data-ttu-id="f76f1-123">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f76f1-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="f76f1-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f76f1-124">Validation file</span></span>  <br/> |<span data-ttu-id="f76f1-125">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f76f1-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f76f1-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f76f1-126">Can be empty</span></span>  <br/> |<span data-ttu-id="f76f1-127">false</span><span class="sxs-lookup"><span data-stu-id="f76f1-127">false</span></span>  <br/> |
   

