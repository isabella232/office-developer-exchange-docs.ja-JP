---
title: GetSearchableMailboxesResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0fcc2f53-742b-46ae-bbab-c3295a3d69e7
description: GetSearchableMailboxesResponse 要素には、Getsearchablemailemailrequest 要求への応答が含まれています。
ms.openlocfilehash: 680fde9d9ad34dd0384e00da023796d004b66b1b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458265"
---
# <a name="getsearchablemailboxesresponse"></a><span data-ttu-id="aae2e-103">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="aae2e-103">GetSearchableMailboxesResponse</span></span>

<span data-ttu-id="aae2e-104">**GetSearchableMailboxesResponse**要素には、 **Getsearchablemailemailrequest**要求への応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="aae2e-104">The **GetSearchableMailboxesResponse** element contains the response to a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<GetSearchableMailboxesResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SearchableMailboxes/>
   <FailedMailboxes/>
</GetSearchableMailboxesResponse>
```

 <span data-ttu-id="aae2e-105">**GetSearchableMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="aae2e-105">**GetSearchableMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aae2e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="aae2e-106">Attributes and elements</span></span>

<span data-ttu-id="aae2e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="aae2e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aae2e-108">属性</span><span class="sxs-lookup"><span data-stu-id="aae2e-108">Attributes</span></span>

<span data-ttu-id="aae2e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="aae2e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aae2e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="aae2e-110">Child elements</span></span>

<span data-ttu-id="aae2e-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)  | [Searchablemailboxes](searchablemailboxes.md)  | [失敗したメールボックス](failedmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="aae2e-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [SearchableMailboxes](searchablemailboxes.md) | [FailedMailboxes](failedmailboxes.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="aae2e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="aae2e-112">Parent elements</span></span>

<span data-ttu-id="aae2e-113">なし。</span><span class="sxs-lookup"><span data-stu-id="aae2e-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="aae2e-114">注釈</span><span class="sxs-lookup"><span data-stu-id="aae2e-114">Remarks</span></span>

<span data-ttu-id="aae2e-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="aae2e-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="aae2e-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="aae2e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aae2e-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="aae2e-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aae2e-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="aae2e-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aae2e-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="aae2e-119">Schema name</span></span>  <br/> |<span data-ttu-id="aae2e-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="aae2e-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="aae2e-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="aae2e-121">Validation file</span></span>  <br/> |<span data-ttu-id="aae2e-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="aae2e-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aae2e-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="aae2e-123">Can be empty</span></span>  <br/> |<span data-ttu-id="aae2e-124">false</span><span class="sxs-lookup"><span data-stu-id="aae2e-124">false</span></span>  <br/> |
   

