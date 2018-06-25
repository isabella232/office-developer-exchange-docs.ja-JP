---
title: GetImItemsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7b340fef-61cd-4a56-bb69-d935f7f7f552
description: GetImItemsResponse 要素は、GetImItems 要求への応答を定義します。
ms.openlocfilehash: d1a4684504e8b88222615962816da3df761579c5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760754"
---
# <a name="getimitemsresponse"></a><span data-ttu-id="dfb18-103">GetImItemsResponse</span><span class="sxs-lookup"><span data-stu-id="dfb18-103">GetImItemsResponse</span></span>

<span data-ttu-id="dfb18-104">**GetImItemsResponse**要素は、 **GetImItems**要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="dfb18-104">The **GetImItemsResponse** element defines a response to a **GetImItems** request.</span></span> 
  
```XML
<GetImItemsResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ImItemList/>
</GetImItemsResponse>
```

 <span data-ttu-id="dfb18-105">**GetImItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="dfb18-105">**GetImItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dfb18-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="dfb18-106">Attributes and elements</span></span>

<span data-ttu-id="dfb18-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dfb18-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dfb18-108">属性</span><span class="sxs-lookup"><span data-stu-id="dfb18-108">Attributes</span></span>

<span data-ttu-id="dfb18-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dfb18-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dfb18-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dfb18-110">Child elements</span></span>

<span data-ttu-id="dfb18-111">[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [ImItemList](imitemlist.md)</span><span class="sxs-lookup"><span data-stu-id="dfb18-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [ImItemList](imitemlist.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dfb18-112">親要素</span><span class="sxs-lookup"><span data-stu-id="dfb18-112">Parent elements</span></span>

<span data-ttu-id="dfb18-113">なし。</span><span class="sxs-lookup"><span data-stu-id="dfb18-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dfb18-114">備考</span><span class="sxs-lookup"><span data-stu-id="dfb18-114">Remarks</span></span>

<span data-ttu-id="dfb18-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="dfb18-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="dfb18-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="dfb18-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dfb18-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="dfb18-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dfb18-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="dfb18-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dfb18-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dfb18-119">Schema name</span></span>  <br/> |<span data-ttu-id="dfb18-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="dfb18-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dfb18-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dfb18-121">Validation file</span></span>  <br/> |<span data-ttu-id="dfb18-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dfb18-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dfb18-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="dfb18-123">Can be empty</span></span>  <br/> ||
   

