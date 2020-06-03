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
description: 連絡先要素には、タスクに関連付けられている連絡先の一覧が含まれています。
ms.openlocfilehash: c2b7bbadd494081a3e47b7b6c489218fab31d574
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458391"
---
# <a name="contacts"></a><span data-ttu-id="07f66-103">連絡先</span><span class="sxs-lookup"><span data-stu-id="07f66-103">Contacts</span></span>

<span data-ttu-id="07f66-104">**連絡先**要素には、タスクに関連付けられている連絡先の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="07f66-104">The **Contacts** element contains a list of contacts that are associated with a task.</span></span> 
  
```xml
<Contacts>
   <String/>
</Contacts>
```

 <span data-ttu-id="07f66-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="07f66-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="07f66-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="07f66-106">Attributes and elements</span></span>

<span data-ttu-id="07f66-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="07f66-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="07f66-108">属性</span><span class="sxs-lookup"><span data-stu-id="07f66-108">Attributes</span></span>

<span data-ttu-id="07f66-109">なし。</span><span class="sxs-lookup"><span data-stu-id="07f66-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="07f66-110">子要素</span><span class="sxs-lookup"><span data-stu-id="07f66-110">Child elements</span></span>

|<span data-ttu-id="07f66-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="07f66-111">**Element**</span></span>|<span data-ttu-id="07f66-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="07f66-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07f66-113">String</span><span class="sxs-lookup"><span data-stu-id="07f66-113">String</span></span>](string.md) <br/> |<span data-ttu-id="07f66-114">連絡先名のコンマ区切りリストを表します。</span><span class="sxs-lookup"><span data-stu-id="07f66-114">Represents a comma-separated list of contact names.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="07f66-115">親要素</span><span class="sxs-lookup"><span data-stu-id="07f66-115">Parent elements</span></span>

|<span data-ttu-id="07f66-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="07f66-116">**Element**</span></span>|<span data-ttu-id="07f66-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="07f66-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07f66-118">タスク</span><span class="sxs-lookup"><span data-stu-id="07f66-118">Task</span></span>](task.md) <br/> |<span data-ttu-id="07f66-119">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="07f66-119">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="07f66-120">注釈</span><span class="sxs-lookup"><span data-stu-id="07f66-120">Remarks</span></span>

<span data-ttu-id="07f66-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="07f66-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="07f66-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="07f66-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07f66-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="07f66-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="07f66-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="07f66-124">Schema name</span></span>  <br/> |<span data-ttu-id="07f66-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="07f66-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="07f66-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="07f66-126">Validation file</span></span>  <br/> |<span data-ttu-id="07f66-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="07f66-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="07f66-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="07f66-128">Can be empty</span></span>  <br/> |<span data-ttu-id="07f66-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="07f66-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="07f66-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="07f66-130">See also</span></span>



- [<span data-ttu-id="07f66-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="07f66-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

