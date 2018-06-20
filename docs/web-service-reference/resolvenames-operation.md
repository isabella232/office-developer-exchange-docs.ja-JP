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
description: ResolveNames 操作解決あいまいな電子メール アドレスと表示名です。
ms.openlocfilehash: 8443cf834dfdf104daeaaa92fdee3742c3fa3719
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833162"
---
# <a name="resolvenames-operation"></a><span data-ttu-id="4d4c1-103">ResolveNames 操作</span><span class="sxs-lookup"><span data-stu-id="4d4c1-103">ResolveNames operation</span></span>

<span data-ttu-id="4d4c1-104">**ResolveNames**操作解決あいまいな電子メール アドレスと表示名です。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-104">The **ResolveNames** operation resolves ambiguous email addresses and display names.</span></span> 
  
## <a name="using-the-resolvenames-operation"></a><span data-ttu-id="4d4c1-105">ResolveNames 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-105">Using the ResolveNames operation</span></span>

<span data-ttu-id="4d4c1-106">エイリアスを確認し、適切なメールボックスのユーザーに表示名を解決するのには、この操作を使用できます。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-106">This operation can be used to verify aliases and resolve display names to the appropriate mailbox user.</span></span> <span data-ttu-id="4d4c1-107">あいまいな名前が存在する場合、 **ResolveNames**操作の応答は、クライアント アプリケーションは、名前を解決できるよう、各メールボックスのユーザーに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-107">If ambiguous names exist, the **ResolveNames** operation response provides information about each mailbox user so that the client application can resolve the names.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4d4c1-108">備考</span><span class="sxs-lookup"><span data-stu-id="4d4c1-108">Remarks</span></span>

<span data-ttu-id="4d4c1-109">ResolveNames 応答では、最大 100 の候補を返します。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-109">The ResolveNames response returns a maximum of 100 candidates.</span></span> <span data-ttu-id="4d4c1-110">返される 100 の候補は、検索操作で発生した最初の 100 人です。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-110">The 100 candidates that are returned are the first 100 that are encountered in the lookup operation.</span></span>
  
<span data-ttu-id="4d4c1-111">プレフィックスが付けられたルーティングなど、smtp または sip、電子メール アドレスは、複数値配列に保存されます。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-111">Email addresses with prefixed routing types, such as smtp or sip, are saved in a multivalue array.</span></span> <span data-ttu-id="4d4c1-112">**ResolveNames**操作は、ルーティングの種類を「sip:User1@Contoso.com」など、未解決の名前の先頭に追加するときに、その配列の各値に対して部分的一致を実行します。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-112">The **ResolveNames** operation performs a partial match against each value of that array when you add the routing type at the beginning of the unresolved name, such as "sip:User1@Contoso.com".</span></span> <span data-ttu-id="4d4c1-113">ルーティングの種類を指定しない場合**ResolveNames**が既定の smtp ルーティングの種類に、照合するプライマリ smtp アドレスのプロパティでは、および複数値の配列を検索します。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-113">If you don't specify a routing type, **ResolveNames** will default to the routing type of smtp, match it to a primary smtp address property, and not search the multivalue array.</span></span> 
  
<span data-ttu-id="4d4c1-114">1 つの要求では、1 つだけのあいまいな名前を指定できます。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-114">Only one ambiguous name can be specified in a single request.</span></span> <span data-ttu-id="4d4c1-115">最初に active Directory を検索し、ユーザーの連絡先フォルダーを検索し、します。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-115">Active Directory is searched first, and then the user's contact folder is searched.</span></span> <span data-ttu-id="4d4c1-116">GetItem 要求で使用できる null 以外の**ItemId**プロパティがあるユーザーの連絡先フォルダーからエントリを解決します。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-116">Resolved entries from a user's contact folder have a non-null **ItemId** property, which can then be used in a GetItem request.</span></span> <span data-ttu-id="4d4c1-117">個人用配布リストの ID である場合は、 [ExpandDL の操作](expanddl-operation.md)で使用できます。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-117">If it is the ID of a private distribution list, then it can be used in an [ExpandDL operation](expanddl-operation.md).</span></span> <span data-ttu-id="4d4c1-118">**ReturnFullContactData**属性は、 **true**に設定されている場合**ResolveNames**操作で Active Directory エントリの間で[連絡先](contact.md)を記述する追加のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-118">If the **ReturnFullContactData** attribute is set to **true**, then Active Directory entries found with the **ResolveNames** operation will return additional properties that describe a [Contact](contact.md).</span></span> <span data-ttu-id="4d4c1-119">**ReturnFullContactData**属性は、メンバーとプライベートで返されるデータには影響は、ユーザーの連絡先フォルダーから配布リストを使用します。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-119">The **ReturnFullContactData** attribute does not affect the data that is returned for contacts and private distribution lists from the user's contact folder.</span></span> 
  
## <a name="resolvenames-request-example"></a><span data-ttu-id="4d4c1-120">ResolveNames 要求の例</span><span class="sxs-lookup"><span data-stu-id="4d4c1-120">ResolveNames request example</span></span>

### <a name="description"></a><span data-ttu-id="4d4c1-121">説明</span><span class="sxs-lookup"><span data-stu-id="4d4c1-121">Description</span></span>

<span data-ttu-id="4d4c1-122">**ResolveNames**要求の次の例では、ユーザーのエントリを解決する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-122">The following example of a **ResolveNames** request shows how to resolve the entry of User.</span></span>
  
### <a name="code"></a><span data-ttu-id="4d4c1-123">コード</span><span class="sxs-lookup"><span data-stu-id="4d4c1-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>User2</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="4d4c1-124">コメント</span><span class="sxs-lookup"><span data-stu-id="4d4c1-124">Comments</span></span>

<span data-ttu-id="4d4c1-125">この要求への応答は"Jo"または「マイル」で始まるすべてのエントリを返す</span><span class="sxs-lookup"><span data-stu-id="4d4c1-125">The response to this request will return all entries that start with "Jo" or "Mi."</span></span> <span data-ttu-id="4d4c1-126">返されたアイテムは、パブリックのメールボックス、パブリックとプライベートの配布リスト、および連絡先です。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-126">The returned items are public mailboxes, public and private distribution lists, and contacts.</span></span>
  
> [!NOTE]
> <span data-ttu-id="4d4c1-127">既定の個人用連絡先フォルダー内の連絡先だけが検索されます。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-127">Only contacts in the default personal Contacts folder are searched.</span></span> 
  
<span data-ttu-id="4d4c1-128">**ResolveNames**要求の可能な結果は、次のように。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-128">The following are the possible results for a **ResolveNames** request:</span></span> 
  
- <span data-ttu-id="4d4c1-129">解決されたエンティティが含まれていない応答を返します**ResponseClass**属性値**エラー**と同じです。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-129">Responses that do not contain a resolved entity will return a **ResponseClass** attribute value equal to **Error**.</span></span> <span data-ttu-id="4d4c1-130">**メッセージ テキスト**要素には「が**ない結果があります**。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-130">The **MessageText** element will contain " **No results are found**."</span></span>
    
- <span data-ttu-id="4d4c1-131">1 つの解決されたエンティティを含む応答を返します**ResponseClass**属性値**成功した場合**と同じです。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-131">Responses that contain a single resolved entity will return a **ResponseClass** attribute value equal to **Success**.</span></span>
    
- <span data-ttu-id="4d4c1-132">複数の可能なエンティティを含む応答を返します**ResponseClass**属性の値**の警告**と同じ。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-132">Responses that contain multiple possible entities will return a **ResponseClass** attribute value equal to **Warning**.</span></span> <span data-ttu-id="4d4c1-133">この例では、エンティティは、一意の id を解決できませんでした。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-133">In this case, the entity could not be resolved to a unique identity.</span></span> <span data-ttu-id="4d4c1-134">[複数の結果が見つかりました"**メッセージ テキスト**要素が含まれます</span><span class="sxs-lookup"><span data-stu-id="4d4c1-134">The **MessageText** element will contain "Multiple results are found."</span></span> 
    
### <a name="request-elements"></a><span data-ttu-id="4d4c1-135">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-135">Request elements</span></span>

<span data-ttu-id="4d4c1-136">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-136">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="4d4c1-137">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="4d4c1-137">ResolveNames</span></span>](resolvenames.md)
    
- [<span data-ttu-id="4d4c1-138">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="4d4c1-138">UnresolvedEntry</span></span>](unresolvedentry.md)
    
## <a name="successful-resolvenames-operation-response-example"></a><span data-ttu-id="4d4c1-139">ResolveNames 操作の正常な応答例</span><span class="sxs-lookup"><span data-stu-id="4d4c1-139">Successful ResolveNames operation response example</span></span>

### <a name="description"></a><span data-ttu-id="4d4c1-140">説明</span><span class="sxs-lookup"><span data-stu-id="4d4c1-140">Description</span></span>

<span data-ttu-id="4d4c1-141">**ResolveNames**要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-141">The following example shows a successful response to a **ResolveNames** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="4d4c1-142">コード</span><span class="sxs-lookup"><span data-stu-id="4d4c1-142">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-resolvenames-response-elements"></a><span data-ttu-id="4d4c1-143">ResolveNames 応答の成功の要素</span><span class="sxs-lookup"><span data-stu-id="4d4c1-143">Successful ResolveNames response elements</span></span>

<span data-ttu-id="4d4c1-144">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-144">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="4d4c1-145">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4d4c1-145">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="4d4c1-146">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="4d4c1-146">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
    
- [<span data-ttu-id="4d4c1-147">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4d4c1-147">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="4d4c1-148">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4d4c1-148">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
    
- [<span data-ttu-id="4d4c1-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4d4c1-149">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="4d4c1-150">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="4d4c1-150">ResolutionSet</span></span>](resolutionset.md)
    
- [<span data-ttu-id="4d4c1-151">解決策</span><span class="sxs-lookup"><span data-stu-id="4d4c1-151">Resolution</span></span>](resolution.md)
    
- [<span data-ttu-id="4d4c1-152">メールボックス</span><span class="sxs-lookup"><span data-stu-id="4d4c1-152">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="4d4c1-153">名 (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="4d4c1-153">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="4d4c1-154">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="4d4c1-154">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="4d4c1-155">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="4d4c1-155">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="4d4c1-156">MailboxType</span><span class="sxs-lookup"><span data-stu-id="4d4c1-156">MailboxType</span></span>](mailboxtype.md)
    
- [<span data-ttu-id="4d4c1-157">Contact</span><span class="sxs-lookup"><span data-stu-id="4d4c1-157">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="4d4c1-158">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="4d4c1-158">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="4d4c1-159">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="4d4c1-159">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="4d4c1-160">エントリ (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="4d4c1-160">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
- [<span data-ttu-id="4d4c1-161">ContactSource</span><span class="sxs-lookup"><span data-stu-id="4d4c1-161">ContactSource</span></span>](contactsource.md)
    
## <a name="resolvenames-operation-error-response"></a><span data-ttu-id="4d4c1-162">ResolveNames 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="4d4c1-162">ResolveNames operation error response</span></span>

### <a name="description"></a><span data-ttu-id="4d4c1-163">説明</span><span class="sxs-lookup"><span data-stu-id="4d4c1-163">Description</span></span>

<span data-ttu-id="4d4c1-164">**ResolveNames**要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-164">The following example shows an error response to a **ResolveNames** request.</span></span> <span data-ttu-id="4d4c1-165">解決できない名前を解決しようとしてエラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-165">The error is caused by trying to resolve a name that cannot be resolved.</span></span> 
  
### <a name="code"></a><span data-ttu-id="4d4c1-166">コード</span><span class="sxs-lookup"><span data-stu-id="4d4c1-166">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="4d4c1-167">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="4d4c1-167">Error response elements</span></span>

<span data-ttu-id="4d4c1-168">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="4d4c1-168">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="4d4c1-169">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4d4c1-169">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="4d4c1-170">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="4d4c1-170">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
    
- [<span data-ttu-id="4d4c1-171">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4d4c1-171">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="4d4c1-172">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4d4c1-172">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
    
- [<span data-ttu-id="4d4c1-173">MessageText</span><span class="sxs-lookup"><span data-stu-id="4d4c1-173">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="4d4c1-174">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4d4c1-174">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="4d4c1-175">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="4d4c1-175">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="4d4c1-176">関連項目</span><span class="sxs-lookup"><span data-stu-id="4d4c1-176">See also</span></span>



[<span data-ttu-id="4d4c1-177">ExpandDL 操作</span><span class="sxs-lookup"><span data-stu-id="4d4c1-177">ExpandDL operation</span></span>](expanddl-operation.md)


[<span data-ttu-id="4d4c1-178">名前解決の使用</span><span class="sxs-lookup"><span data-stu-id="4d4c1-178">Using Name Resolution</span></span>](http://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

