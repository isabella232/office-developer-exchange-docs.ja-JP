---
title: SetImListMigrationCompletedResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7e9ab484-7100-422d-ab22-d8ddb97098c1
description: SetImListMigrationCompletedResponse 要素は、SetImListMigrationCompleted 要求への応答を表します。
ms.openlocfilehash: 2041a0e6b03305644c498ec36967f297f999d993
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833430"
---
# <a name="setimlistmigrationcompletedresponse"></a><span data-ttu-id="3a000-103">SetImListMigrationCompletedResponse</span><span class="sxs-lookup"><span data-stu-id="3a000-103">SetImListMigrationCompletedResponse</span></span>

<span data-ttu-id="3a000-104">**SetImListMigrationCompletedResponse**要素は、 **SetImListMigrationCompleted**要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="3a000-104">The **SetImListMigrationCompletedResponse** element represents a response to a **SetImListMigrationCompleted** request.</span></span> 
  
```XML
<SetImListMigrationCompletedResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</SetImListMigrationCompletedResponse>
```

 <span data-ttu-id="3a000-105">**SetImListMigrationCompletedResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3a000-105">**SetImListMigrationCompletedResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a000-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3a000-106">Attributes and elements</span></span>

<span data-ttu-id="3a000-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3a000-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a000-108">属性</span><span class="sxs-lookup"><span data-stu-id="3a000-108">Attributes</span></span>

<span data-ttu-id="3a000-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3a000-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a000-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3a000-110">Child elements</span></span>

<span data-ttu-id="3a000-111">[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md)</span><span class="sxs-lookup"><span data-stu-id="3a000-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3a000-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3a000-112">Parent elements</span></span>

<span data-ttu-id="3a000-113">なし。</span><span class="sxs-lookup"><span data-stu-id="3a000-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3a000-114">備考</span><span class="sxs-lookup"><span data-stu-id="3a000-114">Remarks</span></span>

<span data-ttu-id="3a000-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3a000-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3a000-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3a000-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3a000-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="3a000-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a000-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="3a000-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3a000-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3a000-119">Schema name</span></span>  <br/> |<span data-ttu-id="3a000-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="3a000-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3a000-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3a000-121">Validation file</span></span>  <br/> |<span data-ttu-id="3a000-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3a000-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3a000-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3a000-123">Can be empty</span></span>  <br/> |<span data-ttu-id="3a000-124">false</span><span class="sxs-lookup"><span data-stu-id="3a000-124">false</span></span>  <br/> |
   

