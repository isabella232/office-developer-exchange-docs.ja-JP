---
title: FindFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindFolderResponse
api_type:
- schema
ms.assetid: f5dd813c-9698-4a39-8fca-3a825df365ed
description: FindFolderResponse 要素は、FindFolder 要求への応答を定義します。
ms.openlocfilehash: 3bf0509acd5a3928eb29015c39c18bb779c1dfce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760498"
---
# <a name="findfolderresponse"></a><span data-ttu-id="6c94a-103">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="6c94a-103">FindFolderResponse</span></span>

<span data-ttu-id="6c94a-104">**FindFolderResponse**要素は、FindFolder 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="6c94a-104">The **FindFolderResponse** element defines a response to a FindFolder request.</span></span> 
  
[<span data-ttu-id="6c94a-105">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="6c94a-105">FindFolderResponse</span></span>](findfolderresponse.md)
  
```xml
<FindFolderResponse>
   <ResponseMessages/>
</FindFolderResponse>
```

 <span data-ttu-id="6c94a-106">**FindFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="6c94a-106">**FindFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6c94a-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6c94a-107">Attributes and elements</span></span>

<span data-ttu-id="6c94a-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6c94a-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6c94a-109">属性</span><span class="sxs-lookup"><span data-stu-id="6c94a-109">Attributes</span></span>

<span data-ttu-id="6c94a-110">なし。</span><span class="sxs-lookup"><span data-stu-id="6c94a-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6c94a-111">子要素</span><span class="sxs-lookup"><span data-stu-id="6c94a-111">Child elements</span></span>

|<span data-ttu-id="6c94a-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="6c94a-112">**Element**</span></span>|<span data-ttu-id="6c94a-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="6c94a-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c94a-114">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="6c94a-114">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="6c94a-115">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6c94a-115">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6c94a-116">親要素</span><span class="sxs-lookup"><span data-stu-id="6c94a-116">Parent elements</span></span>

<span data-ttu-id="6c94a-117">なし。</span><span class="sxs-lookup"><span data-stu-id="6c94a-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6c94a-118">備考</span><span class="sxs-lookup"><span data-stu-id="6c94a-118">Remarks</span></span>

<span data-ttu-id="6c94a-119">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="6c94a-119">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6c94a-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="6c94a-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6c94a-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="6c94a-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6c94a-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6c94a-122">Schema name</span></span>  <br/> |<span data-ttu-id="6c94a-123">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="6c94a-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6c94a-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6c94a-124">Validation file</span></span>  <br/> |<span data-ttu-id="6c94a-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6c94a-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6c94a-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6c94a-126">Can be empty</span></span>  <br/> |<span data-ttu-id="6c94a-127">False</span><span class="sxs-lookup"><span data-stu-id="6c94a-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6c94a-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="6c94a-128">See also</span></span>



<span data-ttu-id="6c94a-129">
  [FindFolder 操作](findfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="6c94a-129">[FindFolder operation](findfolder-operation.md)</span></span>


[<span data-ttu-id="6c94a-130">フォルダーを検索します。</span><span class="sxs-lookup"><span data-stu-id="6c94a-130">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

