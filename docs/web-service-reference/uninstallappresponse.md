---
title: UninstallAppResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0e3f13cc-e3b3-4eea-9128-12c98b5197f4
description: UninstallAppResponse 要素は、UninstallApp 要求への応答を指定します。
ms.openlocfilehash: 9675b72b36fd1ac5e298b2998ed683a1ba6452f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839791"
---
# <a name="uninstallappresponse"></a><span data-ttu-id="f2799-103">UninstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="f2799-103">UninstallAppResponse</span></span>

<span data-ttu-id="f2799-104">**UninstallAppResponse**要素は、 **UninstallApp**要求への応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="f2799-104">The **UninstallAppResponse** element specifies the response to an **UninstallApp** request.</span></span> 
  
```XML
<UninstallAppResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</UninstallAppResponse>
```

 <span data-ttu-id="f2799-105">**UninstallAppResponseType**</span><span class="sxs-lookup"><span data-stu-id="f2799-105">**UninstallAppResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f2799-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f2799-106">Attributes and elements</span></span>

<span data-ttu-id="f2799-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f2799-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f2799-108">属性</span><span class="sxs-lookup"><span data-stu-id="f2799-108">Attributes</span></span>

<span data-ttu-id="f2799-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f2799-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f2799-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f2799-110">Child elements</span></span>

<span data-ttu-id="f2799-111">[MessageXml](messagexml.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md)</span><span class="sxs-lookup"><span data-stu-id="f2799-111">[MessageXml](messagexml.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f2799-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f2799-112">Parent elements</span></span>

<span data-ttu-id="f2799-113">なし。</span><span class="sxs-lookup"><span data-stu-id="f2799-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f2799-114">備考</span><span class="sxs-lookup"><span data-stu-id="f2799-114">Remarks</span></span>

<span data-ttu-id="f2799-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f2799-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f2799-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f2799-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f2799-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="f2799-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f2799-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="f2799-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f2799-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f2799-119">Schema name</span></span>  <br/> |<span data-ttu-id="f2799-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="f2799-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f2799-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f2799-121">Validation file</span></span>  <br/> |<span data-ttu-id="f2799-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f2799-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f2799-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f2799-123">Can be empty</span></span>  <br/> ||
   

