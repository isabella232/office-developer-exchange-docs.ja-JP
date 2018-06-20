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
description: ResolveNames 要素では、あいまいな名前を解決する要求を定義します。
ms.openlocfilehash: e97b6e78d99cf8ffa3d680907916882d40963f59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833172"
---
# <a name="resolvenames"></a><span data-ttu-id="32291-103">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="32291-103">ResolveNames</span></span>

<span data-ttu-id="32291-104">**ResolveNames**要素では、あいまいな名前を解決する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="32291-104">The **ResolveNames** element defines a request to resolve ambiguous names.</span></span> 
  
```XML
<ResolveNames ReturnFullContactData="" SearchScope="" ContactDataShape="">
   <ParentFolderIds/>
   <UnresolvedEntry/>
</ResolveNames>
```

 <span data-ttu-id="32291-105">**ResolveNamesType**</span><span class="sxs-lookup"><span data-stu-id="32291-105">**ResolveNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="32291-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="32291-106">Attributes and elements</span></span>

<span data-ttu-id="32291-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="32291-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="32291-108">属性</span><span class="sxs-lookup"><span data-stu-id="32291-108">Attributes</span></span>

|<span data-ttu-id="32291-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="32291-109">**Attribute**</span></span>|<span data-ttu-id="32291-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="32291-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="32291-111">**ReturnFullContactData**</span><span class="sxs-lookup"><span data-stu-id="32291-111">**ReturnFullContactData**</span></span> <br/> |<span data-ttu-id="32291-112">解決された名前の公開アドレス帳の完全な連絡先の詳細が応答で返されるかどうかについて説明します。</span><span class="sxs-lookup"><span data-stu-id="32291-112">Describes whether the full contact details for public contacts for a resolved name are returned in the response.</span></span> <span data-ttu-id="32291-113">この属性は、パブリック メンバーに必要です。</span><span class="sxs-lookup"><span data-stu-id="32291-113">This attribute is required for public contacts.</span></span> <span data-ttu-id="32291-114">この値は、プライベートの連絡先と個人用配布リスト、[アイテム Id](itemid.md)が常に返されるには影響しません。</span><span class="sxs-lookup"><span data-stu-id="32291-114">This value does not affect private contacts and private distribution lists, for which [ItemId](itemid.md) is always returned.</span></span>  <br/> |
|<span data-ttu-id="32291-115">**SearchScope**</span><span class="sxs-lookup"><span data-stu-id="32291-115">**SearchScope**</span></span> <br/> |<span data-ttu-id="32291-116">ResolveNames 検索範囲の順序を識別します。</span><span class="sxs-lookup"><span data-stu-id="32291-116">Identifies the order and scope for a ResolveNames search.</span></span>  <br/> |
|<span data-ttu-id="32291-117">ContactDataShape</span><span class="sxs-lookup"><span data-stu-id="32291-117">ContactDataShape</span></span>  <br/> |<span data-ttu-id="32291-118">連絡先に対して返されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="32291-118">Identifies the property set returned for contacts.</span></span> <span data-ttu-id="32291-119">この属性は、Exchange Server 2010 のサービス パック 2 (SP2) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="32291-119">This attribute was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>  <br/> |
   
#### <a name="returnfullcontactdata-attribute-values"></a><span data-ttu-id="32291-120">ReturnFullContactData 属性の値</span><span class="sxs-lookup"><span data-stu-id="32291-120">ReturnFullContactData attribute values</span></span>

|<span data-ttu-id="32291-121">**値**</span><span class="sxs-lookup"><span data-stu-id="32291-121">**Value**</span></span>|<span data-ttu-id="32291-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="32291-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="32291-123">True</span><span class="sxs-lookup"><span data-stu-id="32291-123">True</span></span>  <br/> |<span data-ttu-id="32291-124">公開アドレス帳の完全な連絡先の詳細情報が返されます。</span><span class="sxs-lookup"><span data-stu-id="32291-124">Full contact details for public contacts are returned.</span></span>  <br/> |
|<span data-ttu-id="32291-125">False</span><span class="sxs-lookup"><span data-stu-id="32291-125">False</span></span>  <br/> |<span data-ttu-id="32291-126">公開アドレス帳の完全な連絡先の詳細情報は返されません。</span><span class="sxs-lookup"><span data-stu-id="32291-126">Full contact details for public contacts are not returned.</span></span>  <br/> |
   
#### <a name="searchscope-attribute-values"></a><span data-ttu-id="32291-127">SearchScope 属性の値</span><span class="sxs-lookup"><span data-stu-id="32291-127">SearchScope attribute values</span></span>

|<span data-ttu-id="32291-128">**値**</span><span class="sxs-lookup"><span data-stu-id="32291-128">**Value**</span></span>|<span data-ttu-id="32291-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="32291-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="32291-130">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="32291-130">ActiveDirectory</span></span>  <br/> |<span data-ttu-id="32291-131">Active Directory ディレクトリ サービスのみが検索されます。</span><span class="sxs-lookup"><span data-stu-id="32291-131">Only the Active Directory directory service is searched.</span></span>  <br/> |
|<span data-ttu-id="32291-132">ActiveDirectoryContacts</span><span class="sxs-lookup"><span data-stu-id="32291-132">ActiveDirectoryContacts</span></span>  <br/> |<span data-ttu-id="32291-133">最初に active Directory を検索し、 [ParentFolderIds](parentfolderids.md)プロパティで指定されている連絡先フォルダーを検索し、します。</span><span class="sxs-lookup"><span data-stu-id="32291-133">Active Directory is searched first, and then the contact folders that are specified in the [ParentFolderIds](parentfolderids.md) property are searched.</span></span>  <br/> |
|<span data-ttu-id="32291-134">連絡先</span><span class="sxs-lookup"><span data-stu-id="32291-134">Contacts</span></span>  <br/> |<span data-ttu-id="32291-135">[ParentFolderIds](parentfolderids.md)プロパティによって指定されている連絡先フォルダーのみが検索されます。</span><span class="sxs-lookup"><span data-stu-id="32291-135">Only the contact folders that are identified by the [ParentFolderIds](parentfolderids.md) property are searched.</span></span>  <br/> |
|<span data-ttu-id="32291-136">ContactsActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="32291-136">ContactsActiveDirectory</span></span>  <br/> |<span data-ttu-id="32291-137">[ParentFolderIds](parentfolderids.md)プロパティによって指定されている連絡先フォルダーを最初に検索され、Active Directory を検索します。</span><span class="sxs-lookup"><span data-stu-id="32291-137">Contact folders that are identified by the [ParentFolderIds](parentfolderids.md) property are searched first and then Active Directory is searched.</span></span>  <br/> |
   
#### <a name="contactdatashape-attribute-values"></a><span data-ttu-id="32291-138">ContactDataShape 属性の値</span><span class="sxs-lookup"><span data-stu-id="32291-138">ContactDataShape attribute values</span></span>

|<span data-ttu-id="32291-139">**値**</span><span class="sxs-lookup"><span data-stu-id="32291-139">**Value**</span></span>|<span data-ttu-id="32291-140">**説明**</span><span class="sxs-lookup"><span data-stu-id="32291-140">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="32291-141">IdOnly</span><span class="sxs-lookup"><span data-stu-id="32291-141">IdOnly</span></span>  <br/> |<span data-ttu-id="32291-142">連絡先アイテムの id プロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="32291-142">The contact item identifier property is returned.</span></span>  <br/> |
|<span data-ttu-id="32291-143">Default</span><span class="sxs-lookup"><span data-stu-id="32291-143">Default</span></span>  <br/> |<span data-ttu-id="32291-144">連絡先アイテムのプロパティの既定のセットが返されます。</span><span class="sxs-lookup"><span data-stu-id="32291-144">The Default set of contact item properties is returned.</span></span> <span data-ttu-id="32291-145">詳細については、 [EWS の避難用図形](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32291-145">For more information, see [Response shapes in EWS](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span></span>  <br/> |
|<span data-ttu-id="32291-146">AllProperties</span><span class="sxs-lookup"><span data-stu-id="32291-146">AllProperties</span></span>  <br/> |<span data-ttu-id="32291-147">連絡先アイテムのプロパティの AllProperties のセットが返されます。</span><span class="sxs-lookup"><span data-stu-id="32291-147">The AllProperties set of contact item properties are returned.</span></span> <span data-ttu-id="32291-148">詳細については、 [EWS の避難用図形](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32291-148">For more information, see [Response shapes in EWS](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="32291-149">子要素</span><span class="sxs-lookup"><span data-stu-id="32291-149">Child elements</span></span>

|<span data-ttu-id="32291-150">**要素**</span><span class="sxs-lookup"><span data-stu-id="32291-150">**Element**</span></span>|<span data-ttu-id="32291-151">**説明**</span><span class="sxs-lookup"><span data-stu-id="32291-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32291-152">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="32291-152">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="32291-153">**SearchScope**属性は、ActiveDirectoryContacts、連絡先、または ContactsActiveDirectory に設定されている場合を検索する連絡先フォルダー識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="32291-153">Contains an array of contact folder identifiers that would be searched if the **SearchScope** attribute is set to ActiveDirectoryContacts, Contacts, or ContactsActiveDirectory.</span></span> <span data-ttu-id="32291-154">ParentFolderIds アレイでは、1 つの連絡先フォルダーの識別子を含めることができますのみです。</span><span class="sxs-lookup"><span data-stu-id="32291-154">The ParentFolderIds array can only contain a single contact folder identifier.</span></span> <span data-ttu-id="32291-155">**ParentFolderIds**要素が存在しない場合は、既定の連絡先フォルダーが検索されます。</span><span class="sxs-lookup"><span data-stu-id="32291-155">If the **ParentFolderIds** element is not present, the default Contacts folder is searched.</span></span>  <br/> <span data-ttu-id="32291-156">フォルダーの識別子は、代理人アクセスを使用できます。</span><span class="sxs-lookup"><span data-stu-id="32291-156">The folder identifier can be used for delegate access.</span></span>  <br/> <span data-ttu-id="32291-157">作業中のディレクトリ検索は、アクセス制御リスト (Acl) を使用して実行されます。</span><span class="sxs-lookup"><span data-stu-id="32291-157">Active Directory searches are performed by using access control lists (ACLs).</span></span> <span data-ttu-id="32291-158">一部のユーザーは、いくつかの Active Directory オブジェクトを表示する権限をいない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="32291-158">Some users might not have the rights to see some Active Directory objects.</span></span>  <br/> <span data-ttu-id="32291-159">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="32291-159">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="32291-160">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="32291-160">UnresolvedEntry</span></span>](unresolvedentry.md) <br/> |<span data-ttu-id="32291-161">解決するのには、連絡先または配布リストの名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="32291-161">Contains the name of a contact or distribution list to resolve.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="32291-162">親要素</span><span class="sxs-lookup"><span data-stu-id="32291-162">Parent elements</span></span>

<span data-ttu-id="32291-163">なし。</span><span class="sxs-lookup"><span data-stu-id="32291-163">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="32291-164">備考</span><span class="sxs-lookup"><span data-stu-id="32291-164">Remarks</span></span>

<span data-ttu-id="32291-165">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="32291-165">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="32291-166">要素情報</span><span class="sxs-lookup"><span data-stu-id="32291-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32291-167">名前空間</span><span class="sxs-lookup"><span data-stu-id="32291-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="32291-168">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="32291-168">Schema name</span></span>  <br/> |<span data-ttu-id="32291-169">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="32291-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="32291-170">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="32291-170">Validation file</span></span>  <br/> |<span data-ttu-id="32291-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="32291-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="32291-172">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="32291-172">Can be empty</span></span>  <br/> |<span data-ttu-id="32291-173">False</span><span class="sxs-lookup"><span data-stu-id="32291-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="32291-174">関連項目</span><span class="sxs-lookup"><span data-stu-id="32291-174">See also</span></span>



[<span data-ttu-id="32291-175">ResolveNames 操作</span><span class="sxs-lookup"><span data-stu-id="32291-175">ResolveNames operation</span></span>](resolvenames-operation.md)
  
[<span data-ttu-id="32291-176">ResolveNamesType</span><span class="sxs-lookup"><span data-stu-id="32291-176">ResolveNamesType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesType.aspx)
  
[<span data-ttu-id="32291-177">ResolveNamesSearchScopeType</span><span class="sxs-lookup"><span data-stu-id="32291-177">ResolveNamesSearchScopeType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesSearchScopeType.aspx)


- [<span data-ttu-id="32291-178">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="32291-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="32291-179">名前解決の使用</span><span class="sxs-lookup"><span data-stu-id="32291-179">Using Name Resolution</span></span>](http://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

