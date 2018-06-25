---
title: GetSearchableMailboxesResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0fcc2f53-742b-46ae-bbab-c3295a3d69e7
description: GetSearchableMailboxesResponse 要素には、GetSearchableMailboxes 要求への応答が含まれています。
ms.openlocfilehash: 35a671cd534d1b48b29ef836c24d97d7cbd52401
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760856"
---
# <a name="getsearchablemailboxesresponse"></a><span data-ttu-id="9a6ec-103">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="9a6ec-103">GetSearchableMailboxesResponse</span></span>

<span data-ttu-id="9a6ec-104">**GetSearchableMailboxesResponse**要素には、 **GetSearchableMailboxes**要求への応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9a6ec-104">The **GetSearchableMailboxesResponse** element contains the response to a **GetSearchableMailboxes** request.</span></span> 
  
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

 <span data-ttu-id="9a6ec-105">**GetSearchableMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="9a6ec-105">**GetSearchableMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9a6ec-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9a6ec-106">Attributes and elements</span></span>

<span data-ttu-id="9a6ec-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9a6ec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9a6ec-108">属性</span><span class="sxs-lookup"><span data-stu-id="9a6ec-108">Attributes</span></span>

<span data-ttu-id="9a6ec-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9a6ec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9a6ec-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9a6ec-110">Child elements</span></span>

<span data-ttu-id="9a6ec-111">[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [SearchableMailboxes](searchablemailboxes.md) | [FailedMailboxes](failedmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="9a6ec-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [SearchableMailboxes](searchablemailboxes.md) | [FailedMailboxes](failedmailboxes.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9a6ec-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9a6ec-112">Parent elements</span></span>

<span data-ttu-id="9a6ec-113">なし。</span><span class="sxs-lookup"><span data-stu-id="9a6ec-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9a6ec-114">備考</span><span class="sxs-lookup"><span data-stu-id="9a6ec-114">Remarks</span></span>

<span data-ttu-id="9a6ec-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9a6ec-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9a6ec-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9a6ec-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9a6ec-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="9a6ec-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9a6ec-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="9a6ec-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9a6ec-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9a6ec-119">Schema name</span></span>  <br/> |<span data-ttu-id="9a6ec-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="9a6ec-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9a6ec-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9a6ec-121">Validation file</span></span>  <br/> |<span data-ttu-id="9a6ec-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9a6ec-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9a6ec-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9a6ec-123">Can be empty</span></span>  <br/> |<span data-ttu-id="9a6ec-124">false</span><span class="sxs-lookup"><span data-stu-id="9a6ec-124">false</span></span>  <br/> |
   

