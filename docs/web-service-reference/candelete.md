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
description: CanDelete 要素は、顧客が管理対象のフォルダーを削除できるかどうかを示します。
ms.openlocfilehash: b70b28bd6b3c9452f5d7f249f453218d555754da
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759607"
---
# <a name="candelete"></a><span data-ttu-id="07be7-103">CanDelete</span><span class="sxs-lookup"><span data-stu-id="07be7-103">CanDelete</span></span>

<span data-ttu-id="07be7-104">**CanDelete**要素は、顧客が管理対象のフォルダーを削除できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="07be7-104">The **CanDelete** element indicates whether a managed folder can be deleted by a customer.</span></span> 
  
```xml
<CanDelete/>
```

 <span data-ttu-id="07be7-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="07be7-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="07be7-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="07be7-106">Attributes and elements</span></span>

<span data-ttu-id="07be7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="07be7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="07be7-108">属性</span><span class="sxs-lookup"><span data-stu-id="07be7-108">Attributes</span></span>

<span data-ttu-id="07be7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="07be7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="07be7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="07be7-110">Child elements</span></span>

<span data-ttu-id="07be7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="07be7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="07be7-112">親要素</span><span class="sxs-lookup"><span data-stu-id="07be7-112">Parent elements</span></span>

|<span data-ttu-id="07be7-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="07be7-113">**Element**</span></span>|<span data-ttu-id="07be7-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="07be7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07be7-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="07be7-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="07be7-116">管理フォルダーに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="07be7-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="07be7-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="07be7-117">Text value</span></span>

<span data-ttu-id="07be7-118">ブール値を表す文字列値は、この要素が存在する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="07be7-118">A text value that represents a Boolean value is required if this element is present.</span></span> <span data-ttu-id="07be7-119">**True**を示します、フォルダーを削除できます。**false**の値は、フォルダーを削除できないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="07be7-119">A value of **true** indicates that the folder can be deleted; a value of **false** means that the folder cannot be deleted.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="07be7-120">備考</span><span class="sxs-lookup"><span data-stu-id="07be7-120">Remarks</span></span>

<span data-ttu-id="07be7-121">管理フォルダーを削除するには、 [DeleteFolder 操作](deletefolder-operation.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="07be7-121">To delete a managed folder, use the [DeleteFolder operation](deletefolder-operation.md).</span></span>
  
<span data-ttu-id="07be7-122">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="07be7-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="07be7-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="07be7-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07be7-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="07be7-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="07be7-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="07be7-125">Schema name</span></span>  <br/> |<span data-ttu-id="07be7-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="07be7-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="07be7-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="07be7-127">Validation file</span></span>  <br/> |<span data-ttu-id="07be7-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="07be7-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="07be7-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="07be7-129">Can be empty</span></span>  <br/> |<span data-ttu-id="07be7-130">False</span><span class="sxs-lookup"><span data-stu-id="07be7-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="07be7-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="07be7-131">See also</span></span>



[<span data-ttu-id="07be7-132">CreateManagedFolder 操作</span><span class="sxs-lookup"><span data-stu-id="07be7-132">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="07be7-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="07be7-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="07be7-134">フォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="07be7-134">Deleting Folders</span></span>](http://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

