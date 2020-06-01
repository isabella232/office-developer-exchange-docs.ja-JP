---
title: CreateManagedFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolderResponse
api_type:
- schema
ms.assetid: 99062401-d356-4ce7-a5d0-c8c7aab99912
description: CreateManagedFolderResponse 要素は、CreateManagedFolder 要求に対する応答を定義します。
ms.openlocfilehash: a1983545f3279baeb4ec6a7a1ae56ee3501a1d82
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458354"
---
# <a name="createmanagedfolderresponse"></a><span data-ttu-id="3c835-103">CreateManagedFolderResponse</span><span class="sxs-lookup"><span data-stu-id="3c835-103">CreateManagedFolderResponse</span></span>

<span data-ttu-id="3c835-104">**CreateManagedFolderResponse**要素は、CreateManagedFolder 要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="3c835-104">The **CreateManagedFolderResponse** element defines a response to a CreateManagedFolder request.</span></span> 
  
```xml
<CreateManagedFolderResponse>
   <ResponseMessages/>
</CreateManagedFolderResponse>
```

 <span data-ttu-id="3c835-105">**CreateManagedFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="3c835-105">**CreateManagedFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3c835-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3c835-106">Attributes and elements</span></span>

<span data-ttu-id="3c835-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3c835-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3c835-108">属性</span><span class="sxs-lookup"><span data-stu-id="3c835-108">Attributes</span></span>

<span data-ttu-id="3c835-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3c835-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3c835-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3c835-110">Child elements</span></span>

|<span data-ttu-id="3c835-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="3c835-111">**Element**</span></span>|<span data-ttu-id="3c835-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3c835-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c835-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="3c835-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="3c835-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="3c835-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3c835-115">親要素</span><span class="sxs-lookup"><span data-stu-id="3c835-115">Parent elements</span></span>

<span data-ttu-id="3c835-116">なし。</span><span class="sxs-lookup"><span data-stu-id="3c835-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3c835-117">注釈</span><span class="sxs-lookup"><span data-stu-id="3c835-117">Remarks</span></span>

<span data-ttu-id="3c835-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="3c835-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3c835-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3c835-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3c835-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="3c835-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3c835-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3c835-121">Schema name</span></span>  <br/> |<span data-ttu-id="3c835-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="3c835-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3c835-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3c835-123">Validation file</span></span>  <br/> |<span data-ttu-id="3c835-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="3c835-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3c835-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3c835-125">Can be empty</span></span>  <br/> |<span data-ttu-id="3c835-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="3c835-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3c835-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="3c835-127">See also</span></span>



[<span data-ttu-id="3c835-128">CreateManagedFolder 操作</span><span class="sxs-lookup"><span data-stu-id="3c835-128">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)
  
[<span data-ttu-id="3c835-129">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="3c835-129">CreateManagedFolder</span></span>](createmanagedfolder.md)


- [<span data-ttu-id="3c835-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="3c835-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

