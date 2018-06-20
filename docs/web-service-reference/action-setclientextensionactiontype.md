---
title: アクション (SetClientExtensionActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c5624a87-3436-40ce-8d6b-cc01eecab64d
description: Action 要素には、アプリケーションに対して、Exchange server が実行するアクションが含まれています。
ms.openlocfilehash: a231cedfa6e4759dabfcbecfbe9a9b851f834247
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759273"
---
# <a name="action-setclientextensionactiontype"></a><span data-ttu-id="2e9d1-103">アクション (SetClientExtensionActionType)</span><span class="sxs-lookup"><span data-stu-id="2e9d1-103">Action (SetClientExtensionActionType)</span></span>

<span data-ttu-id="2e9d1-104">**Action**要素には、アプリケーションに対して、Exchange server が実行するアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2e9d1-104">The **Action** element contains the action that the Exchange server should take on an app.</span></span> 
  
```XML
<Action ActionId="" ExtensionId="">
   <ClientExtension/>
</Action>
```

 <span data-ttu-id="2e9d1-105">**SetClientExtensionActionType**</span><span class="sxs-lookup"><span data-stu-id="2e9d1-105">**SetClientExtensionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2e9d1-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2e9d1-106">Attributes and elements</span></span>

<span data-ttu-id="2e9d1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2e9d1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2e9d1-108">属性</span><span class="sxs-lookup"><span data-stu-id="2e9d1-108">Attributes</span></span>

|<span data-ttu-id="2e9d1-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="2e9d1-109">**Attribute**</span></span>|<span data-ttu-id="2e9d1-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="2e9d1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2e9d1-111">ActionId</span><span class="sxs-lookup"><span data-stu-id="2e9d1-111">ActionId</span></span>  <br/> |<span data-ttu-id="2e9d1-112">アクションの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="2e9d1-112">Specifies the identifier of the action.</span></span> <span data-ttu-id="2e9d1-113">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="2e9d1-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="2e9d1-114">ExtensionId</span><span class="sxs-lookup"><span data-stu-id="2e9d1-114">ExtensionId</span></span>  <br/> |<span data-ttu-id="2e9d1-115">拡張機能の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="2e9d1-115">Specifies the identifier of the extension.</span></span> <span data-ttu-id="2e9d1-116">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="2e9d1-116">This attribute is optional.</span></span>  <br/> |
   
#### <a name="actionid"></a><span data-ttu-id="2e9d1-117">ActionId</span><span class="sxs-lookup"><span data-stu-id="2e9d1-117">ActionId</span></span>

|<span data-ttu-id="2e9d1-118">**値**</span><span class="sxs-lookup"><span data-stu-id="2e9d1-118">**Value**</span></span>|<span data-ttu-id="2e9d1-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="2e9d1-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2e9d1-120">構成します。</span><span class="sxs-lookup"><span data-stu-id="2e9d1-120">Configure</span></span>  <br/> |<span data-ttu-id="2e9d1-121">構成の操作を示します。</span><span class="sxs-lookup"><span data-stu-id="2e9d1-121">Indicates a configuration action.</span></span>  <br/> |
|<span data-ttu-id="2e9d1-122">インストール</span><span class="sxs-lookup"><span data-stu-id="2e9d1-122">Install</span></span>  <br/> |<span data-ttu-id="2e9d1-123">インストール アクションを示します。</span><span class="sxs-lookup"><span data-stu-id="2e9d1-123">Indicates an installation action.</span></span>  <br/> |
|<span data-ttu-id="2e9d1-124">アンインストール</span><span class="sxs-lookup"><span data-stu-id="2e9d1-124">Uninstall</span></span>  <br/> |<span data-ttu-id="2e9d1-125">アンインストール アクションを示します。</span><span class="sxs-lookup"><span data-stu-id="2e9d1-125">Indicates an uninstallation action.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2e9d1-126">子要素</span><span class="sxs-lookup"><span data-stu-id="2e9d1-126">Child elements</span></span>

|<span data-ttu-id="2e9d1-127">**要素**</span><span class="sxs-lookup"><span data-stu-id="2e9d1-127">**Element**</span></span>|<span data-ttu-id="2e9d1-128">**説明**</span><span class="sxs-lookup"><span data-stu-id="2e9d1-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2e9d1-129">ClientExtension</span><span class="sxs-lookup"><span data-stu-id="2e9d1-129">ClientExtension</span></span>](clientextension.md) <br/> |<span data-ttu-id="2e9d1-130">アプリケーションのユーザーおよび構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2e9d1-130">Contains user and configuration information about an app.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2e9d1-131">親要素</span><span class="sxs-lookup"><span data-stu-id="2e9d1-131">Parent elements</span></span>

|<span data-ttu-id="2e9d1-132">**要素**</span><span class="sxs-lookup"><span data-stu-id="2e9d1-132">**Element**</span></span>|<span data-ttu-id="2e9d1-133">**説明**</span><span class="sxs-lookup"><span data-stu-id="2e9d1-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2e9d1-134">アクション (ArrayOfSetClientExtensionActionsType)</span><span class="sxs-lookup"><span data-stu-id="2e9d1-134">Actions (ArrayOfSetClientExtensionActionsType)</span></span>](actions-arrayofsetclientextensionactionstype.md) <br/> |<span data-ttu-id="2e9d1-135">**アクション**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="2e9d1-135">Specifies an array of **Action** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2e9d1-136">備考</span><span class="sxs-lookup"><span data-stu-id="2e9d1-136">Remarks</span></span>

<span data-ttu-id="2e9d1-137">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2e9d1-137">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2e9d1-138">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2e9d1-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2e9d1-139">要素情報</span><span class="sxs-lookup"><span data-stu-id="2e9d1-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2e9d1-140">名前空間</span><span class="sxs-lookup"><span data-stu-id="2e9d1-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2e9d1-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2e9d1-141">Schema Name</span></span>  <br/> |<span data-ttu-id="2e9d1-142">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="2e9d1-142">Type schema</span></span>  <br/> |
|<span data-ttu-id="2e9d1-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2e9d1-143">Validation File</span></span>  <br/> |<span data-ttu-id="2e9d1-144">types.xsd</span><span class="sxs-lookup"><span data-stu-id="2e9d1-144">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2e9d1-145">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2e9d1-145">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2e9d1-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="2e9d1-146">See also</span></span>

- [<span data-ttu-id="2e9d1-147">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2e9d1-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

