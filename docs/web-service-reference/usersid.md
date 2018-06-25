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
description: UserSid 要素は、セキュリティ記述子定義言語 (SDDL) 形式のシリアル化されたセキュリティ コンテキストの SOAP ヘッダーでユーザーのセキュリティ識別子を表します。 トークンのシリアル化はサポートされていません。
ms.openlocfilehash: 3c72f68638f99a4ee5081517027f0834ebf65b49
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839956"
---
# <a name="usersid"></a><span data-ttu-id="febb1-104">UserSid</span><span class="sxs-lookup"><span data-stu-id="febb1-104">UserSid</span></span>

<span data-ttu-id="febb1-105">**UserSid**要素は、セキュリティ記述子定義言語 (SDDL) 形式のシリアル化されたセキュリティ コンテキストの SOAP ヘッダーでユーザーのセキュリティ識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="febb1-105">The **UserSid** element represents the security descriptor definition language (SDDL) form of the user security identifier in a serialized security context SOAP header.</span></span> <span data-ttu-id="febb1-106">トークンのシリアル化はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="febb1-106">Token serialization is not supported.</span></span> 
  
```xml
<UserSid/>
```

 <span data-ttu-id="febb1-107">**文字列型 (String)**</span><span class="sxs-lookup"><span data-stu-id="febb1-107">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="febb1-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="febb1-108">Attributes and elements</span></span>

<span data-ttu-id="febb1-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="febb1-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="febb1-110">属性</span><span class="sxs-lookup"><span data-stu-id="febb1-110">Attributes</span></span>

<span data-ttu-id="febb1-111">なし。</span><span class="sxs-lookup"><span data-stu-id="febb1-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="febb1-112">子要素</span><span class="sxs-lookup"><span data-stu-id="febb1-112">Child elements</span></span>

<span data-ttu-id="febb1-113">なし。</span><span class="sxs-lookup"><span data-stu-id="febb1-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="febb1-114">親要素</span><span class="sxs-lookup"><span data-stu-id="febb1-114">Parent elements</span></span>

|<span data-ttu-id="febb1-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="febb1-115">**Element**</span></span>|<span data-ttu-id="febb1-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="febb1-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="febb1-117">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="febb1-117">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="febb1-118">サーバー間認証でトークンのシリアル化を SOAP ヘッダーで使用されます。</span><span class="sxs-lookup"><span data-stu-id="febb1-118">Used in the SOAP header for token serialization in server-to-server authentication.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="febb1-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="febb1-119">Text value</span></span>

<span data-ttu-id="febb1-120">テキスト値は、ユーザーのセキュリティ識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="febb1-120">The text value represents a user's security identifier.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="febb1-121">備考</span><span class="sxs-lookup"><span data-stu-id="febb1-121">Remarks</span></span>

<span data-ttu-id="febb1-122">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="febb1-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="febb1-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="febb1-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="febb1-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="febb1-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="febb1-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="febb1-125">Schema Name</span></span>  <br/> |<span data-ttu-id="febb1-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="febb1-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="febb1-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="febb1-127">Validation File</span></span>  <br/> |<span data-ttu-id="febb1-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="febb1-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="febb1-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="febb1-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="febb1-130">False</span><span class="sxs-lookup"><span data-stu-id="febb1-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="febb1-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="febb1-131">See also</span></span>



- [<span data-ttu-id="febb1-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="febb1-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

