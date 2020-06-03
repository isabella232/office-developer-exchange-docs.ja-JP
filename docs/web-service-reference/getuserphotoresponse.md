---
title: GetUserPhotoResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 29b085e8-95c0-4ba6-83e8-40de36a75be3
description: GetUserPhotoResponse 要素には、GetUserPhoto 要求への応答が含まれています。
ms.openlocfilehash: c0dfb6979ade0192b376c3f7115fef78a4cc7e06
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463308"
---
# <a name="getuserphotoresponse"></a><span data-ttu-id="75204-103">GetUserPhotoResponse</span><span class="sxs-lookup"><span data-stu-id="75204-103">GetUserPhotoResponse</span></span>

<span data-ttu-id="75204-104">**GetUserPhotoResponse**要素には、getuserphoto 要求への応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="75204-104">The **GetUserPhotoResponse** element contains the response to a GetUserPhoto request.</span></span> 
  
```XML
<GetUserPhotoResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <HasChanged/>
   <PictureData/>
</GetUserPhotoResponse>
```

 <span data-ttu-id="75204-105">**GetUserPhotoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="75204-105">**GetUserPhotoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="75204-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="75204-106">Attributes and elements</span></span>

<span data-ttu-id="75204-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="75204-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="75204-108">属性</span><span class="sxs-lookup"><span data-stu-id="75204-108">Attributes</span></span>

<span data-ttu-id="75204-109">なし。</span><span class="sxs-lookup"><span data-stu-id="75204-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="75204-110">子要素</span><span class="sxs-lookup"><span data-stu-id="75204-110">Child elements</span></span>

<span data-ttu-id="75204-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)  | [Haschanged](haschanged.md)  | [PictureData](picturedata.md)</span><span class="sxs-lookup"><span data-stu-id="75204-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [HasChanged](haschanged.md) | [PictureData](picturedata.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="75204-112">親要素</span><span class="sxs-lookup"><span data-stu-id="75204-112">Parent elements</span></span>

<span data-ttu-id="75204-113">なし。</span><span class="sxs-lookup"><span data-stu-id="75204-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="75204-114">注釈</span><span class="sxs-lookup"><span data-stu-id="75204-114">Remarks</span></span>

<span data-ttu-id="75204-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="75204-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="75204-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="75204-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="75204-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="75204-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="75204-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="75204-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="75204-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="75204-119">Schema name</span></span>  <br/> |<span data-ttu-id="75204-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="75204-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="75204-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="75204-121">Validation file</span></span>  <br/> |<span data-ttu-id="75204-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="75204-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="75204-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="75204-123">Can be empty</span></span>  <br/> ||
   

