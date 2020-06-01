---
title: GetImItemListResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00422885-0e7b-4b50-a9ca-01f24ff9858f
description: GetImItemListResponse 要素は、GetImItemList 要求に対する応答を定義します。
ms.openlocfilehash: e1e6e30bc1304cf4898b125d3a041c1f0a8a9ab6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456053"
---
# <a name="getimitemlistresponse"></a><span data-ttu-id="82d1a-103">GetImItemListResponse</span><span class="sxs-lookup"><span data-stu-id="82d1a-103">GetImItemListResponse</span></span>

<span data-ttu-id="82d1a-104">**Getimitemlistresponse**要素は、 **getimitemlist**要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="82d1a-104">The **GetImItemListResponse** element defines a response to a **GetImItemList** request.</span></span> 
  
```XML
<GetImItemListResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ImItemList/>
</GetImItemListResponse>
```

 <span data-ttu-id="82d1a-105">**GetImItemListResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="82d1a-105">**GetImItemListResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="82d1a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="82d1a-106">Attributes and elements</span></span>

<span data-ttu-id="82d1a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="82d1a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="82d1a-108">属性</span><span class="sxs-lookup"><span data-stu-id="82d1a-108">Attributes</span></span>

<span data-ttu-id="82d1a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="82d1a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="82d1a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="82d1a-110">Child elements</span></span>

<span data-ttu-id="82d1a-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)  | [Imitemlist](imitemlist.md)</span><span class="sxs-lookup"><span data-stu-id="82d1a-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [ImItemList](imitemlist.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="82d1a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="82d1a-112">Parent elements</span></span>

<span data-ttu-id="82d1a-113">なし。</span><span class="sxs-lookup"><span data-stu-id="82d1a-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="82d1a-114">注釈</span><span class="sxs-lookup"><span data-stu-id="82d1a-114">Remarks</span></span>

<span data-ttu-id="82d1a-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="82d1a-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="82d1a-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="82d1a-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="82d1a-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="82d1a-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="82d1a-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="82d1a-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="82d1a-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="82d1a-119">Schema name</span></span>  <br/> |<span data-ttu-id="82d1a-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="82d1a-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="82d1a-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="82d1a-121">Validation file</span></span>  <br/> |<span data-ttu-id="82d1a-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="82d1a-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="82d1a-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="82d1a-123">Can be empty</span></span>  <br/> ||
   

