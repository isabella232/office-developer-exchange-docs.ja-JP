---
title: GetImItemList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2a243852-362f-4bde-95ab-fe42ead61a85
description: GetImItemList 要素は、インスタントメッセージンググループと連絡先の一覧を取得するための要求を定義します。
ms.openlocfilehash: 435bacdc292eb8e7ea8a7822a2a4cd592598cb03
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456060"
---
# <a name="getimitemlist"></a><span data-ttu-id="59ebf-103">GetImItemList</span><span class="sxs-lookup"><span data-stu-id="59ebf-103">GetImItemList</span></span>

<span data-ttu-id="59ebf-104">**Getimitemlist**要素は、インスタントメッセージンググループと連絡先の一覧を取得するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="59ebf-104">The **GetImItemList** element defines a request to get a list of instant messaging groups and contacts.</span></span> 
  
```XML
<GetImItemList>
   <ExtendedProperties/>
</GetImItemList>
```

 <span data-ttu-id="59ebf-105">**GetImItemListType**</span><span class="sxs-lookup"><span data-stu-id="59ebf-105">**GetImItemListType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="59ebf-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="59ebf-106">Attributes and elements</span></span>

<span data-ttu-id="59ebf-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="59ebf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59ebf-108">属性</span><span class="sxs-lookup"><span data-stu-id="59ebf-108">Attributes</span></span>

<span data-ttu-id="59ebf-109">なし。</span><span class="sxs-lookup"><span data-stu-id="59ebf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59ebf-110">子要素</span><span class="sxs-lookup"><span data-stu-id="59ebf-110">Child elements</span></span>

[<span data-ttu-id="59ebf-111">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span><span class="sxs-lookup"><span data-stu-id="59ebf-111">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span></span>](extendedproperties-nonemptyarrayofextendedfielduris.md)
  
### <a name="parent-elements"></a><span data-ttu-id="59ebf-112">親要素</span><span class="sxs-lookup"><span data-stu-id="59ebf-112">Parent elements</span></span>

<span data-ttu-id="59ebf-113">なし。</span><span class="sxs-lookup"><span data-stu-id="59ebf-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="59ebf-114">注釈</span><span class="sxs-lookup"><span data-stu-id="59ebf-114">Remarks</span></span>

<span data-ttu-id="59ebf-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="59ebf-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="59ebf-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="59ebf-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59ebf-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="59ebf-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59ebf-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="59ebf-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="59ebf-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="59ebf-119">Schema name</span></span>  <br/> |<span data-ttu-id="59ebf-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="59ebf-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="59ebf-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="59ebf-121">Validation file</span></span>  <br/> |<span data-ttu-id="59ebf-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="59ebf-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="59ebf-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="59ebf-123">Can be empty</span></span>  <br/> |<span data-ttu-id="59ebf-124">true</span><span class="sxs-lookup"><span data-stu-id="59ebf-124">true</span></span>  <br/> |
   

