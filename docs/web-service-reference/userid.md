---
title: UserId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserId
api_type:
- schema
ms.assetid: 244af9e0-bf3c-46b4-8bfa-9719a1ed3107
description: ユーザー Id 要素は、代理ユーザー、またはフォルダーのアクセス許可を持つユーザーを識別します。
ms.openlocfilehash: 8e9867f5a8cdd62dd2dae55fbf527595ac14f46d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839933"
---
# <a name="userid"></a><span data-ttu-id="8d8e5-103">UserId</span><span class="sxs-lookup"><span data-stu-id="8d8e5-103">UserId</span></span>

<span data-ttu-id="8d8e5-104">**ユーザー Id**要素は、代理ユーザー、またはフォルダーのアクセス許可を持つユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="8d8e5-104">The **UserId** element identifies a delegate user or a user who has folder access permissions.</span></span> 
  
```xml
<UserId>
   <SID/>
   <PrimarySmtpAddress/>
   <DisplayName/>
   <DistinguishedUser/>
   <ExternalUserIdentity/>
</UserId>
```

 <span data-ttu-id="8d8e5-105">**UserIdType**</span><span class="sxs-lookup"><span data-stu-id="8d8e5-105">**UserIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8d8e5-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8d8e5-106">Attributes and elements</span></span>

<span data-ttu-id="8d8e5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8d8e5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d8e5-108">属性</span><span class="sxs-lookup"><span data-stu-id="8d8e5-108">Attributes</span></span>

<span data-ttu-id="8d8e5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8d8e5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8d8e5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8d8e5-110">Child elements</span></span>

|<span data-ttu-id="8d8e5-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="8d8e5-111">**Element**</span></span>|<span data-ttu-id="8d8e5-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="8d8e5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d8e5-113">SID</span><span class="sxs-lookup"><span data-stu-id="8d8e5-113">SID</span></span>](sid.md) <br/> |<span data-ttu-id="8d8e5-114">セキュリティ識別子 (SID) のセキュリティ記述子定義言語 (SDDL) 形式を表します。</span><span class="sxs-lookup"><span data-stu-id="8d8e5-114">Represents the security descriptor definition language (SDDL) form of the security identifier (SID).</span></span>  <br/> |
|[<span data-ttu-id="8d8e5-115">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="8d8e5-115">PrimarySmtpAddress</span></span>](primarysmtpaddress.md) <br/> |<span data-ttu-id="8d8e5-116">代理人アクセスに使用するアカウントのプライマリ簡易メール転送プロトコル (SMTP) アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="8d8e5-116">Represents the primary Simple Mail Transfer Protocol (SMTP) address of an account to be used for delegate access.</span></span>  <br/> |
|[<span data-ttu-id="8d8e5-117">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="8d8e5-117">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="8d8e5-118">フォルダー、連絡先、配布リスト、または代理ユーザーの表示名を定義します。</span><span class="sxs-lookup"><span data-stu-id="8d8e5-118">Defines the display name of a folder, contact, distribution list, or delegate user.</span></span>  <br/> |
|[<span data-ttu-id="8d8e5-119">DistinguishedUser</span><span class="sxs-lookup"><span data-stu-id="8d8e5-119">DistinguishedUser</span></span>](distinguisheduser.md) <br/> |<span data-ttu-id="8d8e5-120">代理人アクセスの認証と既定のユーザー アカウントを識別します。</span><span class="sxs-lookup"><span data-stu-id="8d8e5-120">Identifies Anonymous and Default user accounts for delegate access.</span></span>  <br/> |
|[<span data-ttu-id="8d8e5-121">ExternalUserIdentity</span><span class="sxs-lookup"><span data-stu-id="8d8e5-121">ExternalUserIdentity</span></span>](externaluseridentity.md) <br/> |<span data-ttu-id="8d8e5-122">フォルダーのアクセス許可を持つ外部ユーザー、外部の代理人のユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="8d8e5-122">Identifies an external delegate user or an external user who has folder access permissions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8d8e5-123">親要素</span><span class="sxs-lookup"><span data-stu-id="8d8e5-123">Parent elements</span></span>

|<span data-ttu-id="8d8e5-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="8d8e5-124">**Element**</span></span>|<span data-ttu-id="8d8e5-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="8d8e5-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d8e5-126">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="8d8e5-126">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="8d8e5-127">1 つのデリゲートを追加するメールボックスの更新を識別します。</span><span class="sxs-lookup"><span data-stu-id="8d8e5-127">Identifies a single delegate to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8d8e5-128">Permission</span><span class="sxs-lookup"><span data-stu-id="8d8e5-128">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="8d8e5-129">フォルダーにユーザーが持つアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="8d8e5-129">Defines the access that a user has to a folder.</span></span>  <br/> |
|[<span data-ttu-id="8d8e5-130">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="8d8e5-130">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="8d8e5-131">予定表フォルダーにユーザーが持つアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="8d8e5-131">Defines the access that a user has to a Calendar folder.</span></span>  <br/> |
|[<span data-ttu-id="8d8e5-132">ユーザー Id</span><span class="sxs-lookup"><span data-stu-id="8d8e5-132">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="8d8e5-133">取得またはプリンシパルのメールボックスから削除する代理人のユーザーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8d8e5-133">Contains an array of delegate users to get or remove from a principal's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8d8e5-134">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8d8e5-134">Text value</span></span>

<span data-ttu-id="8d8e5-135">なし。</span><span class="sxs-lookup"><span data-stu-id="8d8e5-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8d8e5-136">備考</span><span class="sxs-lookup"><span data-stu-id="8d8e5-136">Remarks</span></span>

<span data-ttu-id="8d8e5-137">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8d8e5-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8d8e5-138">要素情報</span><span class="sxs-lookup"><span data-stu-id="8d8e5-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8d8e5-139">名前空間</span><span class="sxs-lookup"><span data-stu-id="8d8e5-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8d8e5-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8d8e5-140">Schema Name</span></span>  <br/> |<span data-ttu-id="8d8e5-141">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8d8e5-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="8d8e5-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8d8e5-142">Validation File</span></span>  <br/> |<span data-ttu-id="8d8e5-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8d8e5-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8d8e5-144">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8d8e5-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="8d8e5-145">False</span><span class="sxs-lookup"><span data-stu-id="8d8e5-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8d8e5-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="8d8e5-146">See also</span></span>



[<span data-ttu-id="8d8e5-147">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="8d8e5-147">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="8d8e5-148">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="8d8e5-148">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="8d8e5-149">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="8d8e5-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="8d8e5-150">デリゲートを追加します。</span><span class="sxs-lookup"><span data-stu-id="8d8e5-150">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

