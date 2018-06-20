---
title: GetImItemList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2a243852-362f-4bde-95ab-fe42ead61a85
description: GetImItemList 要素は、インスタント メッセージング グループと連絡先の一覧を取得する要求を定義します。
ms.openlocfilehash: b39a9e85c58f253511acaa21f62e1a4277fd56e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760752"
---
# <a name="getimitemlist"></a><span data-ttu-id="b6c86-103">GetImItemList</span><span class="sxs-lookup"><span data-stu-id="b6c86-103">GetImItemList</span></span>

<span data-ttu-id="b6c86-104">**GetImItemList**要素は、インスタント メッセージング グループと連絡先の一覧を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="b6c86-104">The **GetImItemList** element defines a request to get a list of instant messaging groups and contacts.</span></span> 
  
```XML
<GetImItemList>
   <ExtendedProperties/>
</GetImItemList>
```

 <span data-ttu-id="b6c86-105">**GetImItemListType**</span><span class="sxs-lookup"><span data-stu-id="b6c86-105">**GetImItemListType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b6c86-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b6c86-106">Attributes and elements</span></span>

<span data-ttu-id="b6c86-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b6c86-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b6c86-108">属性</span><span class="sxs-lookup"><span data-stu-id="b6c86-108">Attributes</span></span>

<span data-ttu-id="b6c86-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b6c86-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b6c86-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b6c86-110">Child elements</span></span>

[<span data-ttu-id="b6c86-111">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span><span class="sxs-lookup"><span data-stu-id="b6c86-111">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span></span>](extendedproperties-nonemptyarrayofextendedfielduris.md)
  
### <a name="parent-elements"></a><span data-ttu-id="b6c86-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b6c86-112">Parent elements</span></span>

<span data-ttu-id="b6c86-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b6c86-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b6c86-114">備考</span><span class="sxs-lookup"><span data-stu-id="b6c86-114">Remarks</span></span>

<span data-ttu-id="b6c86-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b6c86-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b6c86-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b6c86-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b6c86-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="b6c86-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6c86-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="b6c86-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b6c86-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b6c86-119">Schema name</span></span>  <br/> |<span data-ttu-id="b6c86-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="b6c86-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b6c86-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b6c86-121">Validation file</span></span>  <br/> |<span data-ttu-id="b6c86-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b6c86-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b6c86-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b6c86-123">Can be empty</span></span>  <br/> |<span data-ttu-id="b6c86-124">true</span><span class="sxs-lookup"><span data-stu-id="b6c86-124">true</span></span>  <br/> |
   

