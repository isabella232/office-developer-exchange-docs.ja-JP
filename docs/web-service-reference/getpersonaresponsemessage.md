---
title: GetPersonaResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a5bf44c6-c46b-442d-98d4-8b49fdf14b30
description: GetPersonaResponseMessage には、GetPersona 要求からの応答データが含まれています。
ms.openlocfilehash: 7d38daac9c7c3a74ba9d9670c2bd16dcf2cd47e3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760833"
---
# <a name="getpersonaresponsemessage"></a><span data-ttu-id="66dab-103">GetPersonaResponseMessage</span><span class="sxs-lookup"><span data-stu-id="66dab-103">GetPersonaResponseMessage</span></span>

<span data-ttu-id="66dab-104">**GetPersonaResponseMessage**には、 **GetPersona**要求からの応答データが含まれています。</span><span class="sxs-lookup"><span data-stu-id="66dab-104">The **GetPersonaResponseMessage** contains the response data resulting from a **GetPersona** request.</span></span> 
  
```XML
<GetPersonaResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Persona/>
</GetPersonaResponseMessage>
```

 <span data-ttu-id="66dab-105">**GetUserPhotoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="66dab-105">**GetUserPhotoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="66dab-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="66dab-106">Attributes and elements</span></span>

<span data-ttu-id="66dab-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="66dab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="66dab-108">属性</span><span class="sxs-lookup"><span data-stu-id="66dab-108">Attributes</span></span>

<span data-ttu-id="66dab-109">なし。</span><span class="sxs-lookup"><span data-stu-id="66dab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="66dab-110">子要素</span><span class="sxs-lookup"><span data-stu-id="66dab-110">Child elements</span></span>

<span data-ttu-id="66dab-111">[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [ペルソナ](persona.md)</span><span class="sxs-lookup"><span data-stu-id="66dab-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [Persona](persona.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="66dab-112">親要素</span><span class="sxs-lookup"><span data-stu-id="66dab-112">Parent elements</span></span>

[<span data-ttu-id="66dab-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="66dab-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="66dab-114">備考</span><span class="sxs-lookup"><span data-stu-id="66dab-114">Remarks</span></span>

<span data-ttu-id="66dab-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="66dab-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="66dab-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="66dab-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="66dab-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="66dab-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="66dab-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="66dab-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="66dab-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="66dab-119">Schema name</span></span>  <br/> |<span data-ttu-id="66dab-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="66dab-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="66dab-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="66dab-121">Validation file</span></span>  <br/> |<span data-ttu-id="66dab-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="66dab-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="66dab-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="66dab-123">Can be empty</span></span>  <br/> ||
   

