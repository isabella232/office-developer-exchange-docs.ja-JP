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
ms.openlocfilehash: a3609f356dd20e121105b5ca57b389d492e852ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465815"
---
# <a name="markallitemsasreadresponsemessage"></a><span data-ttu-id="8fcaa-103">MarkAllItemsAsReadResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8fcaa-103">MarkAllItemsAsReadResponseMessage</span></span>

<span data-ttu-id="8fcaa-104">**MarkAllItemsAsReadResponseMessage**要素は、 **Markallitemsasread**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="8fcaa-104">The **MarkAllItemsAsReadResponseMessage** element specifies the response message for a **MarkAllItemsAsRead** request.</span></span> 
  
```XML
<MarkAllItemsAsReadResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</MarkAllItemsAsReadResponseMessage>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="8fcaa-105">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8fcaa-105">Attributes and elements</span></span>

<span data-ttu-id="8fcaa-106">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8fcaa-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8fcaa-107">属性</span><span class="sxs-lookup"><span data-stu-id="8fcaa-107">Attributes</span></span>

<span data-ttu-id="8fcaa-108">なし。</span><span class="sxs-lookup"><span data-stu-id="8fcaa-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8fcaa-109">子要素</span><span class="sxs-lookup"><span data-stu-id="8fcaa-109">Child elements</span></span>

<span data-ttu-id="8fcaa-110">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)</span><span class="sxs-lookup"><span data-stu-id="8fcaa-110">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8fcaa-111">親要素</span><span class="sxs-lookup"><span data-stu-id="8fcaa-111">Parent elements</span></span>

[<span data-ttu-id="8fcaa-112">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8fcaa-112">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="8fcaa-113">注釈</span><span class="sxs-lookup"><span data-stu-id="8fcaa-113">Remarks</span></span>

<span data-ttu-id="8fcaa-114">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8fcaa-114">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8fcaa-115">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8fcaa-115">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8fcaa-116">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8fcaa-116">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8fcaa-117">Namespace</span><span class="sxs-lookup"><span data-stu-id="8fcaa-117">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8fcaa-118">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8fcaa-118">Schema name</span></span>  <br/> |<span data-ttu-id="8fcaa-119">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="8fcaa-119">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8fcaa-120">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8fcaa-120">Validation file</span></span>  <br/> |<span data-ttu-id="8fcaa-121">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="8fcaa-121">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8fcaa-122">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8fcaa-122">Can be empty</span></span>  <br/> ||
   

