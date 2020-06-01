---
title: GetImItemsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7b340fef-61cd-4a56-bb69-d935f7f7f552
description: GetImItemsResponse 要素は、GetImItems 要求に対する応答を定義します。
ms.openlocfilehash: 71547834243a7d377a8b1de527b6db78280c7530
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456438"
---
# <a name="getimitemsresponse"></a><span data-ttu-id="bdfd5-103">GetImItemsResponse</span><span class="sxs-lookup"><span data-stu-id="bdfd5-103">GetImItemsResponse</span></span>

<span data-ttu-id="bdfd5-104">**Getimitemsresponse**要素は、 **getimitems**要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="bdfd5-104">The **GetImItemsResponse** element defines a response to a **GetImItems** request.</span></span> 
  
```XML
<GetImItemsResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ImItemList/>
</GetImItemsResponse>
```

 <span data-ttu-id="bdfd5-105">**GetImItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="bdfd5-105">**GetImItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bdfd5-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="bdfd5-106">Attributes and elements</span></span>

<span data-ttu-id="bdfd5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bdfd5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bdfd5-108">属性</span><span class="sxs-lookup"><span data-stu-id="bdfd5-108">Attributes</span></span>

<span data-ttu-id="bdfd5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bdfd5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bdfd5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="bdfd5-110">Child elements</span></span>

<span data-ttu-id="bdfd5-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)  | [Imitemlist](imitemlist.md)</span><span class="sxs-lookup"><span data-stu-id="bdfd5-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [ImItemList](imitemlist.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bdfd5-112">親要素</span><span class="sxs-lookup"><span data-stu-id="bdfd5-112">Parent elements</span></span>

<span data-ttu-id="bdfd5-113">なし。</span><span class="sxs-lookup"><span data-stu-id="bdfd5-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bdfd5-114">注釈</span><span class="sxs-lookup"><span data-stu-id="bdfd5-114">Remarks</span></span>

<span data-ttu-id="bdfd5-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="bdfd5-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bdfd5-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="bdfd5-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bdfd5-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="bdfd5-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bdfd5-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="bdfd5-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bdfd5-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bdfd5-119">Schema name</span></span>  <br/> |<span data-ttu-id="bdfd5-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="bdfd5-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bdfd5-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bdfd5-121">Validation file</span></span>  <br/> |<span data-ttu-id="bdfd5-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="bdfd5-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bdfd5-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="bdfd5-123">Can be empty</span></span>  <br/> ||
   

