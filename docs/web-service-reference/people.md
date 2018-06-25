---
title: 複数のユーザー
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 65312428-548c-4fe9-971a-d0dab3be5ddf
description: 人の要素は、FindPeople 要求の結果として返されるペルソナ データの配列を指定します。
ms.openlocfilehash: df6f1af34872abe13a1d0f3a98b0354c55354e31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832712"
---
# <a name="people"></a><span data-ttu-id="863cf-103">複数のユーザー</span><span class="sxs-lookup"><span data-stu-id="863cf-103">People</span></span>

<span data-ttu-id="863cf-104">**人**の要素は、 **FindPeople**要求の結果として返されるペルソナ データの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="863cf-104">The **People** element specifies an array of persona data returned as the result of a **FindPeople** request.</span></span> 
  
```XML
<People>
   <Persona/>
</People>
```

<span data-ttu-id="863cf-105">**ArrayOfPeopleType**</span><span class="sxs-lookup"><span data-stu-id="863cf-105">**ArrayOfPeopleType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="863cf-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="863cf-106">Attributes and elements</span></span>

<span data-ttu-id="863cf-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="863cf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="863cf-108">属性</span><span class="sxs-lookup"><span data-stu-id="863cf-108">Attributes</span></span>

<span data-ttu-id="863cf-109">なし。</span><span class="sxs-lookup"><span data-stu-id="863cf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="863cf-110">子要素</span><span class="sxs-lookup"><span data-stu-id="863cf-110">Child elements</span></span>

[<span data-ttu-id="863cf-111">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="863cf-111">Persona</span></span>](persona.md)
  
### <a name="parent-elements"></a><span data-ttu-id="863cf-112">親要素</span><span class="sxs-lookup"><span data-stu-id="863cf-112">Parent elements</span></span>

[<span data-ttu-id="863cf-113">FindPeopleResponse</span><span class="sxs-lookup"><span data-stu-id="863cf-113">FindPeopleResponse</span></span>](findpeopleresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="863cf-114">備考</span><span class="sxs-lookup"><span data-stu-id="863cf-114">Remarks</span></span>

<span data-ttu-id="863cf-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="863cf-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="863cf-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="863cf-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="863cf-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="863cf-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="863cf-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="863cf-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="863cf-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="863cf-119">Schema name</span></span>  <br/> |<span data-ttu-id="863cf-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="863cf-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="863cf-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="863cf-121">Validation file</span></span>  <br/> |<span data-ttu-id="863cf-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="863cf-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="863cf-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="863cf-123">Can be empty</span></span>  <br/> ||
   

