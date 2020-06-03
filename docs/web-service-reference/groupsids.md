---
title: GroupSids
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupSids
api_type:
- schema
ms.assetid: ebb00653-83f0-4080-a902-c38df6719800
description: GroupSids 要素は、Active Directory ディレクトリサービスグループオブジェクトのセキュリティ識別子のコレクションを表します。
ms.openlocfilehash: 40f36176fcaa3e2160237f269fb2dc3b12bf8af2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530065"
---
# <a name="groupsids"></a><span data-ttu-id="36ff7-103">GroupSids</span><span class="sxs-lookup"><span data-stu-id="36ff7-103">GroupSids</span></span>

<span data-ttu-id="36ff7-104">**Groupsids**要素は、Active Directory ディレクトリサービスグループオブジェクトのセキュリティ識別子のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="36ff7-104">The **GroupSids** element represents a collection of Active Directory directory service group object security identifiers.</span></span> 
  
```xml
<GroupSids>
   <GroupIdentifier/>
</GroupSids>
```

 <span data-ttu-id="36ff7-105">**非 Emptyarrayofgroupidentifierstype**</span><span class="sxs-lookup"><span data-stu-id="36ff7-105">**NonEmptyArrayOfGroupIdentifiersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="36ff7-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="36ff7-106">Attributes and elements</span></span>

<span data-ttu-id="36ff7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="36ff7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36ff7-108">属性</span><span class="sxs-lookup"><span data-stu-id="36ff7-108">Attributes</span></span>

<span data-ttu-id="36ff7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="36ff7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="36ff7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="36ff7-110">Child elements</span></span>

|<span data-ttu-id="36ff7-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="36ff7-111">**Element**</span></span>|<span data-ttu-id="36ff7-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="36ff7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36ff7-113">GroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="36ff7-113">GroupIdentifier</span></span>](groupidentifier.md) <br/> |<span data-ttu-id="36ff7-114">アカウントがメンバーである Active Directory オブジェクトグループの単一のセキュリティ識別子と属性を表します。</span><span class="sxs-lookup"><span data-stu-id="36ff7-114">Represents a single security identifier and attribute for an Active Directory object group of which the account is a member.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="36ff7-115">親要素</span><span class="sxs-lookup"><span data-stu-id="36ff7-115">Parent elements</span></span>

|<span data-ttu-id="36ff7-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="36ff7-116">**Element**</span></span>|<span data-ttu-id="36ff7-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="36ff7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36ff7-118">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="36ff7-118">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="36ff7-119">サーバー間認証でトークンをシリアル化するための簡易オブジェクトアクセスプロトコル (SOAP) ヘッダーで使用されます。</span><span class="sxs-lookup"><span data-stu-id="36ff7-119">Used in the Simple Object Access Protocol (SOAP) header for token serialization in server-to-server authentication.</span></span> <span data-ttu-id="36ff7-120">トークンのシリアル化はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36ff7-120">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="36ff7-121">注釈</span><span class="sxs-lookup"><span data-stu-id="36ff7-121">Remarks</span></span>

<span data-ttu-id="36ff7-122">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="36ff7-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="36ff7-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="36ff7-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36ff7-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="36ff7-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="36ff7-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="36ff7-125">Schema Name</span></span>  <br/> |<span data-ttu-id="36ff7-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="36ff7-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="36ff7-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="36ff7-127">Validation File</span></span>  <br/> |<span data-ttu-id="36ff7-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="36ff7-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="36ff7-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="36ff7-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="36ff7-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="36ff7-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="36ff7-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="36ff7-131">See also</span></span>



- [<span data-ttu-id="36ff7-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="36ff7-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

