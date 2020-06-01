---
title: ユーザー
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 65312428-548c-4fe9-971a-d0dab3be5ddf
description: People 要素は、FindPeople 要求の結果として返されるペルソナデータの配列を指定します。
ms.openlocfilehash: b3920ca5cdf1d219c5fe119caeaaaf4965c39794
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467187"
---
# <a name="people"></a><span data-ttu-id="ba1a7-103">ユーザー</span><span class="sxs-lookup"><span data-stu-id="ba1a7-103">People</span></span>

<span data-ttu-id="ba1a7-104">**People**要素は、 **findpeople**要求の結果として返されるペルソナデータの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="ba1a7-104">The **People** element specifies an array of persona data returned as the result of a **FindPeople** request.</span></span> 
  
```XML
<People>
   <Persona/>
</People>
```

<span data-ttu-id="ba1a7-105">**ArrayOfPeopleType**</span><span class="sxs-lookup"><span data-stu-id="ba1a7-105">**ArrayOfPeopleType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ba1a7-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ba1a7-106">Attributes and elements</span></span>

<span data-ttu-id="ba1a7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ba1a7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ba1a7-108">属性</span><span class="sxs-lookup"><span data-stu-id="ba1a7-108">Attributes</span></span>

<span data-ttu-id="ba1a7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ba1a7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ba1a7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ba1a7-110">Child elements</span></span>

[<span data-ttu-id="ba1a7-111">ユーザー</span><span class="sxs-lookup"><span data-stu-id="ba1a7-111">Persona</span></span>](persona.md)
  
### <a name="parent-elements"></a><span data-ttu-id="ba1a7-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ba1a7-112">Parent elements</span></span>

[<span data-ttu-id="ba1a7-113">FindPeopleResponse</span><span class="sxs-lookup"><span data-stu-id="ba1a7-113">FindPeopleResponse</span></span>](findpeopleresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="ba1a7-114">注釈</span><span class="sxs-lookup"><span data-stu-id="ba1a7-114">Remarks</span></span>

<span data-ttu-id="ba1a7-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ba1a7-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ba1a7-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ba1a7-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ba1a7-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ba1a7-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ba1a7-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="ba1a7-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ba1a7-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ba1a7-119">Schema name</span></span>  <br/> |<span data-ttu-id="ba1a7-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="ba1a7-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ba1a7-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ba1a7-121">Validation file</span></span>  <br/> |<span data-ttu-id="ba1a7-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="ba1a7-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ba1a7-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ba1a7-123">Can be empty</span></span>  <br/> ||
   

