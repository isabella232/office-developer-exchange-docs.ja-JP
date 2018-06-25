---
title: GetImItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 455e5709-6c06-49fd-bfb2-403fc912287c
description: GetImItems 要求の要素は、指定したインスタント メッセージング グループとインスタント メッセージの連絡先のペルソナに関する情報を取得する要求を定義します。
ms.openlocfilehash: ff7d520dde44fac6e9278633c1ad46b07b38d6c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760755"
---
# <a name="getimitems"></a><span data-ttu-id="7652f-103">GetImItems</span><span class="sxs-lookup"><span data-stu-id="7652f-103">GetImItems</span></span>

<span data-ttu-id="7652f-104">**GetImItems**要求の要素は、指定したインスタント メッセージング グループとインスタント メッセージの連絡先のペルソナに関する情報を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="7652f-104">The **GetImItems** request element defines a request to get information about the specified instant messaging groups and instant messaging contact personas.</span></span> 
  
```XML
<GetImItems>
   <ContactIds/>
   <GroupIds/>
   <ExtendedProperties/>
</GetImItems>
```

 <span data-ttu-id="7652f-105">**GetImItemsType**</span><span class="sxs-lookup"><span data-stu-id="7652f-105">**GetImItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7652f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7652f-106">Attributes and elements</span></span>

<span data-ttu-id="7652f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7652f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7652f-108">属性</span><span class="sxs-lookup"><span data-stu-id="7652f-108">Attributes</span></span>

<span data-ttu-id="7652f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7652f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7652f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7652f-110">Child elements</span></span>

<span data-ttu-id="7652f-111">[ContactIds](contactids.md) | [GroupIds](groupids.md) | [ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)](extendedproperties-nonemptyarrayofextendedfielduris.md)</span><span class="sxs-lookup"><span data-stu-id="7652f-111">[ContactIds](contactids.md) | [GroupIds](groupids.md) | [ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)](extendedproperties-nonemptyarrayofextendedfielduris.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7652f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7652f-112">Parent elements</span></span>

<span data-ttu-id="7652f-113">なし。</span><span class="sxs-lookup"><span data-stu-id="7652f-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7652f-114">備考</span><span class="sxs-lookup"><span data-stu-id="7652f-114">Remarks</span></span>

<span data-ttu-id="7652f-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7652f-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7652f-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7652f-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7652f-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="7652f-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7652f-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="7652f-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7652f-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7652f-119">Schema name</span></span>  <br/> |<span data-ttu-id="7652f-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="7652f-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7652f-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7652f-121">Validation file</span></span>  <br/> |<span data-ttu-id="7652f-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7652f-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7652f-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7652f-123">Can be empty</span></span>  <br/> ||
   

