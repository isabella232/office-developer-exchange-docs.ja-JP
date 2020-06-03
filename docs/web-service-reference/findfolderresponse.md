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
ms.openlocfilehash: 365e4e81b04419ed42f0bd9c8e022b6f8e559a2a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462571"
---
# <a name="findfolderresponse"></a><span data-ttu-id="4ac8f-103">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="4ac8f-103">FindFolderResponse</span></span>

<span data-ttu-id="4ac8f-104">**Findfolderresponse**要素は、findfolder 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="4ac8f-104">The **FindFolderResponse** element defines a response to a FindFolder request.</span></span> 
  
[<span data-ttu-id="4ac8f-105">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="4ac8f-105">FindFolderResponse</span></span>](findfolderresponse.md)
  
```xml
<FindFolderResponse>
   <ResponseMessages/>
</FindFolderResponse>
```

 <span data-ttu-id="4ac8f-106">**FindFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="4ac8f-106">**FindFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ac8f-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4ac8f-107">Attributes and elements</span></span>

<span data-ttu-id="4ac8f-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4ac8f-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ac8f-109">属性</span><span class="sxs-lookup"><span data-stu-id="4ac8f-109">Attributes</span></span>

<span data-ttu-id="4ac8f-110">なし。</span><span class="sxs-lookup"><span data-stu-id="4ac8f-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ac8f-111">子要素</span><span class="sxs-lookup"><span data-stu-id="4ac8f-111">Child elements</span></span>

|<span data-ttu-id="4ac8f-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="4ac8f-112">**Element**</span></span>|<span data-ttu-id="4ac8f-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="4ac8f-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ac8f-114">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4ac8f-114">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="4ac8f-115">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="4ac8f-115">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4ac8f-116">親要素</span><span class="sxs-lookup"><span data-stu-id="4ac8f-116">Parent elements</span></span>

<span data-ttu-id="4ac8f-117">なし。</span><span class="sxs-lookup"><span data-stu-id="4ac8f-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4ac8f-118">注釈</span><span class="sxs-lookup"><span data-stu-id="4ac8f-118">Remarks</span></span>

<span data-ttu-id="4ac8f-119">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="4ac8f-119">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ac8f-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4ac8f-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ac8f-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="4ac8f-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4ac8f-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4ac8f-122">Schema name</span></span>  <br/> |<span data-ttu-id="4ac8f-123">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="4ac8f-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4ac8f-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4ac8f-124">Validation file</span></span>  <br/> |<span data-ttu-id="4ac8f-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="4ac8f-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4ac8f-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4ac8f-126">Can be empty</span></span>  <br/> |<span data-ttu-id="4ac8f-127">正しくない</span><span class="sxs-lookup"><span data-stu-id="4ac8f-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4ac8f-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="4ac8f-128">See also</span></span>



[<span data-ttu-id="4ac8f-129">FindFolder 操作</span><span class="sxs-lookup"><span data-stu-id="4ac8f-129">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="4ac8f-130">フォルダーの検索</span><span class="sxs-lookup"><span data-stu-id="4ac8f-130">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

