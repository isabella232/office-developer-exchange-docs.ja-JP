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
ms.openlocfilehash: a6df1204d4ac3a976694afbca008852acef6a76e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463301"
---
# <a name="getuserphotoresponsemessage"></a><span data-ttu-id="408a9-103">GetUserPhotoResponseMessage</span><span class="sxs-lookup"><span data-stu-id="408a9-103">GetUserPhotoResponseMessage</span></span>

<span data-ttu-id="408a9-104">**GetUserPhotoResponseMessage**要素には、getuserphoto 要求への応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="408a9-104">The **GetUserPhotoResponseMessage** element contains the response to a GetUserPhoto request.</span></span> 
  
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

 <span data-ttu-id="408a9-105">**GetUserPhotoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="408a9-105">**GetUserPhotoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="408a9-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="408a9-106">Attributes and elements</span></span>

<span data-ttu-id="408a9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="408a9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="408a9-108">属性</span><span class="sxs-lookup"><span data-stu-id="408a9-108">Attributes</span></span>

<span data-ttu-id="408a9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="408a9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="408a9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="408a9-110">Child elements</span></span>

<span data-ttu-id="408a9-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)  | [Haschanged](haschanged.md)  | [PictureData](picturedata.md)</span><span class="sxs-lookup"><span data-stu-id="408a9-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [HasChanged](haschanged.md) | [PictureData](picturedata.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="408a9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="408a9-112">Parent elements</span></span>

[<span data-ttu-id="408a9-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="408a9-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="408a9-114">注釈</span><span class="sxs-lookup"><span data-stu-id="408a9-114">Remarks</span></span>

<span data-ttu-id="408a9-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="408a9-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="408a9-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="408a9-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="408a9-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="408a9-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="408a9-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="408a9-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="408a9-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="408a9-119">Schema name</span></span>  <br/> |<span data-ttu-id="408a9-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="408a9-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="408a9-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="408a9-121">Validation file</span></span>  <br/> |<span data-ttu-id="408a9-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="408a9-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="408a9-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="408a9-123">Can be empty</span></span>  <br/> ||
   

