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
description: UserId 要素は、代理ユーザーまたはフォルダーのアクセス許可を持つユーザーを識別します。
ms.openlocfilehash: 68075e335383835ddce9575d85ba5fa945ed305c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455542"
---
# <a name="userid"></a><span data-ttu-id="6ed6b-103">UserId</span><span class="sxs-lookup"><span data-stu-id="6ed6b-103">UserId</span></span>

<span data-ttu-id="6ed6b-104">**UserId**要素は、代理ユーザーまたはフォルダーのアクセス許可を持つユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="6ed6b-104">The **UserId** element identifies a delegate user or a user who has folder access permissions.</span></span> 
  
```xml
<UserId>
   <SID/>
   <PrimarySmtpAddress/>
   <DisplayName/>
   <DistinguishedUser/>
   <ExternalUserIdentity/>
</UserId>
```

 <span data-ttu-id="6ed6b-105">**UserIdType**</span><span class="sxs-lookup"><span data-stu-id="6ed6b-105">**UserIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6ed6b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6ed6b-106">Attributes and elements</span></span>

<span data-ttu-id="6ed6b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6ed6b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6ed6b-108">属性</span><span class="sxs-lookup"><span data-stu-id="6ed6b-108">Attributes</span></span>

<span data-ttu-id="6ed6b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6ed6b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6ed6b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6ed6b-110">Child elements</span></span>

|<span data-ttu-id="6ed6b-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="6ed6b-111">**Element**</span></span>|<span data-ttu-id="6ed6b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6ed6b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6ed6b-113">SID</span><span class="sxs-lookup"><span data-stu-id="6ed6b-113">SID</span></span>](sid.md) <br/> |<span data-ttu-id="6ed6b-114">セキュリティ識別子 (SID) のセキュリティ記述子定義言語 (SDDL) 形式を表します。</span><span class="sxs-lookup"><span data-stu-id="6ed6b-114">Represents the security descriptor definition language (SDDL) form of the security identifier (SID).</span></span>  <br/> |
|[<span data-ttu-id="6ed6b-115">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="6ed6b-115">PrimarySmtpAddress</span></span>](primarysmtpaddress.md) <br/> |<span data-ttu-id="6ed6b-116">代理人アクセスに使用するアカウントのプライマリ簡易メール転送プロトコル (SMTP) アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="6ed6b-116">Represents the primary Simple Mail Transfer Protocol (SMTP) address of an account to be used for delegate access.</span></span>  <br/> |
|[<span data-ttu-id="6ed6b-117">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="6ed6b-117">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="6ed6b-118">フォルダー、連絡先、配布リスト、または代理人のユーザーの表示名を定義します。</span><span class="sxs-lookup"><span data-stu-id="6ed6b-118">Defines the display name of a folder, contact, distribution list, or delegate user.</span></span>  <br/> |
|[<span data-ttu-id="6ed6b-119">DistinguishedUser</span><span class="sxs-lookup"><span data-stu-id="6ed6b-119">DistinguishedUser</span></span>](distinguisheduser.md) <br/> |<span data-ttu-id="6ed6b-120">代理人アクセスの匿名および既定のユーザーアカウントを識別します。</span><span class="sxs-lookup"><span data-stu-id="6ed6b-120">Identifies Anonymous and Default user accounts for delegate access.</span></span>  <br/> |
|[<span data-ttu-id="6ed6b-121">ExternalUserIdentity</span><span class="sxs-lookup"><span data-stu-id="6ed6b-121">ExternalUserIdentity</span></span>](externaluseridentity.md) <br/> |<span data-ttu-id="6ed6b-122">外部代理ユーザーまたはフォルダーアクセス許可を持つ外部ユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="6ed6b-122">Identifies an external delegate user or an external user who has folder access permissions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6ed6b-123">親要素</span><span class="sxs-lookup"><span data-stu-id="6ed6b-123">Parent elements</span></span>

|<span data-ttu-id="6ed6b-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="6ed6b-124">**Element**</span></span>|<span data-ttu-id="6ed6b-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="6ed6b-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6ed6b-126">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="6ed6b-126">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="6ed6b-127">メールボックスに追加または更新する単一の代理人を指定します。</span><span class="sxs-lookup"><span data-stu-id="6ed6b-127">Identifies a single delegate to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6ed6b-128">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6ed6b-128">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="6ed6b-129">ユーザーがフォルダーに対して持つアクセス許可を定義します。</span><span class="sxs-lookup"><span data-stu-id="6ed6b-129">Defines the access that a user has to a folder.</span></span>  <br/> |
|[<span data-ttu-id="6ed6b-130">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="6ed6b-130">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="6ed6b-131">ユーザーが予定表フォルダーに対して持っているアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="6ed6b-131">Defines the access that a user has to a Calendar folder.</span></span>  <br/> |
|[<span data-ttu-id="6ed6b-132">UserIds</span><span class="sxs-lookup"><span data-stu-id="6ed6b-132">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="6ed6b-133">プリンシパルのメールボックスから取得または削除するデリゲートユーザーの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="6ed6b-133">Contains an array of delegate users to get or remove from a principal's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6ed6b-134">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6ed6b-134">Text value</span></span>

<span data-ttu-id="6ed6b-135">なし。</span><span class="sxs-lookup"><span data-stu-id="6ed6b-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6ed6b-136">注釈</span><span class="sxs-lookup"><span data-stu-id="6ed6b-136">Remarks</span></span>

<span data-ttu-id="6ed6b-137">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6ed6b-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6ed6b-138">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6ed6b-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6ed6b-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="6ed6b-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6ed6b-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6ed6b-140">Schema Name</span></span>  <br/> |<span data-ttu-id="6ed6b-141">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6ed6b-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="6ed6b-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6ed6b-142">Validation File</span></span>  <br/> |<span data-ttu-id="6ed6b-143">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6ed6b-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6ed6b-144">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6ed6b-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="6ed6b-145">正しくない</span><span class="sxs-lookup"><span data-stu-id="6ed6b-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6ed6b-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="6ed6b-146">See also</span></span>



[<span data-ttu-id="6ed6b-147">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="6ed6b-147">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="6ed6b-148">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="6ed6b-148">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="6ed6b-149">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6ed6b-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="6ed6b-150">代理人の追加</span><span class="sxs-lookup"><span data-stu-id="6ed6b-150">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

