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
ms.openlocfilehash: a2eb9be41b079d29c64f50bcc9e7151ad424de2c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831697"
---
# <a name="getuserphotoresponse"></a><span data-ttu-id="2ae74-103">GetUserPhotoResponse</span><span class="sxs-lookup"><span data-stu-id="2ae74-103">GetUserPhotoResponse</span></span>

<span data-ttu-id="2ae74-104">**GetUserPhotoResponse**要素には、GetUserPhoto 要求への応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2ae74-104">The **GetUserPhotoResponse** element contains the response to a GetUserPhoto request.</span></span> 
  
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

 <span data-ttu-id="2ae74-105">**GetUserPhotoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="2ae74-105">**GetUserPhotoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2ae74-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2ae74-106">Attributes and elements</span></span>

<span data-ttu-id="2ae74-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2ae74-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ae74-108">属性</span><span class="sxs-lookup"><span data-stu-id="2ae74-108">Attributes</span></span>

<span data-ttu-id="2ae74-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2ae74-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2ae74-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2ae74-110">Child elements</span></span>

<span data-ttu-id="2ae74-111">[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [HasChanged](haschanged.md) | [PictureData](picturedata.md)</span><span class="sxs-lookup"><span data-stu-id="2ae74-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [HasChanged](haschanged.md) | [PictureData](picturedata.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2ae74-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2ae74-112">Parent elements</span></span>

<span data-ttu-id="2ae74-113">なし。</span><span class="sxs-lookup"><span data-stu-id="2ae74-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2ae74-114">備考</span><span class="sxs-lookup"><span data-stu-id="2ae74-114">Remarks</span></span>

<span data-ttu-id="2ae74-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2ae74-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2ae74-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2ae74-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2ae74-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="2ae74-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ae74-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="2ae74-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2ae74-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2ae74-119">Schema name</span></span>  <br/> |<span data-ttu-id="2ae74-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="2ae74-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2ae74-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2ae74-121">Validation file</span></span>  <br/> |<span data-ttu-id="2ae74-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2ae74-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2ae74-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2ae74-123">Can be empty</span></span>  <br/> ||
   

