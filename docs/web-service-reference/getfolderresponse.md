---
title: GetFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetFolderResponse
api_type:
- schema
ms.assetid: 47abeec8-78dd-4297-8525-099174ec880d
description: GetFolderResponse 要素は、GetFolder 要求への応答を定義します。
ms.openlocfilehash: 46cd56aa3067b010d0f3f3b5a321e1855b0520bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459175"
---
# <a name="getfolderresponse"></a><span data-ttu-id="aa15f-103">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="aa15f-103">GetFolderResponse</span></span>

<span data-ttu-id="aa15f-104">**Getfolderresponse**要素は、getfolder 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="aa15f-104">The **GetFolderResponse** element defines a response to a GetFolder request.</span></span> 
  
```xml
<GetFolderResponse>
   <ResponseMessages/>
</GetFolderResponse>
```

 <span data-ttu-id="aa15f-105">**GetFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="aa15f-105">**GetFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aa15f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="aa15f-106">Attributes and elements</span></span>

<span data-ttu-id="aa15f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="aa15f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa15f-108">属性</span><span class="sxs-lookup"><span data-stu-id="aa15f-108">Attributes</span></span>

<span data-ttu-id="aa15f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="aa15f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aa15f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="aa15f-110">Child elements</span></span>

|<span data-ttu-id="aa15f-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="aa15f-111">**Element**</span></span>|<span data-ttu-id="aa15f-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="aa15f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa15f-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="aa15f-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="aa15f-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="aa15f-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aa15f-115">親要素</span><span class="sxs-lookup"><span data-stu-id="aa15f-115">Parent elements</span></span>

<span data-ttu-id="aa15f-116">なし。</span><span class="sxs-lookup"><span data-stu-id="aa15f-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="aa15f-117">注釈</span><span class="sxs-lookup"><span data-stu-id="aa15f-117">Remarks</span></span>

<span data-ttu-id="aa15f-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="aa15f-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aa15f-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="aa15f-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aa15f-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="aa15f-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aa15f-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="aa15f-121">Schema name</span></span>  <br/> |<span data-ttu-id="aa15f-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="aa15f-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="aa15f-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="aa15f-123">Validation file</span></span>  <br/> |<span data-ttu-id="aa15f-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="aa15f-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aa15f-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="aa15f-125">Can be empty</span></span>  <br/> |<span data-ttu-id="aa15f-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="aa15f-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aa15f-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="aa15f-127">See also</span></span>



[<span data-ttu-id="aa15f-128">GetFolder</span><span class="sxs-lookup"><span data-stu-id="aa15f-128">GetFolder</span></span>](getfolder.md)
  
<span data-ttu-id="aa15f-129">
  [GetFolder 操作](getfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="aa15f-129">[GetFolder operation](getfolder-operation.md)</span></span>
  
[<span data-ttu-id="aa15f-130">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="aa15f-130">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)

