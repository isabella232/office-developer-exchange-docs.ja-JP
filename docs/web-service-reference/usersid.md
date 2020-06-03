---
title: UserSid
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserSid
api_type:
- schema
ms.assetid: f8a0dcd9-8564-4e35-b307-c5d2761b48d8
description: UserSid 要素は、シリアル化されたセキュリティコンテキストの SOAP ヘッダー内のユーザーセキュリティ識別子のセキュリティ記述子定義言語 (SDDL) 形式を表します。 トークンのシリアル化はサポートされていません。
ms.openlocfilehash: b8ee51b1998546fc4ab14bd3666192ae63c8dba8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462018"
---
# <a name="usersid"></a><span data-ttu-id="d8bed-104">UserSid</span><span class="sxs-lookup"><span data-stu-id="d8bed-104">UserSid</span></span>

<span data-ttu-id="d8bed-105">**UserSid**要素は、シリアル化されたセキュリティコンテキストの SOAP ヘッダー内のユーザーセキュリティ識別子のセキュリティ記述子定義言語 (SDDL) 形式を表します。</span><span class="sxs-lookup"><span data-stu-id="d8bed-105">The **UserSid** element represents the security descriptor definition language (SDDL) form of the user security identifier in a serialized security context SOAP header.</span></span> <span data-ttu-id="d8bed-106">トークンのシリアル化はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8bed-106">Token serialization is not supported.</span></span> 
  
```xml
<UserSid/>
```

 <span data-ttu-id="d8bed-107">**String**</span><span class="sxs-lookup"><span data-stu-id="d8bed-107">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8bed-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d8bed-108">Attributes and elements</span></span>

<span data-ttu-id="d8bed-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d8bed-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8bed-110">属性</span><span class="sxs-lookup"><span data-stu-id="d8bed-110">Attributes</span></span>

<span data-ttu-id="d8bed-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d8bed-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8bed-112">子要素</span><span class="sxs-lookup"><span data-stu-id="d8bed-112">Child elements</span></span>

<span data-ttu-id="d8bed-113">なし。</span><span class="sxs-lookup"><span data-stu-id="d8bed-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d8bed-114">親要素</span><span class="sxs-lookup"><span data-stu-id="d8bed-114">Parent elements</span></span>

|<span data-ttu-id="d8bed-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="d8bed-115">**Element**</span></span>|<span data-ttu-id="d8bed-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="d8bed-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8bed-117">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="d8bed-117">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="d8bed-118">サーバー間認証のトークンシリアル化のために SOAP ヘッダーで使用されます。</span><span class="sxs-lookup"><span data-stu-id="d8bed-118">Used in the SOAP header for token serialization in server-to-server authentication.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d8bed-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d8bed-119">Text value</span></span>

<span data-ttu-id="d8bed-120">Text 値は、ユーザーのセキュリティ識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="d8bed-120">The text value represents a user's security identifier.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d8bed-121">注釈</span><span class="sxs-lookup"><span data-stu-id="d8bed-121">Remarks</span></span>

<span data-ttu-id="d8bed-122">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d8bed-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8bed-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d8bed-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8bed-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="d8bed-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d8bed-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d8bed-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d8bed-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d8bed-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="d8bed-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d8bed-127">Validation File</span></span>  <br/> |<span data-ttu-id="d8bed-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d8bed-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d8bed-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d8bed-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="d8bed-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="d8bed-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d8bed-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="d8bed-131">See also</span></span>



- [<span data-ttu-id="d8bed-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d8bed-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

