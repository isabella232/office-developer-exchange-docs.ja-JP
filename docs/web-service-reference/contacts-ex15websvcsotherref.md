---
title: 連絡先
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Contacts
api_type:
- schema
ms.assetid: 0cc67cdf-9707-45e7-92c6-fa83a016cdbe
description: 連絡先の要素には、タスクに関連付けられている連絡先の一覧が含まれています。
ms.openlocfilehash: da7963d30f58f7da52e76e3f7f1d0f7fd68abf74
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759672"
---
# <a name="contacts"></a><span data-ttu-id="89c5b-103">連絡先</span><span class="sxs-lookup"><span data-stu-id="89c5b-103">Contacts</span></span>

<span data-ttu-id="89c5b-104">**連絡先**の要素には、タスクに関連付けられている連絡先の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="89c5b-104">The **Contacts** element contains a list of contacts that are associated with a task.</span></span> 
  
```xml
<Contacts>
   <String/>
</Contacts>
```

 <span data-ttu-id="89c5b-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="89c5b-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="89c5b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="89c5b-106">Attributes and elements</span></span>

<span data-ttu-id="89c5b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="89c5b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89c5b-108">属性</span><span class="sxs-lookup"><span data-stu-id="89c5b-108">Attributes</span></span>

<span data-ttu-id="89c5b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="89c5b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="89c5b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="89c5b-110">Child elements</span></span>

|<span data-ttu-id="89c5b-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="89c5b-111">**Element**</span></span>|<span data-ttu-id="89c5b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="89c5b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89c5b-113">String</span><span class="sxs-lookup"><span data-stu-id="89c5b-113">String</span></span>](string.md) <br/> |<span data-ttu-id="89c5b-114">連絡先の名前のコンマ区切りのリストを表します。</span><span class="sxs-lookup"><span data-stu-id="89c5b-114">Represents a comma-separated list of contact names.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="89c5b-115">親要素</span><span class="sxs-lookup"><span data-stu-id="89c5b-115">Parent elements</span></span>

|<span data-ttu-id="89c5b-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="89c5b-116">**Element**</span></span>|<span data-ttu-id="89c5b-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="89c5b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89c5b-118">タスク</span><span class="sxs-lookup"><span data-stu-id="89c5b-118">Task</span></span>](task.md) <br/> |<span data-ttu-id="89c5b-119">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="89c5b-119">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="89c5b-120">備考</span><span class="sxs-lookup"><span data-stu-id="89c5b-120">Remarks</span></span>

<span data-ttu-id="89c5b-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="89c5b-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89c5b-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="89c5b-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89c5b-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="89c5b-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="89c5b-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="89c5b-124">Schema name</span></span>  <br/> |<span data-ttu-id="89c5b-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="89c5b-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="89c5b-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="89c5b-126">Validation file</span></span>  <br/> |<span data-ttu-id="89c5b-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="89c5b-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="89c5b-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="89c5b-128">Can be empty</span></span>  <br/> |<span data-ttu-id="89c5b-129">False</span><span class="sxs-lookup"><span data-stu-id="89c5b-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="89c5b-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="89c5b-130">See also</span></span>



- [<span data-ttu-id="89c5b-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="89c5b-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

