---
title: エラー コード (int)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 65537d96-edf9-41ee-9ad5-91ffe37e2269
description: エラー コード要素は、メールボックスに対して実行が失敗した検索のエラー コードを指定します。
ms.openlocfilehash: ed8a7771376f921303ea093f4be727c4146faa76
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760319"
---
# <a name="errorcode-int"></a><span data-ttu-id="9e85d-103">エラー コード (int)</span><span class="sxs-lookup"><span data-stu-id="9e85d-103">ErrorCode (int)</span></span>

<span data-ttu-id="9e85d-104">**エラー コード**要素は、メールボックスに対して実行が失敗した検索のエラー コードを指定します。</span><span class="sxs-lookup"><span data-stu-id="9e85d-104">The **ErrorCode** element specifies the error code of a failed search performed against a mailbox.</span></span> 
  
```XML
<ErrorCode></ErrorCode>
```

 <span data-ttu-id="9e85d-105">**int**</span><span class="sxs-lookup"><span data-stu-id="9e85d-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e85d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9e85d-106">Attributes and elements</span></span>

<span data-ttu-id="9e85d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9e85d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e85d-108">属性</span><span class="sxs-lookup"><span data-stu-id="9e85d-108">Attributes</span></span>

<span data-ttu-id="9e85d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9e85d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9e85d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9e85d-110">Child elements</span></span>

<span data-ttu-id="9e85d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9e85d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9e85d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9e85d-112">Parent elements</span></span>

|<span data-ttu-id="9e85d-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9e85d-113">**Element**</span></span>|<span data-ttu-id="9e85d-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9e85d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e85d-115">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="9e85d-115">FailedMailbox</span></span>](failedmailbox.md) <br/> |<span data-ttu-id="9e85d-116">メールボックスの保留状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="9e85d-116">Specifies the hold status of the mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9e85d-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9e85d-117">Text value</span></span>

<span data-ttu-id="9e85d-118">**エラー コード**要素のテキスト値は、メールボックスに対して実行が失敗した検索で返されるエラー コードです。</span><span class="sxs-lookup"><span data-stu-id="9e85d-118">The text value of the **ErrorCode** element is the error code returned for a failed search performed against a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9e85d-119">備考</span><span class="sxs-lookup"><span data-stu-id="9e85d-119">Remarks</span></span>

<span data-ttu-id="9e85d-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9e85d-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9e85d-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9e85d-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9e85d-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="9e85d-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e85d-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="9e85d-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9e85d-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9e85d-124">Schema Name</span></span>  <br/> |<span data-ttu-id="9e85d-125">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="9e85d-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="9e85d-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9e85d-126">Validation File</span></span>  <br/> |<span data-ttu-id="9e85d-127">types.xsd</span><span class="sxs-lookup"><span data-stu-id="9e85d-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9e85d-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9e85d-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9e85d-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="9e85d-129">See also</span></span>



- [<span data-ttu-id="9e85d-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9e85d-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

