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
description: RestrictedGroupSids 要素は、ユーザーのトークンからの制限されたグループのコレクションを表します。
ms.openlocfilehash: 739a73d2ac4bdbbee03650d035271b5c8d9ea25a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465360"
---
# <a name="restrictedgroupsids"></a><span data-ttu-id="5ce02-103">RestrictedGroupSids</span><span class="sxs-lookup"><span data-stu-id="5ce02-103">RestrictedGroupSids</span></span>

<span data-ttu-id="5ce02-104">**RestrictedGroupSids**要素は、ユーザーのトークンからの制限されたグループのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="5ce02-104">The **RestrictedGroupSids** element represents a collection of restricted groups from a user's token.</span></span> 
  
```xml
<RestrictedGroupSids>
   <RestrictedGroupIdentifier/>
</RestrictedGroupSids>
```

 <span data-ttu-id="5ce02-105">**NonEmptyArrayOfRestrictedGroupIdentifiersType**</span><span class="sxs-lookup"><span data-stu-id="5ce02-105">**NonEmptyArrayOfRestrictedGroupIdentifiersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5ce02-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5ce02-106">Attributes and elements</span></span>

<span data-ttu-id="5ce02-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5ce02-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5ce02-108">属性</span><span class="sxs-lookup"><span data-stu-id="5ce02-108">Attributes</span></span>

<span data-ttu-id="5ce02-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5ce02-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5ce02-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5ce02-110">Child elements</span></span>

|<span data-ttu-id="5ce02-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="5ce02-111">**Element**</span></span>|<span data-ttu-id="5ce02-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5ce02-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ce02-113">RestrictedGroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="5ce02-113">RestrictedGroupIdentifier</span></span>](restrictedgroupidentifier.md) <br/> |<span data-ttu-id="5ce02-114">グループセキュリティ識別子 (SID) と、制限されたグループの属性を表します。</span><span class="sxs-lookup"><span data-stu-id="5ce02-114">Represents the group security identifier (SID) and attributes for a restricted group.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5ce02-115">親要素</span><span class="sxs-lookup"><span data-stu-id="5ce02-115">Parent elements</span></span>

|<span data-ttu-id="5ce02-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="5ce02-116">**Element**</span></span>|<span data-ttu-id="5ce02-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="5ce02-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ce02-118">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="5ce02-118">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="5ce02-119">サーバー間認証のトークンシリアル化のために SOAP ヘッダーで使用されます。</span><span class="sxs-lookup"><span data-stu-id="5ce02-119">Used in the SOAP header for token serialization in server- to-server authentication.</span></span> <span data-ttu-id="5ce02-120">トークンのシリアル化はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ce02-120">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5ce02-121">注釈</span><span class="sxs-lookup"><span data-stu-id="5ce02-121">Remarks</span></span>

<span data-ttu-id="5ce02-122">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="5ce02-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5ce02-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5ce02-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5ce02-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="5ce02-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5ce02-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5ce02-125">Schema Name</span></span>  <br/> |<span data-ttu-id="5ce02-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="5ce02-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="5ce02-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5ce02-127">Validation File</span></span>  <br/> |<span data-ttu-id="5ce02-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="5ce02-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5ce02-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5ce02-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="5ce02-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="5ce02-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5ce02-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="5ce02-131">See also</span></span>



- [<span data-ttu-id="5ce02-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="5ce02-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

