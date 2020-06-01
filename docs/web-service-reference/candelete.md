---
title: CanDelete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CanDelete
api_type:
- schema
ms.assetid: 55e17121-aad0-4f90-889f-2c3512e9579c
description: CanDelete 要素は、管理フォルダーを顧客が削除できるかどうかを示します。
ms.openlocfilehash: 5fe16c276bdb0c5b3b73ca63099559d3e869db3e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461591"
---
# <a name="candelete"></a><span data-ttu-id="ac1ac-103">CanDelete</span><span class="sxs-lookup"><span data-stu-id="ac1ac-103">CanDelete</span></span>

<span data-ttu-id="ac1ac-104">**Candelete**要素は、管理フォルダーを顧客が削除できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac1ac-104">The **CanDelete** element indicates whether a managed folder can be deleted by a customer.</span></span> 
  
```xml
<CanDelete/>
```

 <span data-ttu-id="ac1ac-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="ac1ac-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ac1ac-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ac1ac-106">Attributes and elements</span></span>

<span data-ttu-id="ac1ac-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ac1ac-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ac1ac-108">属性</span><span class="sxs-lookup"><span data-stu-id="ac1ac-108">Attributes</span></span>

<span data-ttu-id="ac1ac-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ac1ac-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ac1ac-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ac1ac-110">Child elements</span></span>

<span data-ttu-id="ac1ac-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ac1ac-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ac1ac-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ac1ac-112">Parent elements</span></span>

|<span data-ttu-id="ac1ac-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ac1ac-113">**Element**</span></span>|<span data-ttu-id="ac1ac-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ac1ac-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac1ac-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="ac1ac-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="ac1ac-116">管理フォルダーに関する情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="ac1ac-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ac1ac-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ac1ac-117">Text value</span></span>

<span data-ttu-id="ac1ac-118">この要素が存在する場合は、ブール値を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="ac1ac-118">A text value that represents a Boolean value is required if this element is present.</span></span> <span data-ttu-id="ac1ac-119">値が**true の場合**は、フォルダーを削除できることを示します。値が**false**の場合は、フォルダーを削除できないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="ac1ac-119">A value of **true** indicates that the folder can be deleted; a value of **false** means that the folder cannot be deleted.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ac1ac-120">注釈</span><span class="sxs-lookup"><span data-stu-id="ac1ac-120">Remarks</span></span>

<span data-ttu-id="ac1ac-121">管理フォルダーを削除するには、 [deletefolder 操作](deletefolder-operation.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="ac1ac-121">To delete a managed folder, use the [DeleteFolder operation](deletefolder-operation.md).</span></span>
  
<span data-ttu-id="ac1ac-122">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="ac1ac-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ac1ac-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ac1ac-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ac1ac-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="ac1ac-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ac1ac-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ac1ac-125">Schema name</span></span>  <br/> |<span data-ttu-id="ac1ac-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="ac1ac-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="ac1ac-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ac1ac-127">Validation file</span></span>  <br/> |<span data-ttu-id="ac1ac-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="ac1ac-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ac1ac-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ac1ac-129">Can be empty</span></span>  <br/> |<span data-ttu-id="ac1ac-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="ac1ac-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ac1ac-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="ac1ac-131">See also</span></span>



[<span data-ttu-id="ac1ac-132">CreateManagedFolder 操作</span><span class="sxs-lookup"><span data-stu-id="ac1ac-132">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="ac1ac-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ac1ac-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="ac1ac-134">フォルダーの削除</span><span class="sxs-lookup"><span data-stu-id="ac1ac-134">Deleting Folders</span></span>](https://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

