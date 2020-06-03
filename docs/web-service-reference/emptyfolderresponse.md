---
title: EmptyFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c900be49-3c90-41aa-aba5-bcf1116ec2aa
description: EmptyFolderResponse 要素は、EmptyFolder 操作要求への応答を定義します。
ms.openlocfilehash: 9b20df8c0b095870185aab14dbd1f7ff4fc47def
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530678"
---
# <a name="emptyfolderresponse"></a><span data-ttu-id="a3b9f-103">EmptyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="a3b9f-103">EmptyFolderResponse</span></span>

<span data-ttu-id="a3b9f-104">**Emptyfolderresponse**要素は、 [emptyfolder 操作](emptyfolder-operation.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="a3b9f-104">The **EmptyFolderResponse** element defines a response to an [EmptyFolder operation](emptyfolder-operation.md) request.</span></span> 
  
```XML
<EmptyFolderResponse>
   <ResponseMessages/>
</EmptyFolderResponse>
```

 <span data-ttu-id="a3b9f-105">**EmptyFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="a3b9f-105">**EmptyFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a3b9f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a3b9f-106">Attributes and elements</span></span>

<span data-ttu-id="a3b9f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a3b9f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a3b9f-108">属性</span><span class="sxs-lookup"><span data-stu-id="a3b9f-108">Attributes</span></span>

<span data-ttu-id="a3b9f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a3b9f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a3b9f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a3b9f-110">Child elements</span></span>

|<span data-ttu-id="a3b9f-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="a3b9f-111">**Element**</span></span>|<span data-ttu-id="a3b9f-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a3b9f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3b9f-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a3b9f-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="a3b9f-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="a3b9f-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a3b9f-115">親要素</span><span class="sxs-lookup"><span data-stu-id="a3b9f-115">Parent elements</span></span>

<span data-ttu-id="a3b9f-116">なし。</span><span class="sxs-lookup"><span data-stu-id="a3b9f-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a3b9f-117">注釈</span><span class="sxs-lookup"><span data-stu-id="a3b9f-117">Remarks</span></span>

<span data-ttu-id="a3b9f-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a3b9f-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a3b9f-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a3b9f-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a3b9f-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="a3b9f-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a3b9f-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a3b9f-121">Schema name</span></span>  <br/> |<span data-ttu-id="a3b9f-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="a3b9f-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a3b9f-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a3b9f-123">Validation file</span></span>  <br/> |<span data-ttu-id="a3b9f-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="a3b9f-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a3b9f-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a3b9f-125">Can be empty</span></span>  <br/> |<span data-ttu-id="a3b9f-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="a3b9f-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a3b9f-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="a3b9f-127">See also</span></span>



[<span data-ttu-id="a3b9f-128">EmptyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="a3b9f-128">EmptyFolder operation</span></span>](emptyfolder-operation.md)
  
[<span data-ttu-id="a3b9f-129">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="a3b9f-129">EmptyFolder</span></span>](emptyfolder.md)


- [<span data-ttu-id="a3b9f-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a3b9f-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

