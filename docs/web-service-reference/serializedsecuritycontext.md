---
title: SerializedSecurityContext
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SerializedSecurityContext
api_type:
- schema
ms.assetid: a02c4fc1-ed1a-40d9-a18e-6cfdae21a690
description: SerializedSecurityContext 要素は、サーバー間認証でトークンをシリアル化するための簡易オブジェクトアクセスプロトコル (SOAP) ヘッダーで使用されます。 トークンのシリアル化はサポートされていません。
ms.openlocfilehash: 58fea1c7f613315d59e81935561f92f318afc769
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462053"
---
# <a name="serializedsecuritycontext"></a><span data-ttu-id="8530f-104">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="8530f-104">SerializedSecurityContext</span></span>

<span data-ttu-id="8530f-105">**SerializedSecurityContext**要素は、サーバー間認証でトークンをシリアル化するための簡易オブジェクトアクセスプロトコル (SOAP) ヘッダーで使用されます。</span><span class="sxs-lookup"><span data-stu-id="8530f-105">The **SerializedSecurityContext** element is used in the Simple Object Access Protocol (SOAP) header for token serialization in server-to-server authentication.</span></span> <span data-ttu-id="8530f-106">トークンのシリアル化はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8530f-106">Token serialization is not supported.</span></span> 
  
```xml
<SerializedSecurityContext>
   <UserSid/>
   <GroupSids/>
   <RestrictedGroupSids/>
   <PrimarySmtpAddress/>
</SerializedSecurityContext>
```

 <span data-ttu-id="8530f-107">**SerializedSecurityContextType**</span><span class="sxs-lookup"><span data-stu-id="8530f-107">**SerializedSecurityContextType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8530f-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8530f-108">Attributes and elements</span></span>

<span data-ttu-id="8530f-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8530f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8530f-110">属性</span><span class="sxs-lookup"><span data-stu-id="8530f-110">Attributes</span></span>

<span data-ttu-id="8530f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8530f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8530f-112">子要素</span><span class="sxs-lookup"><span data-stu-id="8530f-112">Child elements</span></span>

|<span data-ttu-id="8530f-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="8530f-113">**Element**</span></span>|<span data-ttu-id="8530f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="8530f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8530f-115">UserSid</span><span class="sxs-lookup"><span data-stu-id="8530f-115">UserSid</span></span>](usersid.md) <br/> |<span data-ttu-id="8530f-116">シリアル化されたセキュリティコンテキストの SOAP ヘッダー内のユーザーセキュリティ識別子のセキュリティ記述子定義言語 (SDDL) 形式を表します。</span><span class="sxs-lookup"><span data-stu-id="8530f-116">Represents the security descriptor definition language (SDDL) form of the user security identifier in a serialized security context SOAP header.</span></span>  <br/> |
|[<span data-ttu-id="8530f-117">GroupSids</span><span class="sxs-lookup"><span data-stu-id="8530f-117">GroupSids</span></span>](groupsids.md) <br/> |<span data-ttu-id="8530f-118">Active Directory ディレクトリサービスグループオブジェクトのセキュリティ識別子のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="8530f-118">Represents a collection of Active Directory directory service group object security identifiers.</span></span>  <br/> |
|[<span data-ttu-id="8530f-119">RestrictedGroupSids</span><span class="sxs-lookup"><span data-stu-id="8530f-119">RestrictedGroupSids</span></span>](restrictedgroupsids.md) <br/> |<span data-ttu-id="8530f-120">制限されたグループのグループセキュリティ識別子と属性を表します。</span><span class="sxs-lookup"><span data-stu-id="8530f-120">Represents the group security identifier and attributes for a restricted group.</span></span>  <br/> |
|[<span data-ttu-id="8530f-121">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="8530f-121">PrimarySmtpAddress</span></span>](primarysmtpaddress.md) <br/> |<span data-ttu-id="8530f-122">サーバー間の認証に使用されるアカウントのプライマリ簡易メール転送プロトコル (SMTP) アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="8530f-122">Represents the primary Simple Mail Transfer Protocol (SMTP) address of an account to be used for server-to-server authorization.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8530f-123">親要素</span><span class="sxs-lookup"><span data-stu-id="8530f-123">Parent elements</span></span>

<span data-ttu-id="8530f-124">なし。</span><span class="sxs-lookup"><span data-stu-id="8530f-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8530f-125">注釈</span><span class="sxs-lookup"><span data-stu-id="8530f-125">Remarks</span></span>

<span data-ttu-id="8530f-126">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバー (CAS) の役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="8530f-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server (CAS) role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8530f-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8530f-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8530f-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="8530f-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8530f-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8530f-129">Schema Name</span></span>  <br/> |<span data-ttu-id="8530f-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="8530f-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="8530f-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8530f-131">Validation File</span></span>  <br/> |<span data-ttu-id="8530f-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="8530f-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8530f-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8530f-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="8530f-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="8530f-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8530f-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="8530f-135">See also</span></span>



- [<span data-ttu-id="8530f-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8530f-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="8530f-137">EWS でのサーバー間認証</span><span class="sxs-lookup"><span data-stu-id="8530f-137">Server-to-server authorization in EWS</span></span>](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

