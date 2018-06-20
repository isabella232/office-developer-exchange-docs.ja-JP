---
title: RestrictedGroupSids
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RestrictedGroupSids
api_type:
- schema
ms.assetid: 569ab552-5616-444a-a7f5-de366a684a34
description: RestrictedGroupSids 要素は、ユーザーのトークンから、制限されたグループのコレクションを表します。
ms.openlocfilehash: fcfee809261c7ed0a4e0d092c091841fec641e46
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833201"
---
# <a name="restrictedgroupsids"></a><span data-ttu-id="0341d-103">RestrictedGroupSids</span><span class="sxs-lookup"><span data-stu-id="0341d-103">RestrictedGroupSids</span></span>

<span data-ttu-id="0341d-104">**RestrictedGroupSids**要素は、ユーザーのトークンから、制限されたグループのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="0341d-104">The **RestrictedGroupSids** element represents a collection of restricted groups from a user's token.</span></span> 
  
```xml
<RestrictedGroupSids>
   <RestrictedGroupIdentifier/>
</RestrictedGroupSids>
```

 <span data-ttu-id="0341d-105">**NonEmptyArrayOfRestrictedGroupIdentifiersType**</span><span class="sxs-lookup"><span data-stu-id="0341d-105">**NonEmptyArrayOfRestrictedGroupIdentifiersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0341d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0341d-106">Attributes and elements</span></span>

<span data-ttu-id="0341d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0341d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0341d-108">属性</span><span class="sxs-lookup"><span data-stu-id="0341d-108">Attributes</span></span>

<span data-ttu-id="0341d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0341d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0341d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0341d-110">Child elements</span></span>

|<span data-ttu-id="0341d-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="0341d-111">**Element**</span></span>|<span data-ttu-id="0341d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="0341d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0341d-113">RestrictedGroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="0341d-113">RestrictedGroupIdentifier</span></span>](restrictedgroupidentifier.md) <br/> |<span data-ttu-id="0341d-114">グループ セキュリティ識別子 (SID)、制限されたグループの属性を表します。</span><span class="sxs-lookup"><span data-stu-id="0341d-114">Represents the group security identifier (SID) and attributes for a restricted group.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0341d-115">親要素</span><span class="sxs-lookup"><span data-stu-id="0341d-115">Parent elements</span></span>

|<span data-ttu-id="0341d-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="0341d-116">**Element**</span></span>|<span data-ttu-id="0341d-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="0341d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0341d-118">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="0341d-118">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="0341d-119">サーバー間認証でトークンのシリアル化を SOAP ヘッダーで使用されます。</span><span class="sxs-lookup"><span data-stu-id="0341d-119">Used in the SOAP header for token serialization in server- to-server authentication.</span></span> <span data-ttu-id="0341d-120">トークンのシリアル化はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0341d-120">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0341d-121">備考</span><span class="sxs-lookup"><span data-stu-id="0341d-121">Remarks</span></span>

<span data-ttu-id="0341d-122">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="0341d-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0341d-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="0341d-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0341d-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="0341d-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0341d-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0341d-125">Schema Name</span></span>  <br/> |<span data-ttu-id="0341d-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="0341d-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="0341d-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0341d-127">Validation File</span></span>  <br/> |<span data-ttu-id="0341d-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0341d-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0341d-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0341d-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="0341d-130">False</span><span class="sxs-lookup"><span data-stu-id="0341d-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0341d-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="0341d-131">See also</span></span>



- [<span data-ttu-id="0341d-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0341d-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

