---
title: GetUserPhotoResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54d43fe6-9f7b-4f84-920a-bd686c65b059
description: GetUserPhotoResponseMessage 要素には、GetUserPhoto 要求への応答が含まれています。
ms.openlocfilehash: fa817b59527f616afed84d8548e3a18e6c971e2d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831696"
---
# <a name="getuserphotoresponsemessage"></a><span data-ttu-id="9f6fc-103">GetUserPhotoResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9f6fc-103">GetUserPhotoResponseMessage</span></span>

<span data-ttu-id="9f6fc-104">**GetUserPhotoResponseMessage**要素には、GetUserPhoto 要求への応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9f6fc-104">The **GetUserPhotoResponseMessage** element contains the response to a GetUserPhoto request.</span></span> 
  
```XML
<GetUserPhotoResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <HasChanged/>
   <PictureData/>
</GetUserPhotoResponseMessage>
```

 <span data-ttu-id="9f6fc-105">**GetUserPhotoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="9f6fc-105">**GetUserPhotoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9f6fc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9f6fc-106">Attributes and elements</span></span>

<span data-ttu-id="9f6fc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9f6fc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f6fc-108">属性</span><span class="sxs-lookup"><span data-stu-id="9f6fc-108">Attributes</span></span>

<span data-ttu-id="9f6fc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9f6fc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9f6fc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9f6fc-110">Child elements</span></span>

<span data-ttu-id="9f6fc-111">[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [HasChanged](haschanged.md) | [PictureData](picturedata.md)</span><span class="sxs-lookup"><span data-stu-id="9f6fc-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [HasChanged](haschanged.md) | [PictureData](picturedata.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9f6fc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9f6fc-112">Parent elements</span></span>

[<span data-ttu-id="9f6fc-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9f6fc-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="9f6fc-114">備考</span><span class="sxs-lookup"><span data-stu-id="9f6fc-114">Remarks</span></span>

<span data-ttu-id="9f6fc-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9f6fc-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9f6fc-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9f6fc-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f6fc-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="9f6fc-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f6fc-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="9f6fc-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9f6fc-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9f6fc-119">Schema name</span></span>  <br/> |<span data-ttu-id="9f6fc-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="9f6fc-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9f6fc-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9f6fc-121">Validation file</span></span>  <br/> |<span data-ttu-id="9f6fc-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9f6fc-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9f6fc-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9f6fc-123">Can be empty</span></span>  <br/> ||
   

