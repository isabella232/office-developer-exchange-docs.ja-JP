---
title: GetUserPhoto
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0e524a09-86f8-4a71-ac5c-66527ae70790
description: GetUserPhoto 要素には、ユーザーの写真を取得する要求が含まれています。
ms.openlocfilehash: 64b0ec67abd70fb237549eb0fed1968275c615ba
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463910"
---
# <a name="getuserphoto"></a><span data-ttu-id="8dc5a-103">GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="8dc5a-103">GetUserPhoto</span></span>

<span data-ttu-id="8dc5a-104">**Getuserphoto**要素には、ユーザーの写真を取得する要求が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8dc5a-104">The **GetUserPhoto** element contains the request to get a user's photo.</span></span> 
  
```XML
<GetUserPhoto>
   <Email/>
   <SizeRequested/>
</GetUserPhoto>
```

 <span data-ttu-id="8dc5a-105">**GetUserPhotoType**</span><span class="sxs-lookup"><span data-stu-id="8dc5a-105">**GetUserPhotoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8dc5a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8dc5a-106">Attributes and elements</span></span>

<span data-ttu-id="8dc5a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8dc5a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8dc5a-108">属性</span><span class="sxs-lookup"><span data-stu-id="8dc5a-108">Attributes</span></span>

<span data-ttu-id="8dc5a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8dc5a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8dc5a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8dc5a-110">Child elements</span></span>

<span data-ttu-id="8dc5a-111">[電子メール (文字列)](email-string.md)  | [SizeRequested](sizerequested.md)</span><span class="sxs-lookup"><span data-stu-id="8dc5a-111">[Email (String)](email-string.md) | [SizeRequested](sizerequested.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8dc5a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8dc5a-112">Parent elements</span></span>

<span data-ttu-id="8dc5a-113">なし。</span><span class="sxs-lookup"><span data-stu-id="8dc5a-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8dc5a-114">注釈</span><span class="sxs-lookup"><span data-stu-id="8dc5a-114">Remarks</span></span>

<span data-ttu-id="8dc5a-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8dc5a-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8dc5a-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8dc5a-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8dc5a-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8dc5a-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8dc5a-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="8dc5a-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8dc5a-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8dc5a-119">Schema name</span></span>  <br/> |<span data-ttu-id="8dc5a-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="8dc5a-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8dc5a-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8dc5a-121">Validation file</span></span>  <br/> |<span data-ttu-id="8dc5a-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="8dc5a-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8dc5a-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8dc5a-123">Can be empty</span></span>  <br/> ||
   

