---
title: CopyFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolderResponse
api_type:
- schema
ms.assetid: 5bfbb4d3-e2ed-4b84-96f7-2175f1947aed
description: CopyFolderResponse 要素は、CopyFolder 要求への応答を定義します。
ms.openlocfilehash: aaf5d2bde8c9ba6b0c8aa6345af39dd9a6006ae5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458517"
---
# <a name="copyfolderresponse"></a><span data-ttu-id="90f83-103">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="90f83-103">CopyFolderResponse</span></span>

<span data-ttu-id="90f83-104">**Copyfolderresponse**要素は、copyfolder 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="90f83-104">The **CopyFolderResponse** element defines a response to a CopyFolder request.</span></span> 
  
```xml
<CopyFolderResponse>
   <ResponseMessages/>
</CopyFolderResponse>
```

 <span data-ttu-id="90f83-105">**CopyFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="90f83-105">**CopyFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="90f83-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="90f83-106">Attributes and elements</span></span>

<span data-ttu-id="90f83-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="90f83-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90f83-108">属性</span><span class="sxs-lookup"><span data-stu-id="90f83-108">Attributes</span></span>

<span data-ttu-id="90f83-109">なし。</span><span class="sxs-lookup"><span data-stu-id="90f83-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="90f83-110">子要素</span><span class="sxs-lookup"><span data-stu-id="90f83-110">Child elements</span></span>

|<span data-ttu-id="90f83-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="90f83-111">**Element**</span></span>|<span data-ttu-id="90f83-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="90f83-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90f83-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="90f83-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="90f83-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="90f83-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="90f83-115">親要素</span><span class="sxs-lookup"><span data-stu-id="90f83-115">Parent elements</span></span>

<span data-ttu-id="90f83-116">なし。</span><span class="sxs-lookup"><span data-stu-id="90f83-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="90f83-117">注釈</span><span class="sxs-lookup"><span data-stu-id="90f83-117">Remarks</span></span>

<span data-ttu-id="90f83-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="90f83-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="90f83-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="90f83-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="90f83-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="90f83-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="90f83-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="90f83-121">Schema name</span></span>  <br/> |<span data-ttu-id="90f83-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="90f83-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="90f83-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="90f83-123">Validation file</span></span>  <br/> |<span data-ttu-id="90f83-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="90f83-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="90f83-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="90f83-125">Can be empty</span></span>  <br/> |<span data-ttu-id="90f83-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="90f83-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="90f83-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="90f83-127">See also</span></span>



[<span data-ttu-id="90f83-128">CopyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="90f83-128">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="90f83-129">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="90f83-129">CopyFolder</span></span>](copyfolder.md)


- [<span data-ttu-id="90f83-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="90f83-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

