---
title: UpdateFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateFolderResponse
api_type:
- schema
ms.assetid: 31f47739-dc9c-46ba-9e3f-cce25dc85e6e
description: UpdateFolderResponse 要素は、UpdateFolder 要求への応答を定義します。
ms.openlocfilehash: 85b610d649b84c14e892ea81fe74ad53b331e67f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466620"
---
# <a name="updatefolderresponse"></a><span data-ttu-id="d332b-103">UpdateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="d332b-103">UpdateFolderResponse</span></span>

<span data-ttu-id="d332b-104">**Updatefolderresponse**要素は、updatefolder 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="d332b-104">The **UpdateFolderResponse** element defines the response to an UpdateFolder request.</span></span> 
  
```xml
<UpdateFolderResponse>
   <ResponseMessages/>
</UpdateFolderResponse>
```

 <span data-ttu-id="d332b-105">**UpdateFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="d332b-105">**UpdateFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d332b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d332b-106">Attributes and elements</span></span>

<span data-ttu-id="d332b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d332b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d332b-108">属性</span><span class="sxs-lookup"><span data-stu-id="d332b-108">Attributes</span></span>

<span data-ttu-id="d332b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d332b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d332b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d332b-110">Child elements</span></span>

|<span data-ttu-id="d332b-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="d332b-111">**Element**</span></span>|<span data-ttu-id="d332b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d332b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d332b-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d332b-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d332b-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="d332b-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d332b-115">親要素</span><span class="sxs-lookup"><span data-stu-id="d332b-115">Parent elements</span></span>

<span data-ttu-id="d332b-116">なし。</span><span class="sxs-lookup"><span data-stu-id="d332b-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d332b-117">注釈</span><span class="sxs-lookup"><span data-stu-id="d332b-117">Remarks</span></span>

<span data-ttu-id="d332b-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d332b-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d332b-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d332b-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d332b-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="d332b-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d332b-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d332b-121">Schema name</span></span>  <br/> |<span data-ttu-id="d332b-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="d332b-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d332b-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d332b-123">Validation file</span></span>  <br/> |<span data-ttu-id="d332b-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d332b-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d332b-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d332b-125">Can be empty</span></span>  <br/> |<span data-ttu-id="d332b-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="d332b-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d332b-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="d332b-127">See also</span></span>



[<span data-ttu-id="d332b-128">UpdateFolder 操作</span><span class="sxs-lookup"><span data-stu-id="d332b-128">UpdateFolder operation</span></span>](updatefolder-operation.md)
  
[<span data-ttu-id="d332b-129">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="d332b-129">UpdateFolder</span></span>](updatefolder.md)


- [<span data-ttu-id="d332b-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d332b-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

