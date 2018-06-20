---
title: MarkAllItemsAsReadResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e52f56d4-c6a3-458a-8abb-4e0c19d32341
description: MarkAllItemsAsReadResponseMessage 要素は、MarkAllItemsAsRead 要求の応答メッセージを指定します。
ms.openlocfilehash: e1e0ba3748fe12b6c7f54f0acaa5e1f699a4869a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832349"
---
# <a name="markallitemsasreadresponsemessage"></a><span data-ttu-id="8d200-103">MarkAllItemsAsReadResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8d200-103">MarkAllItemsAsReadResponseMessage</span></span>

<span data-ttu-id="8d200-104">**MarkAllItemsAsReadResponseMessage**要素は、 **MarkAllItemsAsRead**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="8d200-104">The **MarkAllItemsAsReadResponseMessage** element specifies the response message for a **MarkAllItemsAsRead** request.</span></span> 
  
```XML
<MarkAllItemsAsReadResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</MarkAllItemsAsReadResponseMessage>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="8d200-105">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8d200-105">Attributes and elements</span></span>

<span data-ttu-id="8d200-106">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8d200-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d200-107">属性</span><span class="sxs-lookup"><span data-stu-id="8d200-107">Attributes</span></span>

<span data-ttu-id="8d200-108">なし。</span><span class="sxs-lookup"><span data-stu-id="8d200-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8d200-109">子要素</span><span class="sxs-lookup"><span data-stu-id="8d200-109">Child elements</span></span>

<span data-ttu-id="8d200-110">[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md)</span><span class="sxs-lookup"><span data-stu-id="8d200-110">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8d200-111">親要素</span><span class="sxs-lookup"><span data-stu-id="8d200-111">Parent elements</span></span>

[<span data-ttu-id="8d200-112">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8d200-112">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="8d200-113">備考</span><span class="sxs-lookup"><span data-stu-id="8d200-113">Remarks</span></span>

<span data-ttu-id="8d200-114">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8d200-114">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8d200-115">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8d200-115">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8d200-116">要素情報</span><span class="sxs-lookup"><span data-stu-id="8d200-116">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8d200-117">名前空間</span><span class="sxs-lookup"><span data-stu-id="8d200-117">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8d200-118">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8d200-118">Schema name</span></span>  <br/> |<span data-ttu-id="8d200-119">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="8d200-119">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8d200-120">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8d200-120">Validation file</span></span>  <br/> |<span data-ttu-id="8d200-121">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8d200-121">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8d200-122">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8d200-122">Can be empty</span></span>  <br/> ||
   

