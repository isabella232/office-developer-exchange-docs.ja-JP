---
title: ResolveNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNames
api_type:
- schema
ms.assetid: c85207e1-1315-443b-94ec-2b58f405076b
description: ResolveNames 要素は、あいまいな名前を解決する要求を定義します。
ms.openlocfilehash: 9c36a5f84451f91e90a8e7148cf384b5cacd7f29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467950"
---
# <a name="resolvenames"></a><span data-ttu-id="ef366-103">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="ef366-103">ResolveNames</span></span>

<span data-ttu-id="ef366-104">**ResolveNames**要素は、あいまいな名前を解決する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="ef366-104">The **ResolveNames** element defines a request to resolve ambiguous names.</span></span> 
  
```XML
<ResolveNames ReturnFullContactData="" SearchScope="" ContactDataShape="">
   <ParentFolderIds/>
   <UnresolvedEntry/>
</ResolveNames>
```

 <span data-ttu-id="ef366-105">**ResolveNamesType**</span><span class="sxs-lookup"><span data-stu-id="ef366-105">**ResolveNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ef366-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ef366-106">Attributes and elements</span></span>

<span data-ttu-id="ef366-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ef366-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ef366-108">属性</span><span class="sxs-lookup"><span data-stu-id="ef366-108">Attributes</span></span>

|<span data-ttu-id="ef366-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="ef366-109">**Attribute**</span></span>|<span data-ttu-id="ef366-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="ef366-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ef366-111">**ReturnFullContactData**</span><span class="sxs-lookup"><span data-stu-id="ef366-111">**ReturnFullContactData**</span></span> <br/> |<span data-ttu-id="ef366-112">解決された名前のパブリック連絡先の完全な連絡先の詳細を応答で返すかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ef366-112">Describes whether the full contact details for public contacts for a resolved name are returned in the response.</span></span> <span data-ttu-id="ef366-113">この属性は、パブリック連絡先に必要です。</span><span class="sxs-lookup"><span data-stu-id="ef366-113">This attribute is required for public contacts.</span></span> <span data-ttu-id="ef366-114">この値は、[ [ItemId](itemid.md) ] が常に返されるプライベート連絡先とプライベート配布リストには影響しません。</span><span class="sxs-lookup"><span data-stu-id="ef366-114">This value does not affect private contacts and private distribution lists, for which [ItemId](itemid.md) is always returned.</span></span>  <br/> |
|<span data-ttu-id="ef366-115">**SearchScope**</span><span class="sxs-lookup"><span data-stu-id="ef366-115">**SearchScope**</span></span> <br/> |<span data-ttu-id="ef366-116">ResolveNames 検索の順序と範囲を指定します。</span><span class="sxs-lookup"><span data-stu-id="ef366-116">Identifies the order and scope for a ResolveNames search.</span></span>  <br/> |
|<span data-ttu-id="ef366-117">ContactDataShape</span><span class="sxs-lookup"><span data-stu-id="ef366-117">ContactDataShape</span></span>  <br/> |<span data-ttu-id="ef366-118">連絡先に対して返されるプロパティセットを識別します。</span><span class="sxs-lookup"><span data-stu-id="ef366-118">Identifies the property set returned for contacts.</span></span> <span data-ttu-id="ef366-119">この属性は、Exchange Server 2010 Service Pack 2 (SP2) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ef366-119">This attribute was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>  <br/> |
   
#### <a name="returnfullcontactdata-attribute-values"></a><span data-ttu-id="ef366-120">ReturnFullContactData 属性値</span><span class="sxs-lookup"><span data-stu-id="ef366-120">ReturnFullContactData attribute values</span></span>

|<span data-ttu-id="ef366-121">**値**</span><span class="sxs-lookup"><span data-stu-id="ef366-121">**Value**</span></span>|<span data-ttu-id="ef366-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="ef366-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ef366-123">True</span><span class="sxs-lookup"><span data-stu-id="ef366-123">True</span></span>  <br/> |<span data-ttu-id="ef366-124">パブリック連絡先の完全な連絡先の詳細が返されます。</span><span class="sxs-lookup"><span data-stu-id="ef366-124">Full contact details for public contacts are returned.</span></span>  <br/> |
|<span data-ttu-id="ef366-125">正しくない</span><span class="sxs-lookup"><span data-stu-id="ef366-125">False</span></span>  <br/> |<span data-ttu-id="ef366-126">パブリック連絡先の完全な連絡先の詳細は返されません。</span><span class="sxs-lookup"><span data-stu-id="ef366-126">Full contact details for public contacts are not returned.</span></span>  <br/> |
   
#### <a name="searchscope-attribute-values"></a><span data-ttu-id="ef366-127">SearchScope 属性の値</span><span class="sxs-lookup"><span data-stu-id="ef366-127">SearchScope attribute values</span></span>

|<span data-ttu-id="ef366-128">**値**</span><span class="sxs-lookup"><span data-stu-id="ef366-128">**Value**</span></span>|<span data-ttu-id="ef366-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="ef366-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ef366-130">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="ef366-130">ActiveDirectory</span></span>  <br/> |<span data-ttu-id="ef366-131">Active Directory ディレクトリサービスのみが検索されます。</span><span class="sxs-lookup"><span data-stu-id="ef366-131">Only the Active Directory directory service is searched.</span></span>  <br/> |
|<span data-ttu-id="ef366-132">ActiveDirectoryContacts</span><span class="sxs-lookup"><span data-stu-id="ef366-132">ActiveDirectoryContacts</span></span>  <br/> |<span data-ttu-id="ef366-133">Active Directory が最初に検索され、 [ParentFolderIds](parentfolderids.md)プロパティに指定されている連絡先フォルダーが検索されます。</span><span class="sxs-lookup"><span data-stu-id="ef366-133">Active Directory is searched first, and then the contact folders that are specified in the [ParentFolderIds](parentfolderids.md) property are searched.</span></span>  <br/> |
|<span data-ttu-id="ef366-134">連絡先</span><span class="sxs-lookup"><span data-stu-id="ef366-134">Contacts</span></span>  <br/> |<span data-ttu-id="ef366-135">[ParentFolderIds](parentfolderids.md)プロパティによって識別される連絡先フォルダーのみが検索されます。</span><span class="sxs-lookup"><span data-stu-id="ef366-135">Only the contact folders that are identified by the [ParentFolderIds](parentfolderids.md) property are searched.</span></span>  <br/> |
|<span data-ttu-id="ef366-136">ContactsActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="ef366-136">ContactsActiveDirectory</span></span>  <br/> |<span data-ttu-id="ef366-137">[ParentFolderIds](parentfolderids.md)プロパティによって識別された連絡先フォルダーが最初に検索されてから、Active Directory が検索されます。</span><span class="sxs-lookup"><span data-stu-id="ef366-137">Contact folders that are identified by the [ParentFolderIds](parentfolderids.md) property are searched first and then Active Directory is searched.</span></span>  <br/> |
   
#### <a name="contactdatashape-attribute-values"></a><span data-ttu-id="ef366-138">ContactDataShape 属性の値</span><span class="sxs-lookup"><span data-stu-id="ef366-138">ContactDataShape attribute values</span></span>

|<span data-ttu-id="ef366-139">**値**</span><span class="sxs-lookup"><span data-stu-id="ef366-139">**Value**</span></span>|<span data-ttu-id="ef366-140">**説明**</span><span class="sxs-lookup"><span data-stu-id="ef366-140">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ef366-141">IdOnly</span><span class="sxs-lookup"><span data-stu-id="ef366-141">IdOnly</span></span>  <br/> |<span data-ttu-id="ef366-142">連絡先アイテムの識別子のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ef366-142">The contact item identifier property is returned.</span></span>  <br/> |
|<span data-ttu-id="ef366-143">既定</span><span class="sxs-lookup"><span data-stu-id="ef366-143">Default</span></span>  <br/> |<span data-ttu-id="ef366-144">連絡先アイテムのプロパティの既定のセットが返されます。</span><span class="sxs-lookup"><span data-stu-id="ef366-144">The Default set of contact item properties is returned.</span></span> <span data-ttu-id="ef366-145">詳細については、「 [EWS での応答の図形](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ef366-145">For more information, see [Response shapes in EWS](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span></span>  <br/> |
|<span data-ttu-id="ef366-146">AllProperties</span><span class="sxs-lookup"><span data-stu-id="ef366-146">AllProperties</span></span>  <br/> |<span data-ttu-id="ef366-147">連絡先アイテムのプロパティの AllProperties セットが返されます。</span><span class="sxs-lookup"><span data-stu-id="ef366-147">The AllProperties set of contact item properties are returned.</span></span> <span data-ttu-id="ef366-148">詳細については、「 [EWS での応答の図形](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ef366-148">For more information, see [Response shapes in EWS](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ef366-149">子要素</span><span class="sxs-lookup"><span data-stu-id="ef366-149">Child elements</span></span>

|<span data-ttu-id="ef366-150">**Element**</span><span class="sxs-lookup"><span data-stu-id="ef366-150">**Element**</span></span>|<span data-ttu-id="ef366-151">**説明**</span><span class="sxs-lookup"><span data-stu-id="ef366-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ef366-152">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="ef366-152">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="ef366-153">**Searchscope**属性が ActiveDirectoryContacts、Contacts、または ContactsActiveDirectory に設定されている場合に検索される連絡先フォルダーの識別子の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="ef366-153">Contains an array of contact folder identifiers that would be searched if the **SearchScope** attribute is set to ActiveDirectoryContacts, Contacts, or ContactsActiveDirectory.</span></span> <span data-ttu-id="ef366-154">ParentFolderIds 配列には、1つの連絡先フォルダーの識別子のみを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="ef366-154">The ParentFolderIds array can only contain a single contact folder identifier.</span></span> <span data-ttu-id="ef366-155">**ParentFolderIds**要素が存在しない場合は、既定の連絡先フォルダーが検索されます。</span><span class="sxs-lookup"><span data-stu-id="ef366-155">If the **ParentFolderIds** element is not present, the default Contacts folder is searched.</span></span>  <br/> <span data-ttu-id="ef366-156">代理人アクセスには、フォルダー識別子を使用できます。</span><span class="sxs-lookup"><span data-stu-id="ef366-156">The folder identifier can be used for delegate access.</span></span>  <br/> <span data-ttu-id="ef366-157">Active Directory 検索は、アクセス制御リスト (Acl) を使用して実行されます。</span><span class="sxs-lookup"><span data-stu-id="ef366-157">Active Directory searches are performed by using access control lists (ACLs).</span></span> <span data-ttu-id="ef366-158">一部のユーザーは、一部の Active Directory オブジェクトを表示する権限を持っていない場合があります。</span><span class="sxs-lookup"><span data-stu-id="ef366-158">Some users might not have the rights to see some Active Directory objects.</span></span>  <br/> <span data-ttu-id="ef366-159">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="ef366-159">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ef366-160">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="ef366-160">UnresolvedEntry</span></span>](unresolvedentry.md) <br/> |<span data-ttu-id="ef366-161">解決する連絡先または配布リストの名前を格納します。</span><span class="sxs-lookup"><span data-stu-id="ef366-161">Contains the name of a contact or distribution list to resolve.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ef366-162">親要素</span><span class="sxs-lookup"><span data-stu-id="ef366-162">Parent elements</span></span>

<span data-ttu-id="ef366-163">なし。</span><span class="sxs-lookup"><span data-stu-id="ef366-163">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ef366-164">注釈</span><span class="sxs-lookup"><span data-stu-id="ef366-164">Remarks</span></span>

<span data-ttu-id="ef366-165">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ef366-165">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ef366-166">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ef366-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ef366-167">Namespace</span><span class="sxs-lookup"><span data-stu-id="ef366-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ef366-168">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ef366-168">Schema name</span></span>  <br/> |<span data-ttu-id="ef366-169">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="ef366-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ef366-170">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ef366-170">Validation file</span></span>  <br/> |<span data-ttu-id="ef366-171">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="ef366-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ef366-172">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ef366-172">Can be empty</span></span>  <br/> |<span data-ttu-id="ef366-173">正しくない</span><span class="sxs-lookup"><span data-stu-id="ef366-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ef366-174">関連項目</span><span class="sxs-lookup"><span data-stu-id="ef366-174">See also</span></span>



[<span data-ttu-id="ef366-175">ResolveNames 操作</span><span class="sxs-lookup"><span data-stu-id="ef366-175">ResolveNames operation</span></span>](resolvenames-operation.md)
  
[<span data-ttu-id="ef366-176">ResolveNamesType</span><span class="sxs-lookup"><span data-stu-id="ef366-176">ResolveNamesType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesType.aspx)
  
[<span data-ttu-id="ef366-177">ResolveNamesSearchScopeType</span><span class="sxs-lookup"><span data-stu-id="ef366-177">ResolveNamesSearchScopeType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesSearchScopeType.aspx)


- [<span data-ttu-id="ef366-178">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ef366-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="ef366-179">名前解決の使用</span><span class="sxs-lookup"><span data-stu-id="ef366-179">Using Name Resolution</span></span>](https://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

