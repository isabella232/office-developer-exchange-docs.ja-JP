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
description: GroupSids 要素は、Active Directory ディレクトリ サービス グループ オブジェクト セキュリティ識別子のコレクションを表します。
ms.openlocfilehash: c24c8ea3c3b7d37f41986997ed924c951b4a48ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831790"
---
# <a name="groupsids"></a><span data-ttu-id="c2c68-103">GroupSids</span><span class="sxs-lookup"><span data-stu-id="c2c68-103">GroupSids</span></span>

<span data-ttu-id="c2c68-104">**GroupSids**要素は、Active Directory ディレクトリ サービス グループ オブジェクト セキュリティ識別子のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="c2c68-104">The **GroupSids** element represents a collection of Active Directory directory service group object security identifiers.</span></span> 
  
```xml
<GroupSids>
   <GroupIdentifier/>
</GroupSids>
```

 <span data-ttu-id="c2c68-105">**NonEmptyArrayOfGroupIdentifiersType**</span><span class="sxs-lookup"><span data-stu-id="c2c68-105">**NonEmptyArrayOfGroupIdentifiersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2c68-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c2c68-106">Attributes and elements</span></span>

<span data-ttu-id="c2c68-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c2c68-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2c68-108">属性</span><span class="sxs-lookup"><span data-stu-id="c2c68-108">Attributes</span></span>

<span data-ttu-id="c2c68-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c2c68-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c2c68-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c2c68-110">Child elements</span></span>

|<span data-ttu-id="c2c68-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="c2c68-111">**Element**</span></span>|<span data-ttu-id="c2c68-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="c2c68-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2c68-113">GroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="c2c68-113">GroupIdentifier</span></span>](groupidentifier.md) <br/> |<span data-ttu-id="c2c68-114">1 つのセキュリティ識別子と、アカウントがメンバーである Active Directory オブジェクト グループの属性を表します。</span><span class="sxs-lookup"><span data-stu-id="c2c68-114">Represents a single security identifier and attribute for an Active Directory object group of which the account is a member.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c2c68-115">親要素</span><span class="sxs-lookup"><span data-stu-id="c2c68-115">Parent elements</span></span>

|<span data-ttu-id="c2c68-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="c2c68-116">**Element**</span></span>|<span data-ttu-id="c2c68-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="c2c68-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2c68-118">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="c2c68-118">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="c2c68-119">Simple Object Access Protocol (SOAP) ヘッダーでサーバーからサーバーへの認証でトークンのシリアル化のために使用されます。</span><span class="sxs-lookup"><span data-stu-id="c2c68-119">Used in the Simple Object Access Protocol (SOAP) header for token serialization in server-to-server authentication.</span></span> <span data-ttu-id="c2c68-120">トークンのシリアル化はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2c68-120">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c2c68-121">備考</span><span class="sxs-lookup"><span data-stu-id="c2c68-121">Remarks</span></span>

<span data-ttu-id="c2c68-122">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="c2c68-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2c68-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="c2c68-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2c68-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="c2c68-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c2c68-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c2c68-125">Schema Name</span></span>  <br/> |<span data-ttu-id="c2c68-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c2c68-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="c2c68-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c2c68-127">Validation File</span></span>  <br/> |<span data-ttu-id="c2c68-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c2c68-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c2c68-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c2c68-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="c2c68-130">False</span><span class="sxs-lookup"><span data-stu-id="c2c68-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c2c68-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="c2c68-131">See also</span></span>



- [<span data-ttu-id="c2c68-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c2c68-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

