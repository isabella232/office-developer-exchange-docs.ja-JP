---
title: RemoveContactFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 41a7c520-a9ce-4548-9ff7-0ac756523d65
description: RemoveContactFromImList 要素は、インスタントメッセージングの連絡先をすべてのインスタントメッセージンググループから削除する要求を表します。
ms.openlocfilehash: 192f3d28f5f5004300b6b3f2dfcaebf1f3225e76
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458461"
---
# <a name="removecontactfromimlist"></a><span data-ttu-id="95855-103">RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="95855-103">RemoveContactFromImList</span></span>

<span data-ttu-id="95855-104">**RemoveContactFromImList**要素は、インスタントメッセージングの連絡先をすべてのインスタントメッセージンググループから削除する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="95855-104">The **RemoveContactFromImList** element represents a request to remove an instant messaging contact from all instant messaging groups.</span></span> 
  
```XML
<RemoveContactFromImList>
   <ContactId/>
</RemoveContactFromImList>
```

 <span data-ttu-id="95855-105">**RemoveContactFromImListType**</span><span class="sxs-lookup"><span data-stu-id="95855-105">**RemoveContactFromImListType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="95855-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="95855-106">Attributes and elements</span></span>

<span data-ttu-id="95855-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="95855-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="95855-108">属性</span><span class="sxs-lookup"><span data-stu-id="95855-108">Attributes</span></span>

<span data-ttu-id="95855-109">なし。</span><span class="sxs-lookup"><span data-stu-id="95855-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="95855-110">子要素</span><span class="sxs-lookup"><span data-stu-id="95855-110">Child elements</span></span>

[<span data-ttu-id="95855-111">ContactId</span><span class="sxs-lookup"><span data-stu-id="95855-111">ContactId</span></span>](contactid.md)
  
### <a name="parent-elements"></a><span data-ttu-id="95855-112">親要素</span><span class="sxs-lookup"><span data-stu-id="95855-112">Parent elements</span></span>

<span data-ttu-id="95855-113">なし。</span><span class="sxs-lookup"><span data-stu-id="95855-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="95855-114">注釈</span><span class="sxs-lookup"><span data-stu-id="95855-114">Remarks</span></span>

<span data-ttu-id="95855-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="95855-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="95855-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="95855-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="95855-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="95855-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="95855-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="95855-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="95855-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="95855-119">Schema name</span></span>  <br/> |<span data-ttu-id="95855-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="95855-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="95855-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="95855-121">Validation file</span></span>  <br/> |<span data-ttu-id="95855-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="95855-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="95855-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="95855-123">Can be empty</span></span>  <br/> ||
   

