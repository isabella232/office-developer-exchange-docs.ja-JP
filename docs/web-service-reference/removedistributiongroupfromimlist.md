---
title: RemoveDistributionGroupFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 35d2e592-38c1-4861-8293-f7fba3328f4e
description: RemoveDistributionGroupFromImList 要素は、特定のインスタントメッセージング配布リストグループを削除する要求を表します。
ms.openlocfilehash: 0dff549c62c305a86464eaeac165d5f5bc01c9f5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459596"
---
# <a name="removedistributiongroupfromimlist"></a><span data-ttu-id="197df-103">RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="197df-103">RemoveDistributionGroupFromImList</span></span>

<span data-ttu-id="197df-104">**RemoveDistributionGroupFromImList**要素は、特定のインスタントメッセージング配布リストグループを削除する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="197df-104">The **RemoveDistributionGroupFromImList** element represents a request to remove a specific instant messaging distribution list group.</span></span> 
  
```XML
<RemoveDistributionGroupFromImList>
   <GroupId/>
</RemoveDistributionGroupFromImList>
```

 <span data-ttu-id="197df-105">**RemoveDistributionGroupFromImListType**</span><span class="sxs-lookup"><span data-stu-id="197df-105">**RemoveDistributionGroupFromImListType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="197df-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="197df-106">Attributes and elements</span></span>

<span data-ttu-id="197df-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="197df-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="197df-108">属性</span><span class="sxs-lookup"><span data-stu-id="197df-108">Attributes</span></span>

<span data-ttu-id="197df-109">なし。</span><span class="sxs-lookup"><span data-stu-id="197df-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="197df-110">子要素</span><span class="sxs-lookup"><span data-stu-id="197df-110">Child elements</span></span>

[<span data-ttu-id="197df-111">GroupId</span><span class="sxs-lookup"><span data-stu-id="197df-111">GroupId</span></span>](groupid.md)
  
### <a name="parent-elements"></a><span data-ttu-id="197df-112">親要素</span><span class="sxs-lookup"><span data-stu-id="197df-112">Parent elements</span></span>

<span data-ttu-id="197df-113">なし。</span><span class="sxs-lookup"><span data-stu-id="197df-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="197df-114">注釈</span><span class="sxs-lookup"><span data-stu-id="197df-114">Remarks</span></span>

<span data-ttu-id="197df-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="197df-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="197df-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="197df-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="197df-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="197df-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="197df-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="197df-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="197df-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="197df-119">Schema name</span></span>  <br/> |<span data-ttu-id="197df-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="197df-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="197df-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="197df-121">Validation file</span></span>  <br/> |<span data-ttu-id="197df-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="197df-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="197df-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="197df-123">Can be empty</span></span>  <br/> |<span data-ttu-id="197df-124">false</span><span class="sxs-lookup"><span data-stu-id="197df-124">false</span></span>  <br/> |
   

