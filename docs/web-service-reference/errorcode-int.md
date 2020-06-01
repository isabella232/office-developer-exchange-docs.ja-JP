---
title: ErrorCode (int)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 65537d96-edf9-41ee-9ad5-91ffe37e2269
description: ErrorCode 要素は、メールボックスに対して実行された、失敗した検索のエラーコードを指定します。
ms.openlocfilehash: 24170a56e5fa23c3811fcbd27f0240e6ba3c87b7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460667"
---
# <a name="errorcode-int"></a><span data-ttu-id="4f8aa-103">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="4f8aa-103">ErrorCode (int)</span></span>

<span data-ttu-id="4f8aa-104">**ErrorCode**要素は、メールボックスに対して実行された、失敗した検索のエラーコードを指定します。</span><span class="sxs-lookup"><span data-stu-id="4f8aa-104">The **ErrorCode** element specifies the error code of a failed search performed against a mailbox.</span></span> 
  
```XML
<ErrorCode></ErrorCode>
```

 <span data-ttu-id="4f8aa-105">**int**</span><span class="sxs-lookup"><span data-stu-id="4f8aa-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4f8aa-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4f8aa-106">Attributes and elements</span></span>

<span data-ttu-id="4f8aa-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4f8aa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4f8aa-108">属性</span><span class="sxs-lookup"><span data-stu-id="4f8aa-108">Attributes</span></span>

<span data-ttu-id="4f8aa-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4f8aa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4f8aa-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4f8aa-110">Child elements</span></span>

<span data-ttu-id="4f8aa-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4f8aa-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4f8aa-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4f8aa-112">Parent elements</span></span>

|<span data-ttu-id="4f8aa-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="4f8aa-113">**Element**</span></span>|<span data-ttu-id="4f8aa-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="4f8aa-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4f8aa-115">失敗したメールボックス</span><span class="sxs-lookup"><span data-stu-id="4f8aa-115">FailedMailbox</span></span>](failedmailbox.md) <br/> |<span data-ttu-id="4f8aa-116">メールボックスの保持状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="4f8aa-116">Specifies the hold status of the mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4f8aa-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4f8aa-117">Text value</span></span>

<span data-ttu-id="4f8aa-118">**ErrorCode**要素のテキスト値は、メールボックスに対して実行された検索でエラーが発生した場合に返されるエラーコードです。</span><span class="sxs-lookup"><span data-stu-id="4f8aa-118">The text value of the **ErrorCode** element is the error code returned for a failed search performed against a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4f8aa-119">注釈</span><span class="sxs-lookup"><span data-stu-id="4f8aa-119">Remarks</span></span>

<span data-ttu-id="4f8aa-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4f8aa-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4f8aa-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4f8aa-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4f8aa-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4f8aa-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4f8aa-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="4f8aa-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4f8aa-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4f8aa-124">Schema Name</span></span>  <br/> |<span data-ttu-id="4f8aa-125">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="4f8aa-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="4f8aa-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4f8aa-126">Validation File</span></span>  <br/> |<span data-ttu-id="4f8aa-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="4f8aa-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4f8aa-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4f8aa-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4f8aa-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="4f8aa-129">See also</span></span>



- [<span data-ttu-id="4f8aa-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="4f8aa-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

