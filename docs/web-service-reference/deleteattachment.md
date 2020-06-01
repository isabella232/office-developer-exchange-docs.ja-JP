---
title: DeleteAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteAttachment
api_type:
- schema
ms.assetid: 43d0c1cb-92ca-4399-9b3a-acb2b5c22624
description: DeleteAttachment 要素は、Exchange ストアから添付ファイルを削除する要求のルート要素です。
ms.openlocfilehash: ae8dd5abc1dced2645e579a62f1f57a66cbc9877
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457348"
---
# <a name="deleteattachment"></a><span data-ttu-id="d5fd4-103">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="d5fd4-103">DeleteAttachment</span></span>

<span data-ttu-id="d5fd4-104">**Deleteattachment**要素は、Exchange ストアから添付ファイルを削除する要求のルート要素です。</span><span class="sxs-lookup"><span data-stu-id="d5fd4-104">The **DeleteAttachment** element is the root element in a request to delete an attachment from the Exchange store.</span></span> 
  
```xml
<DeleteAttachment>
   <AttachmentIds/>
</DeleteAttachment>
```

<span data-ttu-id="d5fd4-105">**DeleteAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="d5fd4-105">**DeleteAttachmentType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d5fd4-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d5fd4-106">Attributes and elements</span></span>

<span data-ttu-id="d5fd4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d5fd4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d5fd4-108">属性</span><span class="sxs-lookup"><span data-stu-id="d5fd4-108">Attributes</span></span>

<span data-ttu-id="d5fd4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d5fd4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d5fd4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d5fd4-110">Child elements</span></span>

|<span data-ttu-id="d5fd4-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="d5fd4-111">**Element**</span></span>|<span data-ttu-id="d5fd4-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d5fd4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5fd4-113">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="d5fd4-113">AttachmentIds</span></span>](attachmentids.md) <br/> |<span data-ttu-id="d5fd4-114">添付ファイルの削除に使用される添付ファイル識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d5fd4-114">Contains an array of attachment identifiers that are used to delete the attachments.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d5fd4-115">親要素</span><span class="sxs-lookup"><span data-stu-id="d5fd4-115">Parent elements</span></span>

<span data-ttu-id="d5fd4-116">なし。</span><span class="sxs-lookup"><span data-stu-id="d5fd4-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d5fd4-117">注釈</span><span class="sxs-lookup"><span data-stu-id="d5fd4-117">Remarks</span></span>

<span data-ttu-id="d5fd4-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d5fd4-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d5fd4-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d5fd4-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d5fd4-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="d5fd4-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d5fd4-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d5fd4-121">Schema Name</span></span>  <br/> |<span data-ttu-id="d5fd4-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="d5fd4-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d5fd4-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d5fd4-123">Validation File</span></span>  <br/> |<span data-ttu-id="d5fd4-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d5fd4-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d5fd4-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d5fd4-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="d5fd4-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="d5fd4-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d5fd4-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="d5fd4-127">See also</span></span>

- [<span data-ttu-id="d5fd4-128">DeleteAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="d5fd4-128">DeleteAttachment operation</span></span>](deleteattachment-operation.md)

