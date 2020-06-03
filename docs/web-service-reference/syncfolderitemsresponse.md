---
title: SyncFolderItemsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderItemsResponse
api_type:
- schema
ms.assetid: 82fe0644-1756-40b2-955c-20c01110660c
description: SyncFolderItemsResponse 要素は、SyncFolderItems 要求への応答を定義します。
ms.openlocfilehash: 694730a5ead8b875da9b3544099d0b20a478a627
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530233"
---
# <a name="syncfolderitemsresponse"></a><span data-ttu-id="2f99d-103">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="2f99d-103">SyncFolderItemsResponse</span></span>

<span data-ttu-id="2f99d-104">**Syncfolderitemsresponse**要素は、SyncFolderItems 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="2f99d-104">The **SyncFolderItemsResponse** element defines a response to a SyncFolderItems request.</span></span> 
  
```xml
<SyncFolderItemsResponse>
   <ResponseMessages/>
</SyncFolderItemsResponse>
```

 <span data-ttu-id="2f99d-105">**SyncFolderItemsResponseType**</span><span class="sxs-lookup"><span data-stu-id="2f99d-105">**SyncFolderItemsResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2f99d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2f99d-106">Attributes and elements</span></span>

<span data-ttu-id="2f99d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2f99d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2f99d-108">属性</span><span class="sxs-lookup"><span data-stu-id="2f99d-108">Attributes</span></span>

<span data-ttu-id="2f99d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2f99d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2f99d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2f99d-110">Child elements</span></span>

|<span data-ttu-id="2f99d-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="2f99d-111">**Element**</span></span>|<span data-ttu-id="2f99d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2f99d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2f99d-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2f99d-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="2f99d-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="2f99d-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2f99d-115">親要素</span><span class="sxs-lookup"><span data-stu-id="2f99d-115">Parent elements</span></span>

<span data-ttu-id="2f99d-116">なし。</span><span class="sxs-lookup"><span data-stu-id="2f99d-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2f99d-117">注釈</span><span class="sxs-lookup"><span data-stu-id="2f99d-117">Remarks</span></span>

<span data-ttu-id="2f99d-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2f99d-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2f99d-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2f99d-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2f99d-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="2f99d-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2f99d-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2f99d-121">Schema name</span></span>  <br/> |<span data-ttu-id="2f99d-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="2f99d-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2f99d-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2f99d-123">Validation file</span></span>  <br/> |<span data-ttu-id="2f99d-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="2f99d-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2f99d-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2f99d-125">Can be empty</span></span>  <br/> |<span data-ttu-id="2f99d-126">いいえ</span><span class="sxs-lookup"><span data-stu-id="2f99d-126">False</span></span>  <br/> |
   

