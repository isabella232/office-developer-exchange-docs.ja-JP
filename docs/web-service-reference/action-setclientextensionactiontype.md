---
title: Action (SetClientExtensionActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c5624a87-3436-40ce-8d6b-cc01eecab64d
description: Action 要素には、Exchange サーバーがアプリに対して実行するアクションが含まれています。
ms.openlocfilehash: 29579e26377edacb5fb0bb8406144eeb116b8d15
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529687"
---
# <a name="action-setclientextensionactiontype"></a><span data-ttu-id="fa10f-103">Action (SetClientExtensionActionType)</span><span class="sxs-lookup"><span data-stu-id="fa10f-103">Action (SetClientExtensionActionType)</span></span>

<span data-ttu-id="fa10f-104">**Action**要素には、Exchange サーバーがアプリに対して実行するアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fa10f-104">The **Action** element contains the action that the Exchange server should take on an app.</span></span> 
  
```XML
<Action ActionId="" ExtensionId="">
   <ClientExtension/>
</Action>
```

 <span data-ttu-id="fa10f-105">**SetClientExtensionActionType**</span><span class="sxs-lookup"><span data-stu-id="fa10f-105">**SetClientExtensionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fa10f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="fa10f-106">Attributes and elements</span></span>

<span data-ttu-id="fa10f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fa10f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fa10f-108">属性</span><span class="sxs-lookup"><span data-stu-id="fa10f-108">Attributes</span></span>

|<span data-ttu-id="fa10f-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="fa10f-109">**Attribute**</span></span>|<span data-ttu-id="fa10f-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="fa10f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fa10f-111">ActionId</span><span class="sxs-lookup"><span data-stu-id="fa10f-111">ActionId</span></span>  <br/> |<span data-ttu-id="fa10f-112">アクションの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="fa10f-112">Specifies the identifier of the action.</span></span> <span data-ttu-id="fa10f-113">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="fa10f-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="fa10f-114">ExtensionId</span><span class="sxs-lookup"><span data-stu-id="fa10f-114">ExtensionId</span></span>  <br/> |<span data-ttu-id="fa10f-115">拡張機能の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="fa10f-115">Specifies the identifier of the extension.</span></span> <span data-ttu-id="fa10f-116">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="fa10f-116">This attribute is optional.</span></span>  <br/> |
   
#### <a name="actionid"></a><span data-ttu-id="fa10f-117">ActionId</span><span class="sxs-lookup"><span data-stu-id="fa10f-117">ActionId</span></span>

|<span data-ttu-id="fa10f-118">**値**</span><span class="sxs-lookup"><span data-stu-id="fa10f-118">**Value**</span></span>|<span data-ttu-id="fa10f-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="fa10f-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fa10f-120">Configure</span><span class="sxs-lookup"><span data-stu-id="fa10f-120">Configure</span></span>  <br/> |<span data-ttu-id="fa10f-121">構成操作を示します。</span><span class="sxs-lookup"><span data-stu-id="fa10f-121">Indicates a configuration action.</span></span>  <br/> |
|<span data-ttu-id="fa10f-122">Install</span><span class="sxs-lookup"><span data-stu-id="fa10f-122">Install</span></span>  <br/> |<span data-ttu-id="fa10f-123">インストールアクションを示します。</span><span class="sxs-lookup"><span data-stu-id="fa10f-123">Indicates an installation action.</span></span>  <br/> |
|<span data-ttu-id="fa10f-124">Uninstall</span><span class="sxs-lookup"><span data-stu-id="fa10f-124">Uninstall</span></span>  <br/> |<span data-ttu-id="fa10f-125">アンインストールアクションを示します。</span><span class="sxs-lookup"><span data-stu-id="fa10f-125">Indicates an uninstallation action.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fa10f-126">子要素</span><span class="sxs-lookup"><span data-stu-id="fa10f-126">Child elements</span></span>

|<span data-ttu-id="fa10f-127">**Element**</span><span class="sxs-lookup"><span data-stu-id="fa10f-127">**Element**</span></span>|<span data-ttu-id="fa10f-128">**説明**</span><span class="sxs-lookup"><span data-stu-id="fa10f-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa10f-129">ClientExtension</span><span class="sxs-lookup"><span data-stu-id="fa10f-129">ClientExtension</span></span>](clientextension.md) <br/> |<span data-ttu-id="fa10f-130">アプリに関するユーザーおよび構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fa10f-130">Contains user and configuration information about an app.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fa10f-131">親要素</span><span class="sxs-lookup"><span data-stu-id="fa10f-131">Parent elements</span></span>

|<span data-ttu-id="fa10f-132">**要素**</span><span class="sxs-lookup"><span data-stu-id="fa10f-132">**Element**</span></span>|<span data-ttu-id="fa10f-133">**説明**</span><span class="sxs-lookup"><span data-stu-id="fa10f-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa10f-134">Actions (ArrayOfSetClientExtensionActionsType)</span><span class="sxs-lookup"><span data-stu-id="fa10f-134">Actions (ArrayOfSetClientExtensionActionsType)</span></span>](actions-arrayofsetclientextensionactionstype.md) <br/> |<span data-ttu-id="fa10f-135">**Action**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="fa10f-135">Specifies an array of **Action** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fa10f-136">注釈</span><span class="sxs-lookup"><span data-stu-id="fa10f-136">Remarks</span></span>

<span data-ttu-id="fa10f-137">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fa10f-137">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fa10f-138">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fa10f-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fa10f-139">要素の情報</span><span class="sxs-lookup"><span data-stu-id="fa10f-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fa10f-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="fa10f-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fa10f-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fa10f-141">Schema Name</span></span>  <br/> |<span data-ttu-id="fa10f-142">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="fa10f-142">Type schema</span></span>  <br/> |
|<span data-ttu-id="fa10f-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fa10f-143">Validation File</span></span>  <br/> |<span data-ttu-id="fa10f-144">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="fa10f-144">types.xsd</span></span>  <br/> |
|<span data-ttu-id="fa10f-145">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fa10f-145">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="fa10f-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="fa10f-146">See also</span></span>

- [<span data-ttu-id="fa10f-147">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="fa10f-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

