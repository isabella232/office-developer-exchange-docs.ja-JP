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
description: CreateManagedFolderResponse 要素は、CreateManagedFolder 要求への応答を定義します。
ms.openlocfilehash: fc486a197b7b0a0ed7310dda88d4bf8735f99876
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759852"
---
# <a name="createmanagedfolderresponse"></a><span data-ttu-id="ffc32-103">CreateManagedFolderResponse</span><span class="sxs-lookup"><span data-stu-id="ffc32-103">CreateManagedFolderResponse</span></span>

<span data-ttu-id="ffc32-104">**CreateManagedFolderResponse**要素は、CreateManagedFolder 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="ffc32-104">The **CreateManagedFolderResponse** element defines a response to a CreateManagedFolder request.</span></span> 
  
```xml
<CreateManagedFolderResponse>
   <ResponseMessages/>
</CreateManagedFolderResponse>
```

 <span data-ttu-id="ffc32-105">**CreateManagedFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="ffc32-105">**CreateManagedFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ffc32-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ffc32-106">Attributes and elements</span></span>

<span data-ttu-id="ffc32-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ffc32-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ffc32-108">属性</span><span class="sxs-lookup"><span data-stu-id="ffc32-108">Attributes</span></span>

<span data-ttu-id="ffc32-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ffc32-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ffc32-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ffc32-110">Child elements</span></span>

|<span data-ttu-id="ffc32-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="ffc32-111">**Element**</span></span>|<span data-ttu-id="ffc32-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ffc32-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ffc32-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ffc32-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="ffc32-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ffc32-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ffc32-115">親要素</span><span class="sxs-lookup"><span data-stu-id="ffc32-115">Parent elements</span></span>

<span data-ttu-id="ffc32-116">なし。</span><span class="sxs-lookup"><span data-stu-id="ffc32-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ffc32-117">備考</span><span class="sxs-lookup"><span data-stu-id="ffc32-117">Remarks</span></span>

<span data-ttu-id="ffc32-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="ffc32-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ffc32-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="ffc32-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ffc32-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="ffc32-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ffc32-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ffc32-121">Schema name</span></span>  <br/> |<span data-ttu-id="ffc32-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="ffc32-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ffc32-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ffc32-123">Validation file</span></span>  <br/> |<span data-ttu-id="ffc32-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ffc32-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ffc32-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ffc32-125">Can be empty</span></span>  <br/> |<span data-ttu-id="ffc32-126">False</span><span class="sxs-lookup"><span data-stu-id="ffc32-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ffc32-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="ffc32-127">See also</span></span>



[<span data-ttu-id="ffc32-128">CreateManagedFolder 操作</span><span class="sxs-lookup"><span data-stu-id="ffc32-128">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)
  
[<span data-ttu-id="ffc32-129">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="ffc32-129">CreateManagedFolder</span></span>](createmanagedfolder.md)


- [<span data-ttu-id="ffc32-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ffc32-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

