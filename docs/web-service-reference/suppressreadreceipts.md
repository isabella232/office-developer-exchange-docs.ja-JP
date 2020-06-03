---
title: SuppressReadReceipts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f0805560-7a2f-455b-94d2-ec4f1e3652c3
description: SuppressReadReceipts 要素は、開封確認を抑制する必要があるかどうかを示します。
ms.openlocfilehash: aa604d4907582bd73727ba664958a589a222f9cb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455934"
---
# <a name="suppressreadreceipts"></a><span data-ttu-id="244b9-103">SuppressReadReceipts</span><span class="sxs-lookup"><span data-stu-id="244b9-103">SuppressReadReceipts</span></span>

<span data-ttu-id="244b9-104">**SuppressReadReceipts**要素は、開封確認を抑制する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="244b9-104">The **SuppressReadReceipts** element indicates whether read receipts should be suppressed.</span></span> 
  
```XML
<SuppressReadReceipts>true | false</SuppressReadReceipts>
```

 <span data-ttu-id="244b9-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="244b9-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="244b9-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="244b9-106">Attributes and elements</span></span>

<span data-ttu-id="244b9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="244b9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="244b9-108">属性</span><span class="sxs-lookup"><span data-stu-id="244b9-108">Attributes</span></span>

<span data-ttu-id="244b9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="244b9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="244b9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="244b9-110">Child elements</span></span>

<span data-ttu-id="244b9-111">なし。</span><span class="sxs-lookup"><span data-stu-id="244b9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="244b9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="244b9-112">Parent elements</span></span>

<span data-ttu-id="244b9-113">[ConversationAction](conversationaction.md)  | [Markallitemsasread](markallitemsasread.md)</span><span class="sxs-lookup"><span data-stu-id="244b9-113">[ConversationAction](conversationaction.md) | [MarkAllItemsAsRead](markallitemsasread.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="244b9-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="244b9-114">Text value</span></span>

<span data-ttu-id="244b9-115">**SuppressReadReciepts**要素のテキスト値が**true**である場合、開封確認が抑制されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="244b9-115">A text value of **true** for the **SuppressReadReciepts** element indicates that read receipts are suppressed.</span></span> <span data-ttu-id="244b9-116">値が**false**の場合、開封確認が送信者に送信されることを示します。</span><span class="sxs-lookup"><span data-stu-id="244b9-116">A value of **false** indicates that read receipts will be sent to the sender.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="244b9-117">注釈</span><span class="sxs-lookup"><span data-stu-id="244b9-117">Remarks</span></span>

<span data-ttu-id="244b9-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="244b9-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="244b9-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="244b9-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="244b9-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="244b9-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="244b9-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="244b9-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="244b9-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="244b9-122">Schema name</span></span>  <br/> |<span data-ttu-id="244b9-123">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="244b9-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="244b9-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="244b9-124">Validation file</span></span>  <br/> |<span data-ttu-id="244b9-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="244b9-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="244b9-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="244b9-126">Can be empty</span></span>  <br/> ||
   

