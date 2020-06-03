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
ms.openlocfilehash: c55e4a7f7f0b8f8a40e6fcaf8d18e253a6da2679
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468804"
---
# <a name="securityidentifier"></a><span data-ttu-id="f081e-103">SecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="f081e-103">SecurityIdentifier</span></span>

<span data-ttu-id="f081e-104">**SecurityIdentifier**要素は、セキュリティ識別子 ( [SID](sid.md)) のセキュリティ記述子定義言語 (SDDL) 形式を表します。</span><span class="sxs-lookup"><span data-stu-id="f081e-104">The **SecurityIdentifier** element represents the security descriptor definition language (SDDL) form of a security identifier ( [SID](sid.md)).</span></span>
  
```xml
<SecurityIdentifier/>
```

 <span data-ttu-id="f081e-105">**string**</span><span class="sxs-lookup"><span data-stu-id="f081e-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f081e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f081e-106">Attributes and elements</span></span>

<span data-ttu-id="f081e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f081e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f081e-108">属性</span><span class="sxs-lookup"><span data-stu-id="f081e-108">Attributes</span></span>

<span data-ttu-id="f081e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f081e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f081e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f081e-110">Child elements</span></span>

<span data-ttu-id="f081e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f081e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f081e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f081e-112">Parent elements</span></span>

|<span data-ttu-id="f081e-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="f081e-113">**Element**</span></span>|<span data-ttu-id="f081e-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f081e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f081e-115">GroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="f081e-115">GroupIdentifier</span></span>](groupidentifier.md) <br/> |<span data-ttu-id="f081e-116">アカウントがメンバーである Active Directory オブジェクトグループの単一のセキュリティ識別子と属性を表します。</span><span class="sxs-lookup"><span data-stu-id="f081e-116">Represents a single security identifier and attribute for an Active Directory object group of which the account is a member.</span></span>  <br/> <span data-ttu-id="f081e-117">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f081e-117">The following is the XPath expression to this element:</span></span>  <br/>  `/SerializedSecurityContext/GroupSids/GroupIdentifier[i]` <br/> |
|[<span data-ttu-id="f081e-118">RestrictedGroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="f081e-118">RestrictedGroupIdentifier</span></span>](restrictedgroupidentifier.md) <br/> |<span data-ttu-id="f081e-119">ユーザートークン内の制限されたグループのグループセキュリティ識別子と属性を表します。</span><span class="sxs-lookup"><span data-stu-id="f081e-119">Represents the group security identifier and attributes for a restricted group within a user token.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f081e-120">注釈</span><span class="sxs-lookup"><span data-stu-id="f081e-120">Remarks</span></span>

<span data-ttu-id="f081e-121">この要素は、Simple Object Access Protocol (SOAP) ヘッダーで使用されます。</span><span class="sxs-lookup"><span data-stu-id="f081e-121">This element is used in the Simple Object Access Protocol (SOAP) header.</span></span>
  
<span data-ttu-id="f081e-122">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="f081e-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f081e-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f081e-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f081e-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="f081e-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f081e-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f081e-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f081e-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f081e-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="f081e-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f081e-127">Validation File</span></span>  <br/> |<span data-ttu-id="f081e-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f081e-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f081e-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f081e-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="f081e-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="f081e-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f081e-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="f081e-131">See also</span></span>



- [<span data-ttu-id="f081e-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f081e-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

