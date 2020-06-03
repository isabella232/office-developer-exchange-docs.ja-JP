---
title: UninstallAppResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0e3f13cc-e3b3-4eea-9128-12c98b5197f4
description: UninstallAppResponse 要素は、アン Installapp 要求への応答を指定します。
ms.openlocfilehash: 12d74669aed0c380e32dd568bb99b88c30fdb22d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459455"
---
# <a name="uninstallappresponse"></a><span data-ttu-id="bb884-103">UninstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="bb884-103">UninstallAppResponse</span></span>

<span data-ttu-id="bb884-104">**UninstallAppResponse**要素は、**アン installapp**要求への応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="bb884-104">The **UninstallAppResponse** element specifies the response to an **UninstallApp** request.</span></span> 
  
```XML
<UninstallAppResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</UninstallAppResponse>
```

 <span data-ttu-id="bb884-105">**UninstallAppResponseType**</span><span class="sxs-lookup"><span data-stu-id="bb884-105">**UninstallAppResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bb884-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="bb884-106">Attributes and elements</span></span>

<span data-ttu-id="bb884-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bb884-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bb884-108">属性</span><span class="sxs-lookup"><span data-stu-id="bb884-108">Attributes</span></span>

<span data-ttu-id="bb884-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bb884-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bb884-110">子要素</span><span class="sxs-lookup"><span data-stu-id="bb884-110">Child elements</span></span>

<span data-ttu-id="bb884-111">[MessageXml](messagexml.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)</span><span class="sxs-lookup"><span data-stu-id="bb884-111">[MessageXml](messagexml.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bb884-112">親要素</span><span class="sxs-lookup"><span data-stu-id="bb884-112">Parent elements</span></span>

<span data-ttu-id="bb884-113">なし。</span><span class="sxs-lookup"><span data-stu-id="bb884-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bb884-114">注釈</span><span class="sxs-lookup"><span data-stu-id="bb884-114">Remarks</span></span>

<span data-ttu-id="bb884-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="bb884-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bb884-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="bb884-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bb884-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="bb884-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bb884-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="bb884-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bb884-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bb884-119">Schema name</span></span>  <br/> |<span data-ttu-id="bb884-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="bb884-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bb884-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bb884-121">Validation file</span></span>  <br/> |<span data-ttu-id="bb884-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="bb884-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bb884-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="bb884-123">Can be empty</span></span>  <br/> ||
   

