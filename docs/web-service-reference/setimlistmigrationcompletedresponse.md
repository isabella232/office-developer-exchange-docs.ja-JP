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
ms.openlocfilehash: 66d85362319df1c88064130e99bba98f21b50db7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464820"
---
# <a name="setimlistmigrationcompletedresponse"></a><span data-ttu-id="c98fa-103">SetImListMigrationCompletedResponse</span><span class="sxs-lookup"><span data-stu-id="c98fa-103">SetImListMigrationCompletedResponse</span></span>

<span data-ttu-id="c98fa-104">**SetImListMigrationCompletedResponse**要素は、 **SetImListMigrationCompleted**要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="c98fa-104">The **SetImListMigrationCompletedResponse** element represents a response to a **SetImListMigrationCompleted** request.</span></span> 
  
```XML
<SetImListMigrationCompletedResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</SetImListMigrationCompletedResponse>
```

 <span data-ttu-id="c98fa-105">**SetImListMigrationCompletedResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="c98fa-105">**SetImListMigrationCompletedResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c98fa-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c98fa-106">Attributes and elements</span></span>

<span data-ttu-id="c98fa-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c98fa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c98fa-108">属性</span><span class="sxs-lookup"><span data-stu-id="c98fa-108">Attributes</span></span>

<span data-ttu-id="c98fa-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c98fa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c98fa-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c98fa-110">Child elements</span></span>

<span data-ttu-id="c98fa-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)</span><span class="sxs-lookup"><span data-stu-id="c98fa-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c98fa-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c98fa-112">Parent elements</span></span>

<span data-ttu-id="c98fa-113">なし。</span><span class="sxs-lookup"><span data-stu-id="c98fa-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c98fa-114">注釈</span><span class="sxs-lookup"><span data-stu-id="c98fa-114">Remarks</span></span>

<span data-ttu-id="c98fa-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c98fa-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c98fa-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c98fa-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c98fa-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c98fa-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c98fa-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="c98fa-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c98fa-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c98fa-119">Schema name</span></span>  <br/> |<span data-ttu-id="c98fa-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="c98fa-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c98fa-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c98fa-121">Validation file</span></span>  <br/> |<span data-ttu-id="c98fa-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="c98fa-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c98fa-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c98fa-123">Can be empty</span></span>  <br/> |<span data-ttu-id="c98fa-124">false</span><span class="sxs-lookup"><span data-stu-id="c98fa-124">false</span></span>  <br/> |
   

