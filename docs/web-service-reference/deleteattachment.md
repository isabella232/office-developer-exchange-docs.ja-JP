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
description: DeleteAttachment 要素は、Exchange ストアからの添付ファイルを削除する要求のルート要素です。
ms.openlocfilehash: 2beedd647febf025f6e3140ec37b196c9aeb7611
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759960"
---
# <a name="deleteattachment"></a><span data-ttu-id="89ac8-103">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="89ac8-103">DeleteAttachment</span></span>

<span data-ttu-id="89ac8-104">**DeleteAttachment**要素は、Exchange ストアからの添付ファイルを削除する要求のルート要素です。</span><span class="sxs-lookup"><span data-stu-id="89ac8-104">The **DeleteAttachment** element is the root element in a request to delete an attachment from the Exchange store.</span></span> 
  
```xml
<DeleteAttachment>
   <AttachmentIds/>
</DeleteAttachment>
```

<span data-ttu-id="89ac8-105">**DeleteAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="89ac8-105">**DeleteAttachmentType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="89ac8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="89ac8-106">Attributes and elements</span></span>

<span data-ttu-id="89ac8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="89ac8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89ac8-108">属性</span><span class="sxs-lookup"><span data-stu-id="89ac8-108">Attributes</span></span>

<span data-ttu-id="89ac8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="89ac8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="89ac8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="89ac8-110">Child elements</span></span>

|<span data-ttu-id="89ac8-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="89ac8-111">**Element**</span></span>|<span data-ttu-id="89ac8-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="89ac8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89ac8-113">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="89ac8-113">AttachmentIds</span></span>](attachmentids.md) <br/> |<span data-ttu-id="89ac8-114">添付ファイルを削除するのには使用されている添付ファイルの識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="89ac8-114">Contains an array of attachment identifiers that are used to delete the attachments.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="89ac8-115">親要素</span><span class="sxs-lookup"><span data-stu-id="89ac8-115">Parent elements</span></span>

<span data-ttu-id="89ac8-116">なし。</span><span class="sxs-lookup"><span data-stu-id="89ac8-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="89ac8-117">備考</span><span class="sxs-lookup"><span data-stu-id="89ac8-117">Remarks</span></span>

<span data-ttu-id="89ac8-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="89ac8-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89ac8-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="89ac8-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89ac8-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="89ac8-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="89ac8-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="89ac8-121">Schema Name</span></span>  <br/> |<span data-ttu-id="89ac8-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="89ac8-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="89ac8-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="89ac8-123">Validation File</span></span>  <br/> |<span data-ttu-id="89ac8-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="89ac8-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="89ac8-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="89ac8-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="89ac8-126">False</span><span class="sxs-lookup"><span data-stu-id="89ac8-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="89ac8-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="89ac8-127">See also</span></span>

- [<span data-ttu-id="89ac8-128">DeleteAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="89ac8-128">DeleteAttachment operation</span></span>](deleteattachment-operation.md)

