---
title: CreateFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateFolderResponse
api_type:
- schema
ms.assetid: 158adecc-491a-47d9-af73-acc2cd3f8566
description: CreateFolderResponse 要素は、CreateFolder 要求への応答を定義します。
ms.openlocfilehash: b584b2bb5514e411d9327c2c9effca4c3feb9b83
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759818"
---
# <a name="createfolderresponse"></a><span data-ttu-id="9f14f-103">CreateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="9f14f-103">CreateFolderResponse</span></span>

<span data-ttu-id="9f14f-104">**CreateFolderResponse**要素は、CreateFolder 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="9f14f-104">The **CreateFolderResponse** element defines a response to a CreateFolder request.</span></span> 
  
```xml
<CreateFolderResponse>
   <ResponseMessages/>
</CreateFolderResponse>
```

 <span data-ttu-id="9f14f-105">**CreateFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="9f14f-105">**CreateFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9f14f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9f14f-106">Attributes and elements</span></span>

<span data-ttu-id="9f14f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9f14f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f14f-108">属性</span><span class="sxs-lookup"><span data-stu-id="9f14f-108">Attributes</span></span>

<span data-ttu-id="9f14f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9f14f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9f14f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9f14f-110">Child elements</span></span>

|<span data-ttu-id="9f14f-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="9f14f-111">**Element**</span></span>|<span data-ttu-id="9f14f-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9f14f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f14f-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9f14f-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="9f14f-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9f14f-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9f14f-115">親要素</span><span class="sxs-lookup"><span data-stu-id="9f14f-115">Parent elements</span></span>

<span data-ttu-id="9f14f-116">なし。</span><span class="sxs-lookup"><span data-stu-id="9f14f-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9f14f-117">備考</span><span class="sxs-lookup"><span data-stu-id="9f14f-117">Remarks</span></span>

<span data-ttu-id="9f14f-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="9f14f-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f14f-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="9f14f-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f14f-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="9f14f-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9f14f-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9f14f-121">Schema name</span></span>  <br/> |<span data-ttu-id="9f14f-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="9f14f-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9f14f-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9f14f-123">Validation file</span></span>  <br/> |<span data-ttu-id="9f14f-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9f14f-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9f14f-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9f14f-125">Can be empty</span></span>  <br/> |<span data-ttu-id="9f14f-126">False</span><span class="sxs-lookup"><span data-stu-id="9f14f-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9f14f-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="9f14f-127">See also</span></span>



<span data-ttu-id="9f14f-128">
  [CreateFolder 操作](createfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="9f14f-128">[CreateFolder operation](createfolder-operation.md)</span></span>
  
[<span data-ttu-id="9f14f-129">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="9f14f-129">CreateFolder</span></span>](createfolder.md)


- [<span data-ttu-id="9f14f-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9f14f-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

