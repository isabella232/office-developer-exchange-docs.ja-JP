---
title: ReadFlag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9d91aa89-9f9f-4877-846d-aaf48bbeec7c
description: ReadFlag 要素は、フォルダー内のアイテムに設定する読み取り状態を示します。
ms.openlocfilehash: 1d3b9f3fe199ed2e63bdb632135120a5f89f4d1f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529897"
---
# <a name="readflag"></a><span data-ttu-id="4370d-103">ReadFlag</span><span class="sxs-lookup"><span data-stu-id="4370d-103">ReadFlag</span></span>

<span data-ttu-id="4370d-104">**Readflag**要素は、フォルダー内のアイテムに設定する読み取り状態を示します。</span><span class="sxs-lookup"><span data-stu-id="4370d-104">The **ReadFlag** element indicates the read state to set on items in a folder.</span></span> 
  
```XML
<ReadFlag>true | false</ReadFlag>
```

 <span data-ttu-id="4370d-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="4370d-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4370d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4370d-106">Attributes and elements</span></span>

<span data-ttu-id="4370d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4370d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4370d-108">属性</span><span class="sxs-lookup"><span data-stu-id="4370d-108">Attributes</span></span>

<span data-ttu-id="4370d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4370d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4370d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4370d-110">Child elements</span></span>

<span data-ttu-id="4370d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4370d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4370d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4370d-112">Parent elements</span></span>

[<span data-ttu-id="4370d-113">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="4370d-113">MarkAllItemsAsRead</span></span>](markallitemsasread.md)
  
## <a name="text-value"></a><span data-ttu-id="4370d-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4370d-114">Text value</span></span>

<span data-ttu-id="4370d-115">**Readflag**要素のテキスト値が**true の場合**は、フォルダー内のアイテムが開封済みとしてマークされることを示します。</span><span class="sxs-lookup"><span data-stu-id="4370d-115">A text value of **true** for the **ReadFlag** element indicates that the items in the folder will be marked as read.</span></span> <span data-ttu-id="4370d-116">値が**false**の場合は、フォルダー内のアイテムが未読としてマークされることを示します。</span><span class="sxs-lookup"><span data-stu-id="4370d-116">A value of **false** indicates that the items in the folder will be marked as unread.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4370d-117">注釈</span><span class="sxs-lookup"><span data-stu-id="4370d-117">Remarks</span></span>

<span data-ttu-id="4370d-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4370d-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4370d-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4370d-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4370d-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4370d-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4370d-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="4370d-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4370d-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4370d-122">Schema name</span></span>  <br/> |<span data-ttu-id="4370d-123">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="4370d-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4370d-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4370d-124">Validation file</span></span>  <br/> |<span data-ttu-id="4370d-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="4370d-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4370d-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4370d-126">Can be empty</span></span>  <br/> ||
   

