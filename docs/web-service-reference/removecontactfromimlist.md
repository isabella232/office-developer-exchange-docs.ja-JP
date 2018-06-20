---
title: RemoveContactFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 41a7c520-a9ce-4548-9ff7-0ac756523d65
description: RemoveContactFromImList 要素は、インスタント メッセージ、インスタント メッセージングのすべてのグループから連絡先を削除する要求を表します。
ms.openlocfilehash: c98b44ba829137006c9aeb231e3f3439deec4687
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833078"
---
# <a name="removecontactfromimlist"></a><span data-ttu-id="24176-103">RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="24176-103">RemoveContactFromImList</span></span>

<span data-ttu-id="24176-104">**RemoveContactFromImList**要素は、インスタント メッセージ、インスタント メッセージングのすべてのグループから連絡先を削除する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="24176-104">The **RemoveContactFromImList** element represents a request to remove an instant messaging contact from all instant messaging groups.</span></span> 
  
```XML
<RemoveContactFromImList>
   <ContactId/>
</RemoveContactFromImList>
```

 <span data-ttu-id="24176-105">**RemoveContactFromImListType**</span><span class="sxs-lookup"><span data-stu-id="24176-105">**RemoveContactFromImListType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="24176-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="24176-106">Attributes and elements</span></span>

<span data-ttu-id="24176-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="24176-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="24176-108">属性</span><span class="sxs-lookup"><span data-stu-id="24176-108">Attributes</span></span>

<span data-ttu-id="24176-109">なし。</span><span class="sxs-lookup"><span data-stu-id="24176-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="24176-110">子要素</span><span class="sxs-lookup"><span data-stu-id="24176-110">Child elements</span></span>

[<span data-ttu-id="24176-111">ContactId</span><span class="sxs-lookup"><span data-stu-id="24176-111">ContactId</span></span>](contactid.md)
  
### <a name="parent-elements"></a><span data-ttu-id="24176-112">親要素</span><span class="sxs-lookup"><span data-stu-id="24176-112">Parent elements</span></span>

<span data-ttu-id="24176-113">なし。</span><span class="sxs-lookup"><span data-stu-id="24176-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="24176-114">備考</span><span class="sxs-lookup"><span data-stu-id="24176-114">Remarks</span></span>

<span data-ttu-id="24176-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="24176-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="24176-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="24176-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="24176-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="24176-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="24176-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="24176-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="24176-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="24176-119">Schema name</span></span>  <br/> |<span data-ttu-id="24176-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="24176-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="24176-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="24176-121">Validation file</span></span>  <br/> |<span data-ttu-id="24176-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="24176-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="24176-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="24176-123">Can be empty</span></span>  <br/> ||
   

