---
title: GetPersonaResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a5bf44c6-c46b-442d-98d4-8b49fdf14b30
description: GetPersonaResponseMessage には、GetPersona 要求の結果として得られる応答データが含まれています。
ms.openlocfilehash: 6391e1b6682180e292d03c5db651e8edc6f46b52
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458328"
---
# <a name="getpersonaresponsemessage"></a><span data-ttu-id="3ddd1-103">GetPersonaResponseMessage</span><span class="sxs-lookup"><span data-stu-id="3ddd1-103">GetPersonaResponseMessage</span></span>

<span data-ttu-id="3ddd1-104">**GetPersonaResponseMessage**には、 **getpersona**要求の結果として得られる応答データが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3ddd1-104">The **GetPersonaResponseMessage** contains the response data resulting from a **GetPersona** request.</span></span> 
  
```XML
<GetPersonaResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Persona/>
</GetPersonaResponseMessage>
```

 <span data-ttu-id="3ddd1-105">**GetUserPhotoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3ddd1-105">**GetUserPhotoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3ddd1-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3ddd1-106">Attributes and elements</span></span>

<span data-ttu-id="3ddd1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3ddd1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3ddd1-108">属性</span><span class="sxs-lookup"><span data-stu-id="3ddd1-108">Attributes</span></span>

<span data-ttu-id="3ddd1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3ddd1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3ddd1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3ddd1-110">Child elements</span></span>

<span data-ttu-id="3ddd1-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)  | [Persona](persona.md)</span><span class="sxs-lookup"><span data-stu-id="3ddd1-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [Persona](persona.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3ddd1-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3ddd1-112">Parent elements</span></span>

[<span data-ttu-id="3ddd1-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="3ddd1-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="3ddd1-114">注釈</span><span class="sxs-lookup"><span data-stu-id="3ddd1-114">Remarks</span></span>

<span data-ttu-id="3ddd1-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3ddd1-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3ddd1-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3ddd1-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3ddd1-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3ddd1-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3ddd1-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="3ddd1-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3ddd1-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3ddd1-119">Schema name</span></span>  <br/> |<span data-ttu-id="3ddd1-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="3ddd1-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3ddd1-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3ddd1-121">Validation file</span></span>  <br/> |<span data-ttu-id="3ddd1-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="3ddd1-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3ddd1-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3ddd1-123">Can be empty</span></span>  <br/> ||
   

