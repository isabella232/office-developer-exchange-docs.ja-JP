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
description: SerializedSecurityContext 要素は、サーバーからサーバーへの認証でトークンのシリアル化に、Simple Object Access Protocol (SOAP) ヘッダーで使用されます。 トークンのシリアル化はサポートされていません。
ms.openlocfilehash: c5590551dc0780d918b05902e4f48fb9d1390b59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833363"
---
# <a name="serializedsecuritycontext"></a><span data-ttu-id="b1357-104">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="b1357-104">SerializedSecurityContext</span></span>

<span data-ttu-id="b1357-105">**SerializedSecurityContext**要素は、サーバーからサーバーへの認証でトークンのシリアル化に、Simple Object Access Protocol (SOAP) ヘッダーで使用されます。</span><span class="sxs-lookup"><span data-stu-id="b1357-105">The **SerializedSecurityContext** element is used in the Simple Object Access Protocol (SOAP) header for token serialization in server-to-server authentication.</span></span> <span data-ttu-id="b1357-106">トークンのシリアル化はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1357-106">Token serialization is not supported.</span></span> 
  
```xml
<SerializedSecurityContext>
   <UserSid/>
   <GroupSids/>
   <RestrictedGroupSids/>
   <PrimarySmtpAddress/>
</SerializedSecurityContext>
```

 <span data-ttu-id="b1357-107">**SerializedSecurityContextType**</span><span class="sxs-lookup"><span data-stu-id="b1357-107">**SerializedSecurityContextType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b1357-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b1357-108">Attributes and elements</span></span>

<span data-ttu-id="b1357-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b1357-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b1357-110">属性</span><span class="sxs-lookup"><span data-stu-id="b1357-110">Attributes</span></span>

<span data-ttu-id="b1357-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b1357-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b1357-112">子要素</span><span class="sxs-lookup"><span data-stu-id="b1357-112">Child elements</span></span>

|<span data-ttu-id="b1357-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b1357-113">**Element**</span></span>|<span data-ttu-id="b1357-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b1357-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b1357-115">UserSid</span><span class="sxs-lookup"><span data-stu-id="b1357-115">UserSid</span></span>](usersid.md) <br/> |<span data-ttu-id="b1357-116">セキュリティ記述子定義言語 (SDDL) 形式のシリアル化されたセキュリティ コンテキストの SOAP ヘッダーでユーザーのセキュリティ識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="b1357-116">Represents the security descriptor definition language (SDDL) form of the user security identifier in a serialized security context SOAP header.</span></span>  <br/> |
|[<span data-ttu-id="b1357-117">GroupSids</span><span class="sxs-lookup"><span data-stu-id="b1357-117">GroupSids</span></span>](groupsids.md) <br/> |<span data-ttu-id="b1357-118">Active Directory ディレクトリ サービス グループ オブジェクト セキュリティ識別子のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="b1357-118">Represents a collection of Active Directory directory service group object security identifiers.</span></span>  <br/> |
|[<span data-ttu-id="b1357-119">RestrictedGroupSids</span><span class="sxs-lookup"><span data-stu-id="b1357-119">RestrictedGroupSids</span></span>](restrictedgroupsids.md) <br/> |<span data-ttu-id="b1357-120">グループ セキュリティ識別子および制限されたグループの属性を表します。</span><span class="sxs-lookup"><span data-stu-id="b1357-120">Represents the group security identifier and attributes for a restricted group.</span></span>  <br/> |
|[<span data-ttu-id="b1357-121">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="b1357-121">PrimarySmtpAddress</span></span>](primarysmtpaddress.md) <br/> |<span data-ttu-id="b1357-122">サーバーからサーバーへの認証に使用するアカウントのプライマリ簡易メール転送プロトコル (SMTP) アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="b1357-122">Represents the primary Simple Mail Transfer Protocol (SMTP) address of an account to be used for server-to-server authorization.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b1357-123">親要素</span><span class="sxs-lookup"><span data-stu-id="b1357-123">Parent elements</span></span>

<span data-ttu-id="b1357-124">なし。</span><span class="sxs-lookup"><span data-stu-id="b1357-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b1357-125">備考</span><span class="sxs-lookup"><span data-stu-id="b1357-125">Remarks</span></span>

<span data-ttu-id="b1357-126">この要素を記述するスキーマは、クライアント アクセス サーバー (CAS) の役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b1357-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server (CAS) role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b1357-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="b1357-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b1357-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="b1357-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b1357-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b1357-129">Schema Name</span></span>  <br/> |<span data-ttu-id="b1357-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b1357-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="b1357-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b1357-131">Validation File</span></span>  <br/> |<span data-ttu-id="b1357-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b1357-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b1357-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b1357-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="b1357-134">False</span><span class="sxs-lookup"><span data-stu-id="b1357-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b1357-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="b1357-135">See also</span></span>



- [<span data-ttu-id="b1357-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b1357-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="b1357-137">EWS でのサーバーからサーバーへの承認</span><span class="sxs-lookup"><span data-stu-id="b1357-137">Server-to-server authorization in EWS</span></span>](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

