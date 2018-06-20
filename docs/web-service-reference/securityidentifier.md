---
title: SecurityIdentifier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SecurityIdentifier
api_type:
- schema
ms.assetid: f7656729-f2c9-41cc-b1ec-60f480fc4dab
description: SecurityIdentifier 要素は、セキュリティ識別子 (SID) のセキュリティ記述子定義言語 (SDDL) 形式を表します。
ms.openlocfilehash: c18d7d4505c618792497c32c7499eab9ac82989e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833314"
---
# <a name="securityidentifier"></a><span data-ttu-id="83dfd-103">SecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="83dfd-103">SecurityIdentifier</span></span>

<span data-ttu-id="83dfd-104">**SecurityIdentifier**要素は、セキュリティ識別子 ( [SID](sid.md)) のセキュリティ記述子定義言語 (SDDL) 形式を表します。</span><span class="sxs-lookup"><span data-stu-id="83dfd-104">The **SecurityIdentifier** element represents the security descriptor definition language (SDDL) form of a security identifier ( [SID](sid.md)).</span></span>
  
```xml
<SecurityIdentifier/>
```

 <span data-ttu-id="83dfd-105">**string**</span><span class="sxs-lookup"><span data-stu-id="83dfd-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="83dfd-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="83dfd-106">Attributes and elements</span></span>

<span data-ttu-id="83dfd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="83dfd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="83dfd-108">属性</span><span class="sxs-lookup"><span data-stu-id="83dfd-108">Attributes</span></span>

<span data-ttu-id="83dfd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="83dfd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="83dfd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="83dfd-110">Child elements</span></span>

<span data-ttu-id="83dfd-111">なし。</span><span class="sxs-lookup"><span data-stu-id="83dfd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="83dfd-112">親要素</span><span class="sxs-lookup"><span data-stu-id="83dfd-112">Parent elements</span></span>

|<span data-ttu-id="83dfd-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="83dfd-113">**Element**</span></span>|<span data-ttu-id="83dfd-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="83dfd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="83dfd-115">GroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="83dfd-115">GroupIdentifier</span></span>](groupidentifier.md) <br/> |<span data-ttu-id="83dfd-116">1 つのセキュリティ識別子と、アカウントがメンバーである Active Directory オブジェクト グループの属性を表します。</span><span class="sxs-lookup"><span data-stu-id="83dfd-116">Represents a single security identifier and attribute for an Active Directory object group of which the account is a member.</span></span>  <br/> <span data-ttu-id="83dfd-117">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="83dfd-117">The following is the XPath expression to this element:</span></span>  <br/>  `/SerializedSecurityContext/GroupSids/GroupIdentifier[i]` <br/> |
|[<span data-ttu-id="83dfd-118">RestrictedGroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="83dfd-118">RestrictedGroupIdentifier</span></span>](restrictedgroupidentifier.md) <br/> |<span data-ttu-id="83dfd-119">グループのセキュリティ識別子とユーザーのトークン内の制限されたグループの属性を表します。</span><span class="sxs-lookup"><span data-stu-id="83dfd-119">Represents the group security identifier and attributes for a restricted group within a user token.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="83dfd-120">備考</span><span class="sxs-lookup"><span data-stu-id="83dfd-120">Remarks</span></span>

<span data-ttu-id="83dfd-121">Simple Object Access Protocol (SOAP) ヘッダーには、この要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="83dfd-121">This element is used in the Simple Object Access Protocol (SOAP) header.</span></span>
  
<span data-ttu-id="83dfd-122">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="83dfd-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="83dfd-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="83dfd-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="83dfd-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="83dfd-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="83dfd-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="83dfd-125">Schema Name</span></span>  <br/> |<span data-ttu-id="83dfd-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="83dfd-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="83dfd-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="83dfd-127">Validation File</span></span>  <br/> |<span data-ttu-id="83dfd-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="83dfd-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="83dfd-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="83dfd-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="83dfd-130">False</span><span class="sxs-lookup"><span data-stu-id="83dfd-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="83dfd-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="83dfd-131">See also</span></span>



- [<span data-ttu-id="83dfd-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="83dfd-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

