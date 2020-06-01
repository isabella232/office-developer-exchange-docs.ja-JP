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
ms.openlocfilehash: eacfe580342e6667fd9fc84ad953a5e4070b6ed7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465822"
---
# <a name="managedfolderid"></a><span data-ttu-id="36a62-103">ManagedFolderId</span><span class="sxs-lookup"><span data-stu-id="36a62-103">ManagedFolderId</span></span>

<span data-ttu-id="36a62-104">**ManagedFolderId**要素には、管理フォルダーのフォルダー ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="36a62-104">The **ManagedFolderId** element contains the folder ID of the managed folder.</span></span> 
  
```xml
<ManagedFolderId/>
```

 <span data-ttu-id="36a62-105">**string**</span><span class="sxs-lookup"><span data-stu-id="36a62-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="36a62-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="36a62-106">Attributes and elements</span></span>

<span data-ttu-id="36a62-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="36a62-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36a62-108">属性</span><span class="sxs-lookup"><span data-stu-id="36a62-108">Attributes</span></span>

<span data-ttu-id="36a62-109">なし。</span><span class="sxs-lookup"><span data-stu-id="36a62-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="36a62-110">子要素</span><span class="sxs-lookup"><span data-stu-id="36a62-110">Child elements</span></span>

<span data-ttu-id="36a62-111">なし。</span><span class="sxs-lookup"><span data-stu-id="36a62-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="36a62-112">親要素</span><span class="sxs-lookup"><span data-stu-id="36a62-112">Parent elements</span></span>

|<span data-ttu-id="36a62-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="36a62-113">**Element**</span></span>|<span data-ttu-id="36a62-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="36a62-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36a62-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="36a62-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="36a62-116">管理フォルダーに関する情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="36a62-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="36a62-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="36a62-117">Text value</span></span>

<span data-ttu-id="36a62-118">この要素にはテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="36a62-118">A text value is required for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="36a62-119">注釈</span><span class="sxs-lookup"><span data-stu-id="36a62-119">Remarks</span></span>

<span data-ttu-id="36a62-120">**ManagedFolderId** identifier の値は、Microsoft Windows Powershell コマンドによって取得される**Guid**プロパティに相当し `Get-ManagedFolder` ます。</span><span class="sxs-lookup"><span data-stu-id="36a62-120">The **ManagedFolderId** identifier value is the equivalent of the **Guid** property that is retrieved by the  `Get-ManagedFolder` Microsoft Windows Powershell command.</span></span> <span data-ttu-id="36a62-121">また、これは、Active Directory ディレクトリサービスの管理フォルダーの**objectGUID**属性の値でもあります。</span><span class="sxs-lookup"><span data-stu-id="36a62-121">It is also the value of the **objectGUID** attribute for the managed folder in the Active Directory directory service.</span></span> 
  
<span data-ttu-id="36a62-122">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="36a62-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="36a62-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="36a62-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36a62-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="36a62-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="36a62-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="36a62-125">Schema name</span></span>  <br/> |<span data-ttu-id="36a62-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="36a62-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="36a62-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="36a62-127">Validation file</span></span>  <br/> |<span data-ttu-id="36a62-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="36a62-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="36a62-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="36a62-129">Can be empty</span></span>  <br/> |<span data-ttu-id="36a62-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="36a62-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="36a62-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="36a62-131">See also</span></span>



[<span data-ttu-id="36a62-132">CreateManagedFolder 操作</span><span class="sxs-lookup"><span data-stu-id="36a62-132">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="36a62-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="36a62-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="36a62-134">フォルダーの削除</span><span class="sxs-lookup"><span data-stu-id="36a62-134">Deleting Folders</span></span>](https://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)
  
[<span data-ttu-id="36a62-135">管理フォルダーの追加</span><span class="sxs-lookup"><span data-stu-id="36a62-135">Adding Managed Folders</span></span>](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

