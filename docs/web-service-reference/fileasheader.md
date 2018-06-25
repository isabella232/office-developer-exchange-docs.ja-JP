---
title: FileAsHeader
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0dbc22f8-9b71-4b8f-b1d4-6ae2e4bc1db6
description: FileAsHeader は、ヘッダー ファイルとして保存] オプションを指定します。
ms.openlocfilehash: a90c7a64037ff1785c710621a950154482515b13
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760483"
---
# <a name="fileasheader"></a><span data-ttu-id="f21da-103">FileAsHeader</span><span class="sxs-lookup"><span data-stu-id="f21da-103">FileAsHeader</span></span>

<span data-ttu-id="f21da-104">**FileAsHeader**は、ヘッダー**ファイルとして**保存] オプションを指定します。</span><span class="sxs-lookup"><span data-stu-id="f21da-104">The **FileAsHeader** specifies the header for the **File As** option.</span></span> 
  
```XML
<FileAsHeader></FileAsHeader>
```

 <span data-ttu-id="f21da-105">**string**</span><span class="sxs-lookup"><span data-stu-id="f21da-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f21da-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f21da-106">Attributes and elements</span></span>

<span data-ttu-id="f21da-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f21da-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f21da-108">属性</span><span class="sxs-lookup"><span data-stu-id="f21da-108">Attributes</span></span>

<span data-ttu-id="f21da-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f21da-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f21da-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f21da-110">Child elements</span></span>

<span data-ttu-id="f21da-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f21da-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f21da-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f21da-112">Parent elements</span></span>

|<span data-ttu-id="f21da-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="f21da-113">**Element**</span></span>|<span data-ttu-id="f21da-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f21da-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f21da-115">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="f21da-115">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="f21da-116">**GetPersona**の要求によって返されるペルソナ データのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="f21da-116">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f21da-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f21da-117">Text value</span></span>

<span data-ttu-id="f21da-118">**FileAsHeader**要素のテキスト値は、ヘッダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="f21da-118">The text value of the **FileAsHeader** element specifies the header.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f21da-119">備考</span><span class="sxs-lookup"><span data-stu-id="f21da-119">Remarks</span></span>

<span data-ttu-id="f21da-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f21da-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f21da-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f21da-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f21da-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="f21da-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f21da-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="f21da-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f21da-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f21da-124">Schema Name</span></span>  <br/> |<span data-ttu-id="f21da-125">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="f21da-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="f21da-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f21da-126">Validation File</span></span>  <br/> |<span data-ttu-id="f21da-127">types.xsd</span><span class="sxs-lookup"><span data-stu-id="f21da-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f21da-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f21da-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f21da-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="f21da-129">See also</span></span>



- [<span data-ttu-id="f21da-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f21da-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

