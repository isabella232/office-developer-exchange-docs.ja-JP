---
title: Getnonindexableitem、Response
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6cf2aea3-c6f7-4cad-a45d-2daffeece4b6
description: GetNonIndexableItemDetails Response 要素は、GetNonIndexableItemDetails 要求への応答を指定します。
ms.openlocfilehash: 7563a772e04f72c50ddfea0a69fa511d2a538b8e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455619"
---
# <a name="getnonindexableitemdetailsresponse"></a><span data-ttu-id="2023d-103">Getnonindexableitem、Response</span><span class="sxs-lookup"><span data-stu-id="2023d-103">GetNonIndexableItemDetailsResponse</span></span>

<span data-ttu-id="2023d-104">**Getnonindexableitemdetails response**要素は、 **getnonindexableitemdetails**要求への応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="2023d-104">The **GetNonIndexableItemDetailsResponse** element specifies the response to a **GetNonIndexableItemDetails** request.</span></span> 
  
```XML
<GetNonIndexableItemDetailsResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <NonIndexableItemDetailsResult/>
</GetNonIndexableItemDetailsResponse>
```

 <span data-ttu-id="2023d-105">**Getnonindexableitem/[Responsemessagetype]**</span><span class="sxs-lookup"><span data-stu-id="2023d-105">**GetNonIndexableItemDetailsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2023d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2023d-106">Attributes and elements</span></span>

<span data-ttu-id="2023d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2023d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2023d-108">属性</span><span class="sxs-lookup"><span data-stu-id="2023d-108">Attributes</span></span>

<span data-ttu-id="2023d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2023d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2023d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2023d-110">Child elements</span></span>

<span data-ttu-id="2023d-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)  | [Nonindexableitemの取得結果](nonindexableitemdetailsresult.md)</span><span class="sxs-lookup"><span data-stu-id="2023d-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [NonIndexableItemDetailsResult](nonindexableitemdetailsresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2023d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2023d-112">Parent elements</span></span>

[<span data-ttu-id="2023d-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2023d-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="2023d-114">注釈</span><span class="sxs-lookup"><span data-stu-id="2023d-114">Remarks</span></span>

<span data-ttu-id="2023d-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2023d-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2023d-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2023d-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2023d-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2023d-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2023d-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="2023d-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2023d-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2023d-119">Schema name</span></span>  <br/> |<span data-ttu-id="2023d-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="2023d-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2023d-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2023d-121">Validation file</span></span>  <br/> |<span data-ttu-id="2023d-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="2023d-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2023d-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2023d-123">Can be empty</span></span>  <br/> |<span data-ttu-id="2023d-124">false</span><span class="sxs-lookup"><span data-stu-id="2023d-124">false</span></span>  <br/> |
   

