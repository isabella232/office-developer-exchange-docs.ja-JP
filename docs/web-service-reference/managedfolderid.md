---
title: ManagedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ManagedFolderId
api_type:
- schema
ms.assetid: 3efb7abb-0e91-4d8a-9fa2-3dec8bd17c30
description: ManagedFolderId 要素には、管理フォルダーのフォルダー ID が含まれています。
ms.openlocfilehash: acdb69f82678633baff12c46494c39015c36d233
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832340"
---
# <a name="managedfolderid"></a><span data-ttu-id="6f7d7-103">ManagedFolderId</span><span class="sxs-lookup"><span data-stu-id="6f7d7-103">ManagedFolderId</span></span>

<span data-ttu-id="6f7d7-104">**ManagedFolderId**要素には、管理フォルダーのフォルダー ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6f7d7-104">The **ManagedFolderId** element contains the folder ID of the managed folder.</span></span> 
  
```xml
<ManagedFolderId/>
```

 <span data-ttu-id="6f7d7-105">**string**</span><span class="sxs-lookup"><span data-stu-id="6f7d7-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6f7d7-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6f7d7-106">Attributes and elements</span></span>

<span data-ttu-id="6f7d7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6f7d7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6f7d7-108">属性</span><span class="sxs-lookup"><span data-stu-id="6f7d7-108">Attributes</span></span>

<span data-ttu-id="6f7d7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6f7d7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6f7d7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6f7d7-110">Child elements</span></span>

<span data-ttu-id="6f7d7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6f7d7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6f7d7-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6f7d7-112">Parent elements</span></span>

|<span data-ttu-id="6f7d7-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6f7d7-113">**Element**</span></span>|<span data-ttu-id="6f7d7-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6f7d7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f7d7-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="6f7d7-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="6f7d7-116">管理フォルダーに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6f7d7-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6f7d7-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6f7d7-117">Text value</span></span>

<span data-ttu-id="6f7d7-118">テキスト値は、この要素の必要があります。</span><span class="sxs-lookup"><span data-stu-id="6f7d7-118">A text value is required for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6f7d7-119">備考</span><span class="sxs-lookup"><span data-stu-id="6f7d7-119">Remarks</span></span>

<span data-ttu-id="6f7d7-120">**Guid**プロパティによって取得されるのと同じでは識別子の値を**ManagedFolderId** `Get-ManagedFolder` Microsoft Windows Powershell コマンドです。</span><span class="sxs-lookup"><span data-stu-id="6f7d7-120">The **ManagedFolderId** identifier value is the equivalent of the **Guid** property that is retrieved by the  `Get-ManagedFolder` Microsoft Windows Powershell command.</span></span> <span data-ttu-id="6f7d7-121">また、Active Directory ディレクトリ サービスの管理対象フォルダーの**objectGUID**属性の値です。</span><span class="sxs-lookup"><span data-stu-id="6f7d7-121">It is also the value of the **objectGUID** attribute for the managed folder in the Active Directory directory service.</span></span> 
  
<span data-ttu-id="6f7d7-122">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="6f7d7-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6f7d7-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="6f7d7-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6f7d7-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="6f7d7-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6f7d7-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6f7d7-125">Schema name</span></span>  <br/> |<span data-ttu-id="6f7d7-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6f7d7-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="6f7d7-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6f7d7-127">Validation file</span></span>  <br/> |<span data-ttu-id="6f7d7-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6f7d7-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6f7d7-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6f7d7-129">Can be empty</span></span>  <br/> |<span data-ttu-id="6f7d7-130">False</span><span class="sxs-lookup"><span data-stu-id="6f7d7-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6f7d7-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="6f7d7-131">See also</span></span>



[<span data-ttu-id="6f7d7-132">CreateManagedFolder 操作</span><span class="sxs-lookup"><span data-stu-id="6f7d7-132">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="6f7d7-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6f7d7-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="6f7d7-134">フォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="6f7d7-134">Deleting Folders</span></span>](http://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)
  
[<span data-ttu-id="6f7d7-135">管理フォルダーを追加します。</span><span class="sxs-lookup"><span data-stu-id="6f7d7-135">Adding Managed Folders</span></span>](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

