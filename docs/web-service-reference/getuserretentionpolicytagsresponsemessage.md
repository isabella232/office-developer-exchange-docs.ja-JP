---
title: GetUserRetentionPolicyTagsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9991d6e0-8c31-4e73-8af3-da4298474b66
description: GetUserRetentionPolicyTagsResponseMessage 要素は、GetUserRetentionPolicyTags 要求の応答メッセージを指定します。
ms.openlocfilehash: db73cb7f1922d845c9565753ff8d4917b82b1259
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831701"
---
# <a name="getuserretentionpolicytagsresponsemessage"></a><span data-ttu-id="90425-103">GetUserRetentionPolicyTagsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="90425-103">GetUserRetentionPolicyTagsResponseMessage</span></span>

<span data-ttu-id="90425-104">**GetUserRetentionPolicyTagsResponseMessage**要素は、 **GetUserRetentionPolicyTags**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="90425-104">The **GetUserRetentionPolicyTagsResponseMessage** element specifies the response message for a **GetUserRetentionPolicyTags** request.</span></span> 
  
```XML
<GetUserRetentionPolicyTagsResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RetentionPolicyTags/>
</GetUserRetentionPolicyTagsResponseMessage>
```

 <span data-ttu-id="90425-105">**GetUserRetentionPolicyTagsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="90425-105">**GetUserRetentionPolicyTagsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="90425-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="90425-106">Attributes and elements</span></span>

<span data-ttu-id="90425-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="90425-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90425-108">属性</span><span class="sxs-lookup"><span data-stu-id="90425-108">Attributes</span></span>

<span data-ttu-id="90425-109">なし。</span><span class="sxs-lookup"><span data-stu-id="90425-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="90425-110">子要素</span><span class="sxs-lookup"><span data-stu-id="90425-110">Child elements</span></span>

<span data-ttu-id="90425-111">[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [RetentionPolicyTags](retentionpolicytags.md)</span><span class="sxs-lookup"><span data-stu-id="90425-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [RetentionPolicyTags](retentionpolicytags.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="90425-112">親要素</span><span class="sxs-lookup"><span data-stu-id="90425-112">Parent elements</span></span>

[<span data-ttu-id="90425-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="90425-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="90425-114">備考</span><span class="sxs-lookup"><span data-stu-id="90425-114">Remarks</span></span>

<span data-ttu-id="90425-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="90425-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="90425-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="90425-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="90425-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="90425-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="90425-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="90425-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="90425-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="90425-119">Schema name</span></span>  <br/> |<span data-ttu-id="90425-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="90425-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="90425-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="90425-121">Validation file</span></span>  <br/> |<span data-ttu-id="90425-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="90425-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="90425-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="90425-123">Can be empty</span></span>  <br/> |<span data-ttu-id="90425-124">false</span><span class="sxs-lookup"><span data-stu-id="90425-124">false</span></span>  <br/> |
   

