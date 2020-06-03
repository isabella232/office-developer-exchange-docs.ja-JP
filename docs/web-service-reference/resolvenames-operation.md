---
title: ResolveNames 操作
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
ms.assetid: 6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb
description: ResolveNames 操作は、あいまいな電子メールアドレスと表示名を解決します。
ms.openlocfilehash: 51728addddd2bfb9d35b874ae8c11e83a4c8629b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468279"
---
# <a name="resolvenames-operation"></a><span data-ttu-id="3830b-103">ResolveNames 操作</span><span class="sxs-lookup"><span data-stu-id="3830b-103">ResolveNames operation</span></span>

<span data-ttu-id="3830b-104">**ResolveNames**操作は、あいまいな電子メールアドレスと表示名を解決します。</span><span class="sxs-lookup"><span data-stu-id="3830b-104">The **ResolveNames** operation resolves ambiguous email addresses and display names.</span></span> 
  
## <a name="using-the-resolvenames-operation"></a><span data-ttu-id="3830b-105">ResolveNames 操作の使用</span><span class="sxs-lookup"><span data-stu-id="3830b-105">Using the ResolveNames operation</span></span>

<span data-ttu-id="3830b-106">この操作は、エイリアスを確認し、表示名を適切なメールボックスユーザーに解決するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="3830b-106">This operation can be used to verify aliases and resolve display names to the appropriate mailbox user.</span></span> <span data-ttu-id="3830b-107">あいまいな名前が存在する場合、 **ResolveNames**操作の応答は、クライアントアプリケーションが名前を解決できるように、各メールボックスユーザーに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="3830b-107">If ambiguous names exist, the **ResolveNames** operation response provides information about each mailbox user so that the client application can resolve the names.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3830b-108">注釈</span><span class="sxs-lookup"><span data-stu-id="3830b-108">Remarks</span></span>

<span data-ttu-id="3830b-109">ResolveNames 応答は、最大100の候補を返します。</span><span class="sxs-lookup"><span data-stu-id="3830b-109">The ResolveNames response returns a maximum of 100 candidates.</span></span> <span data-ttu-id="3830b-110">返される100候補は、参照操作で検出された最初の100です。</span><span class="sxs-lookup"><span data-stu-id="3830b-110">The 100 candidates that are returned are the first 100 that are encountered in the lookup operation.</span></span>
  
<span data-ttu-id="3830b-111">Smtp、sip などのプレフィックス付きルーティングタイプを持つ電子メールアドレスは、複数値配列に保存されます。</span><span class="sxs-lookup"><span data-stu-id="3830b-111">Email addresses with prefixed routing types, such as smtp or sip, are saved in a multivalue array.</span></span> <span data-ttu-id="3830b-112">**ResolveNames**操作は、未解決の名前の先頭 ("sip:User1@Contoso.com" など) にルーティングの種類を追加するときに、その配列の各値に対して部分一致を実行します。</span><span class="sxs-lookup"><span data-stu-id="3830b-112">The **ResolveNames** operation performs a partial match against each value of that array when you add the routing type at the beginning of the unresolved name, such as "sip:User1@Contoso.com".</span></span> <span data-ttu-id="3830b-113">ルーティングの種類を指定しない場合、 **ResolveNames**は smtp のルーティングの種類を既定で設定し、それをプライマリ smtp アドレスプロパティに一致させ、複数値配列は検索しません。</span><span class="sxs-lookup"><span data-stu-id="3830b-113">If you don't specify a routing type, **ResolveNames** will default to the routing type of smtp, match it to a primary smtp address property, and not search the multivalue array.</span></span> 
  
<span data-ttu-id="3830b-114">1つの要求で指定できるあいまいな名前は1つだけです。</span><span class="sxs-lookup"><span data-stu-id="3830b-114">Only one ambiguous name can be specified in a single request.</span></span> <span data-ttu-id="3830b-115">Active Directory が最初に検索されてから、ユーザーの連絡先フォルダーが検索されます。</span><span class="sxs-lookup"><span data-stu-id="3830b-115">Active Directory is searched first, and then the user's contact folder is searched.</span></span> <span data-ttu-id="3830b-116">解決されたユーザーの連絡先フォルダーのエントリには、非 null の**ItemId**プロパティがあります。このプロパティは、GetItem 要求で使用できます。</span><span class="sxs-lookup"><span data-stu-id="3830b-116">Resolved entries from a user's contact folder have a non-null **ItemId** property, which can then be used in a GetItem request.</span></span> <span data-ttu-id="3830b-117">プライベート配布リストの ID である場合は、 [Expanddl 操作](expanddl-operation.md)で使用できます。</span><span class="sxs-lookup"><span data-stu-id="3830b-117">If it is the ID of a private distribution list, then it can be used in an [ExpandDL operation](expanddl-operation.md).</span></span> <span data-ttu-id="3830b-118">**Returnfullcontactdata**属性が**true**に設定されている場合、 **ResolveNames**操作で見つかった Active Directory エントリは、[連絡先](contact.md)を記述する追加のプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="3830b-118">If the **ReturnFullContactData** attribute is set to **true**, then Active Directory entries found with the **ResolveNames** operation will return additional properties that describe a [Contact](contact.md).</span></span> <span data-ttu-id="3830b-119">**Returnfullcontactdata**属性は、ユーザーの連絡先フォルダーから連絡先およびプライベート配布リストに対して返されるデータには影響しません。</span><span class="sxs-lookup"><span data-stu-id="3830b-119">The **ReturnFullContactData** attribute does not affect the data that is returned for contacts and private distribution lists from the user's contact folder.</span></span> 
  
## <a name="resolvenames-request-example"></a><span data-ttu-id="3830b-120">ResolveNames 要求の例</span><span class="sxs-lookup"><span data-stu-id="3830b-120">ResolveNames request example</span></span>

### <a name="description"></a><span data-ttu-id="3830b-121">Description</span><span class="sxs-lookup"><span data-stu-id="3830b-121">Description</span></span>

<span data-ttu-id="3830b-122">次の**ResolveNames**要求の例は、ユーザーのエントリを解決する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="3830b-122">The following example of a **ResolveNames** request shows how to resolve the entry of User.</span></span>
  
### <a name="code"></a><span data-ttu-id="3830b-123">コード</span><span class="sxs-lookup"><span data-stu-id="3830b-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>User2</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="3830b-124">コメント</span><span class="sxs-lookup"><span data-stu-id="3830b-124">Comments</span></span>

<span data-ttu-id="3830b-125">この要求への応答では、"Jo" または "Mi" で始まるすべてのエントリが返されます。</span><span class="sxs-lookup"><span data-stu-id="3830b-125">The response to this request will return all entries that start with "Jo" or "Mi."</span></span> <span data-ttu-id="3830b-126">返されるアイテムは、パブリックメールボックス、パブリックおよびプライベート配布リスト、および連絡先です。</span><span class="sxs-lookup"><span data-stu-id="3830b-126">The returned items are public mailboxes, public and private distribution lists, and contacts.</span></span>
  
> [!NOTE]
> <span data-ttu-id="3830b-127">既定の個人用連絡先フォルダー内の連絡先のみが検索されます。</span><span class="sxs-lookup"><span data-stu-id="3830b-127">Only contacts in the default personal Contacts folder are searched.</span></span> 
  
<span data-ttu-id="3830b-128">**ResolveNames**要求に対して考えられる結果は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="3830b-128">The following are the possible results for a **ResolveNames** request:</span></span> 
  
- <span data-ttu-id="3830b-129">解決されたエンティティを含まない応答は、**エラー**と等しい**ResponseClass**属性値を返します。</span><span class="sxs-lookup"><span data-stu-id="3830b-129">Responses that do not contain a resolved entity will return a **ResponseClass** attribute value equal to **Error**.</span></span> <span data-ttu-id="3830b-130">**Messagetext**要素には、"**結果が見つかりません**" が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3830b-130">The **MessageText** element will contain " **No results are found**."</span></span>
    
- <span data-ttu-id="3830b-131">1つの解決されたエンティティを含む応答は、**成功**と等しい**ResponseClass**属性値を返します。</span><span class="sxs-lookup"><span data-stu-id="3830b-131">Responses that contain a single resolved entity will return a **ResponseClass** attribute value equal to **Success**.</span></span>
    
- <span data-ttu-id="3830b-132">複数の可能なエンティティが含まれる応答は、**警告**と同じ**ResponseClass**属性値を返します。</span><span class="sxs-lookup"><span data-stu-id="3830b-132">Responses that contain multiple possible entities will return a **ResponseClass** attribute value equal to **Warning**.</span></span> <span data-ttu-id="3830b-133">この場合、エンティティを一意の id に解決できませんでした。</span><span class="sxs-lookup"><span data-stu-id="3830b-133">In this case, the entity could not be resolved to a unique identity.</span></span> <span data-ttu-id="3830b-134">**Messagetext**要素には、"複数の結果が見つかりました" という文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3830b-134">The **MessageText** element will contain "Multiple results are found."</span></span> 
    
### <a name="request-elements"></a><span data-ttu-id="3830b-135">Request 要素</span><span class="sxs-lookup"><span data-stu-id="3830b-135">Request elements</span></span>

<span data-ttu-id="3830b-136">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="3830b-136">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="3830b-137">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="3830b-137">ResolveNames</span></span>](resolvenames.md)
    
- [<span data-ttu-id="3830b-138">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="3830b-138">UnresolvedEntry</span></span>](unresolvedentry.md)
    
## <a name="successful-resolvenames-operation-response-example"></a><span data-ttu-id="3830b-139">成功した ResolveNames 操作の応答の例</span><span class="sxs-lookup"><span data-stu-id="3830b-139">Successful ResolveNames operation response example</span></span>

### <a name="description"></a><span data-ttu-id="3830b-140">Description</span><span class="sxs-lookup"><span data-stu-id="3830b-140">Description</span></span>

<span data-ttu-id="3830b-141">次の例は、 **ResolveNames**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="3830b-141">The following example shows a successful response to a **ResolveNames** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="3830b-142">コード</span><span class="sxs-lookup"><span data-stu-id="3830b-142">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ResolutionSet TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>User2</t:Name>
                <t:EmailAddress>User2@example.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Mailbox</t:MailboxType>
              </t:Mailbox>
              <t:Contact>
                <t:DisplayName>User2</t:DisplayName>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress1">SMTP:User2@example.com</t:Entry>
                </t:EmailAddresses>
                <t:ContactSource>ActiveDirectory</t:ContactSource>
              </t:Contact>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-resolvenames-response-elements"></a><span data-ttu-id="3830b-143">Successful ResolveNames response 要素</span><span class="sxs-lookup"><span data-stu-id="3830b-143">Successful ResolveNames response elements</span></span>

<span data-ttu-id="3830b-144">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="3830b-144">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="3830b-145">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="3830b-145">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="3830b-146">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="3830b-146">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
    
- [<span data-ttu-id="3830b-147">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="3830b-147">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="3830b-148">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="3830b-148">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
    
- [<span data-ttu-id="3830b-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3830b-149">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="3830b-150">解像度セット</span><span class="sxs-lookup"><span data-stu-id="3830b-150">ResolutionSet</span></span>](resolutionset.md)
    
- [<span data-ttu-id="3830b-151">Resolution</span><span class="sxs-lookup"><span data-stu-id="3830b-151">Resolution</span></span>](resolution.md)
    
- [<span data-ttu-id="3830b-152">メールボックス</span><span class="sxs-lookup"><span data-stu-id="3830b-152">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="3830b-153">Name (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="3830b-153">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="3830b-154">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="3830b-154">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="3830b-155">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="3830b-155">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="3830b-156">MailboxType</span><span class="sxs-lookup"><span data-stu-id="3830b-156">MailboxType</span></span>](mailboxtype.md)
    
- [<span data-ttu-id="3830b-157">Contact</span><span class="sxs-lookup"><span data-stu-id="3830b-157">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="3830b-158">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="3830b-158">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="3830b-159">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="3830b-159">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="3830b-160">Entry (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="3830b-160">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
- [<span data-ttu-id="3830b-161">ContactSource</span><span class="sxs-lookup"><span data-stu-id="3830b-161">ContactSource</span></span>](contactsource.md)
    
## <a name="resolvenames-operation-error-response"></a><span data-ttu-id="3830b-162">ResolveNames 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="3830b-162">ResolveNames operation error response</span></span>

### <a name="description"></a><span data-ttu-id="3830b-163">Description</span><span class="sxs-lookup"><span data-stu-id="3830b-163">Description</span></span>

<span data-ttu-id="3830b-164">次の例は、 **ResolveNames**要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="3830b-164">The following example shows an error response to a **ResolveNames** request.</span></span> <span data-ttu-id="3830b-165">解決できない名前を解決しようとすると、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="3830b-165">The error is caused by trying to resolve a name that cannot be resolved.</span></span> 
  
### <a name="code"></a><span data-ttu-id="3830b-166">コード</span><span class="sxs-lookup"><span data-stu-id="3830b-166">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Error">
          <m:MessageText>No results were found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionNoResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="3830b-167">エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="3830b-167">Error response elements</span></span>

<span data-ttu-id="3830b-168">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="3830b-168">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="3830b-169">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="3830b-169">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="3830b-170">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="3830b-170">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
    
- [<span data-ttu-id="3830b-171">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="3830b-171">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="3830b-172">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="3830b-172">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
    
- [<span data-ttu-id="3830b-173">MessageText</span><span class="sxs-lookup"><span data-stu-id="3830b-173">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="3830b-174">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3830b-174">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="3830b-175">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="3830b-175">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="3830b-176">関連項目</span><span class="sxs-lookup"><span data-stu-id="3830b-176">See also</span></span>



[<span data-ttu-id="3830b-177">ExpandDL 操作</span><span class="sxs-lookup"><span data-stu-id="3830b-177">ExpandDL operation</span></span>](expanddl-operation.md)


[<span data-ttu-id="3830b-178">名前解決の使用</span><span class="sxs-lookup"><span data-stu-id="3830b-178">Using Name Resolution</span></span>](https://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

