---
title: ExpandDL 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: 1f7837e7-9eff-4e10-9577-c40f7ed6af94
description: ExpandDL 操作では、配布リストの完全なメンバーシップを公開します。
ms.openlocfilehash: e4654120881f81a79358e0e7c0ab016f94db3288
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760379"
---
# <a name="expanddl-operation"></a><span data-ttu-id="cb86b-103">ExpandDL 操作</span><span class="sxs-lookup"><span data-stu-id="cb86b-103">ExpandDL operation</span></span>

<span data-ttu-id="cb86b-104">ExpandDL 操作では、配布リストの完全なメンバーシップを公開します。</span><span class="sxs-lookup"><span data-stu-id="cb86b-104">The ExpandDL operation exposes the full membership of distribution lists.</span></span>
  
## <a name="using-the-expanddl-web-method"></a><span data-ttu-id="cb86b-105">ExpandDL Web メソッドを使用します。</span><span class="sxs-lookup"><span data-stu-id="cb86b-105">Using the ExpandDL Web Method</span></span>

<span data-ttu-id="cb86b-106">ExpandDL 操作では、Exchange.asmx に配置されている Web サービスを使用します。</span><span class="sxs-lookup"><span data-stu-id="cb86b-106">The ExpandDL operation uses the Web service that is located in Exchange.asmx.</span></span> <span data-ttu-id="cb86b-107">この Web サービス メソッドは、パブリックな配布リストの拡張の[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)の子要素またはプライベートの拡張のため、[アイテム Id](itemid.md)の子要素のいずれかを含むことができる[メールボックス](mailbox.md)の要素を受け入れる配布リストです。</span><span class="sxs-lookup"><span data-stu-id="cb86b-107">This Web service method accepts a [Mailbox](mailbox.md) element that can contain either an [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) child element for an expansion of a public distribution list or an [ItemId](itemid.md) child element for the expansion of a private distribution list.</span></span> 
  
<span data-ttu-id="cb86b-108">パブリックな配布リストを展開するには、次のいずれかを使用します。</span><span class="sxs-lookup"><span data-stu-id="cb86b-108">Public distribution lists can be expanded by using one of the following:</span></span>
  
1. <span data-ttu-id="cb86b-109">配布リストのエイリアス</span><span class="sxs-lookup"><span data-stu-id="cb86b-109">Distribution list alias</span></span>
    
2. <span data-ttu-id="cb86b-110">簡易メール転送プロトコル (SMTP) アドレス</span><span class="sxs-lookup"><span data-stu-id="cb86b-110">The Simple Mail Transfer Protocol (SMTP) address</span></span>
    
3. <span data-ttu-id="cb86b-111">X400</span><span class="sxs-lookup"><span data-stu-id="cb86b-111">X400</span></span>
    
4. <span data-ttu-id="cb86b-112">X500</span><span class="sxs-lookup"><span data-stu-id="cb86b-112">X500</span></span>
    
5. <span data-ttu-id="cb86b-113">Exchange の従来のアドレス</span><span class="sxs-lookup"><span data-stu-id="cb86b-113">Exchange Legacy address</span></span>
    
6. <span data-ttu-id="cb86b-114">配布リストの名前</span><span class="sxs-lookup"><span data-stu-id="cb86b-114">The distribution list name</span></span>
    
7. <span data-ttu-id="cb86b-115">表示名</span><span class="sxs-lookup"><span data-stu-id="cb86b-115">The display name</span></span>
    
> [!IMPORTANT]
> <span data-ttu-id="cb86b-116">表示名が一意ではありません。</span><span class="sxs-lookup"><span data-stu-id="cb86b-116">Display names are not unique.</span></span> <span data-ttu-id="cb86b-117">複数のアカウントは、同じ表示名を共有できます。</span><span class="sxs-lookup"><span data-stu-id="cb86b-117">Multiple accounts can share the same display name.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="cb86b-118">備考</span><span class="sxs-lookup"><span data-stu-id="cb86b-118">Remarks</span></span>

<span data-ttu-id="cb86b-119">再帰的な拡張はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb86b-119">Recursive expansion is not supported.</span></span> <span data-ttu-id="cb86b-120">1 回の呼び出しでは、1 つの配布リストを拡張できます。</span><span class="sxs-lookup"><span data-stu-id="cb86b-120">Only one distribution list can be expanded in a single call.</span></span> <span data-ttu-id="cb86b-121">1 つ以上の配布リストには、条件が一致すると、Web サービスはエラーを報告します。</span><span class="sxs-lookup"><span data-stu-id="cb86b-121">If more than one distribution list match the criteria, the Web service reports an error.</span></span> <span data-ttu-id="cb86b-122">クライアント アプリケーションでは、あいまいな配布リストと、 [ExpandDL 操作](expanddl-operation.md)のパラメーターとして必要な配布リストの正しい電子メール アドレスを選択し、あいまいな名前解決 (ANR) を使用できます。</span><span class="sxs-lookup"><span data-stu-id="cb86b-122">A client application can use ambiguous name resolution (ANR) to find ambiguous distribution lists and then chose the correct e-mail address of the required distribution list as a parameter for the [ExpandDL operation](expanddl-operation.md).</span></span> <span data-ttu-id="cb86b-123">詳細については、 [ResolveNames の操作](resolvenames-operation.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb86b-123">For more information, see [ResolveNames operation](resolvenames-operation.md).</span></span>
  
<span data-ttu-id="cb86b-124">パブリックな配布リストは、Active Directory に配置されます。</span><span class="sxs-lookup"><span data-stu-id="cb86b-124">Public distribution lists are located in Active Directory.</span></span> <span data-ttu-id="cb86b-125">メールが有効なまたは動的配布グループすることができます。</span><span class="sxs-lookup"><span data-stu-id="cb86b-125">They can be any mail-enabled or dynamic distribution group.</span></span> <span data-ttu-id="cb86b-126">アドレス] ボックスの一覧からグループを表示する必要があり、各メンバーには空でない電子メール アドレスが必要があります。</span><span class="sxs-lookup"><span data-stu-id="cb86b-126">The group should not be hidden from the address list and each member should have a non-empty e-mail address.</span></span> <span data-ttu-id="cb86b-127">配布リストのメンバーには、メールが有効なユーザーと連絡先、パブリック フォルダー、およびメールが有効な配布リストおよび動的グループを指定できます。</span><span class="sxs-lookup"><span data-stu-id="cb86b-127">Members of the distribution list can be mail-enabled users and contacts, public folders, and mail-enabled distribution lists and dynamic groups.</span></span>
  
<span data-ttu-id="cb86b-128">個人用配布リストは、ユーザーのメールボックスの [連絡先] フォルダーに配置されます。</span><span class="sxs-lookup"><span data-stu-id="cb86b-128">Private distribution lists are located in the Contacts folder of a user's mailbox.</span></span> <span data-ttu-id="cb86b-129">個人用配布リストは、ExpandDL 要求でそのストアの項目の識別子を使用するための電子メール アドレスがありません。</span><span class="sxs-lookup"><span data-stu-id="cb86b-129">Private distribution lists do not have e-mail addresses so their store item identifiers are used in an ExpandDL request.</span></span> <span data-ttu-id="cb86b-130">個人用配布リストのメンバーは、メールが有効なユーザー、連絡先または配布リストを Active Directory から、またはユーザーの連絡先フォルダーから連絡先または非公開の配布が一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="cb86b-130">Members of a private distribution list can be any mail-enabled user, contacts or distribution lists from Active Directory, or contacts or private distribution lists from a user's Contacts folder.</span></span>
  
<span data-ttu-id="cb86b-131">連絡先または個人用配布リストは、項目の識別子が応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="cb86b-131">For contacts or private distribution lists, the item identifiers are returned in the response.</span></span> <span data-ttu-id="cb86b-132">これは、オブジェクトに関する情報を取得または個人用配布リストのメンバーシップを展開に使用できます。</span><span class="sxs-lookup"><span data-stu-id="cb86b-132">This can be used to get information about the object or to expand membership in a private distribution list.</span></span>
  
## <a name="expanddl-private-distribution-list-request-example"></a><span data-ttu-id="cb86b-133">ExpandDL プライベート同報リストの要求の例</span><span class="sxs-lookup"><span data-stu-id="cb86b-133">ExpandDL Private Distribution List request example</span></span>

### <a name="description"></a><span data-ttu-id="cb86b-134">説明</span><span class="sxs-lookup"><span data-stu-id="cb86b-134">Description</span></span>

<span data-ttu-id="cb86b-135">ExpandDL 要求の次の例では、個人用配布リストを展開するための要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="cb86b-135">The following example of an ExpandDL request shows how to form a request to expand a private distribution list.</span></span>
  
### <a name="code"></a><span data-ttu-id="cb86b-136">コード</span><span class="sxs-lookup"><span data-stu-id="cb86b-136">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:ItemId Id="xASUAd==" ChangeKey="AAts0Q=="/>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="cb86b-137">コメント</span><span class="sxs-lookup"><span data-stu-id="cb86b-137">Comments</span></span>

<span data-ttu-id="cb86b-138">個人用配布リストを展開するには、[メールボックス](mailbox.md)の要素にユーザーのメールボックス内の個人用配布リストを識別する[ItemId](itemid.md)の要素が含まれます。</span><span class="sxs-lookup"><span data-stu-id="cb86b-138">To expand a private distribution list, the [Mailbox](mailbox.md) element will contain the [ItemId](itemid.md) element that identifies a private distribution list in the user's mailbox.</span></span> 
  
## <a name="expanddl-public-distribution-list-request-example"></a><span data-ttu-id="cb86b-139">ExpandDL パブリック同報リストの要求の例</span><span class="sxs-lookup"><span data-stu-id="cb86b-139">ExpandDL Public Distribution List request example</span></span>

### <a name="description"></a><span data-ttu-id="cb86b-140">説明</span><span class="sxs-lookup"><span data-stu-id="cb86b-140">Description</span></span>

<span data-ttu-id="cb86b-141">ExpandDL 要求の次の例では、パブリックな配布リストを展開するための要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="cb86b-141">The following example of an ExpandDL request shows how to form a request to expand a public distribution list.</span></span> <span data-ttu-id="cb86b-142">例では、配布リストを展開するのには表示名の使用を示します。</span><span class="sxs-lookup"><span data-stu-id="cb86b-142">The example shows the use of a display name to expand a distribution list.</span></span>
  
### <a name="code"></a><span data-ttu-id="cb86b-143">コード</span><span class="sxs-lookup"><span data-stu-id="cb86b-143">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:EmailAddress>TheDistributionList</t:EmailAddress>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="cb86b-144">コメント</span><span class="sxs-lookup"><span data-stu-id="cb86b-144">Comments</span></span>

<span data-ttu-id="cb86b-145">この要求に対する応答を配布リストには、各メールボックスを識別する**メールボックス**の要素が含まれます。</span><span class="sxs-lookup"><span data-stu-id="cb86b-145">The response to this request will contain **Mailbox** elements that identify each mailbox in the distribution list.</span></span> <span data-ttu-id="cb86b-146">配布リストに含まれる配布リストが含まれる場合は、埋め込みの配布リストに別の配布リストの展開を実行しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="cb86b-146">If a distribution list is contained within a distribution list, a separate distribution list expansion must be performed on the embedded distribution list.</span></span> <span data-ttu-id="cb86b-147">配布リストにメンバーが存在しないか、要求された配布リストが存在しない場合、 **ResponseClass**属性には成功した場合に相当する値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="cb86b-147">If the distribution list has no members or the requested distribution list does not exist, the **ResponseClass** attribute will contain a value equal to Success.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="cb86b-148">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="cb86b-148">Request elements</span></span>

<span data-ttu-id="cb86b-149">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="cb86b-149">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="cb86b-150">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="cb86b-150">ExpandDL</span></span>](expanddl.md)
    
- [<span data-ttu-id="cb86b-151">メールボックス</span><span class="sxs-lookup"><span data-stu-id="cb86b-151">Mailbox</span></span>](mailbox.md)
    
- <span data-ttu-id="cb86b-152">[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)を使用して、パブリックな配布リストを識別します。</span><span class="sxs-lookup"><span data-stu-id="cb86b-152">[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) is used to identify public distribution lists.</span></span> <span data-ttu-id="cb86b-153">[アイテム Id](itemid.md)要素を使用して、個人用配布リストを識別します。</span><span class="sxs-lookup"><span data-stu-id="cb86b-153">The [ItemId](itemid.md) element is used to identify private distribution lists.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="cb86b-154">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、これらの要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="cb86b-154">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="successful-expanddl-response-example"></a><span data-ttu-id="cb86b-155">成功した ExpandDL の応答の例</span><span class="sxs-lookup"><span data-stu-id="cb86b-155">Successful ExpandDL response example</span></span>

### <a name="description"></a><span data-ttu-id="cb86b-156">説明</span><span class="sxs-lookup"><span data-stu-id="cb86b-156">Description</span></span>

<span data-ttu-id="cb86b-157">ExpandDL 応答の次の使用例は、上記の要求への応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="cb86b-157">The following example of an ExpandDL response shows a response to the request described above.</span></span> <span data-ttu-id="cb86b-158">配布リストの展開では、次の項目について説明します。</span><span class="sxs-lookup"><span data-stu-id="cb86b-158">The distribution list expansion describes the following:</span></span> 
  
- <span data-ttu-id="cb86b-159">応答で返される配布リストのメンバーの数です。</span><span class="sxs-lookup"><span data-stu-id="cb86b-159">The number of members of the distribution list that are returned in the response.</span></span>
    
- <span data-ttu-id="cb86b-160">かどうか、応答には、配布リストのすべてのメンバーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="cb86b-160">Whether the response contains all the members of the distribution list.</span></span>
    
- <span data-ttu-id="cb86b-161">メールボックスの名前です。</span><span class="sxs-lookup"><span data-stu-id="cb86b-161">The name of the mailbox.</span></span>
    
- <span data-ttu-id="cb86b-162">メールボックスの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="cb86b-162">The e-mail address of the mailbox.</span></span>
    
- <span data-ttu-id="cb86b-163">メールボックスのルーティングの種類です。</span><span class="sxs-lookup"><span data-stu-id="cb86b-163">The routing type for the mailbox.</span></span>
    
- <span data-ttu-id="cb86b-164">メールボックスの種類です。</span><span class="sxs-lookup"><span data-stu-id="cb86b-164">The type of mailbox.</span></span>
    
> [!NOTE]
> <span data-ttu-id="cb86b-165">配布リストの名前が応答に含まれていません。したがって、する必要がありますの追跡の要求からの名前。</span><span class="sxs-lookup"><span data-stu-id="cb86b-165">The distribution list name is not included in the response; therefore, you must keep track of the name from the request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="cb86b-166">コード</span><span class="sxs-lookup"><span data-stu-id="cb86b-166">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ExpandDLResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DLExpansion TotalItemsInView="3" IncludesLastItemInRange="true">
            <t:Mailbox>
              <t:Name>Dan Park</t:Name>
              <t:EmailAddress>dpark@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
            <t:Mailbox>
              <t:Name>Jeff Price</t:Name>
              <t:EmailAddress>jprice@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
            <t:Mailbox>
              <t:Name>Tanja Plate</t:Name>
              <t:EmailAddress>tplate@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
          </m:DLExpansion>
        </m:ExpandDLResponseMessage>
      </m:ResponseMessages>
    </ExpandDLResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="cb86b-167">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="cb86b-167">Successful response elements</span></span>

<span data-ttu-id="cb86b-168">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="cb86b-168">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="cb86b-169">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="cb86b-169">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="cb86b-170">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="cb86b-170">ExpandDLResponse</span></span>](expanddlresponse.md)
    
- [<span data-ttu-id="cb86b-171">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="cb86b-171">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="cb86b-172">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="cb86b-172">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
    
- [<span data-ttu-id="cb86b-173">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="cb86b-173">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="cb86b-174">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="cb86b-174">DLExpansion</span></span>](dlexpansion.md)
    
- [<span data-ttu-id="cb86b-175">メールボックス</span><span class="sxs-lookup"><span data-stu-id="cb86b-175">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="cb86b-176">名 (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="cb86b-176">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="cb86b-177">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="cb86b-177">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="cb86b-178">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="cb86b-178">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="cb86b-179">MailboxType</span><span class="sxs-lookup"><span data-stu-id="cb86b-179">MailboxType</span></span>](mailboxtype.md)
    
<span data-ttu-id="cb86b-180">ExpandDL 操作の応答メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="cb86b-180">To find other options for the response message of the ExpandDL operation, explore the schema hierarchy.</span></span> <span data-ttu-id="cb86b-181">[ExpandDLResponse](expanddlresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="cb86b-181">Start at the [ExpandDLResponse](expanddlresponse.md) element.</span></span> 
  
## <a name="expanddl-error-response"></a><span data-ttu-id="cb86b-182">ExpandDL エラー応答</span><span class="sxs-lookup"><span data-stu-id="cb86b-182">ExpandDL error response</span></span>

### <a name="description"></a><span data-ttu-id="cb86b-183">説明</span><span class="sxs-lookup"><span data-stu-id="cb86b-183">Description</span></span>

<span data-ttu-id="cb86b-184">ExpandDL 要求に対するエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cb86b-184">The following example shows an error response to an ExpandDL request.</span></span>
  
### <a name="code"></a><span data-ttu-id="cb86b-185">コード</span><span class="sxs-lookup"><span data-stu-id="cb86b-185">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ExpandDLResponseMessage ResponseClass="Error">
          <m:MessageText>No results are found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionNoResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ExpandDLResponseMessage>
      </m:ResponseMessages>
    </ExpandDLResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="cb86b-186">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="cb86b-186">Error response elements</span></span>

<span data-ttu-id="cb86b-187">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="cb86b-187">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="cb86b-188">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="cb86b-188">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="cb86b-189">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="cb86b-189">ExpandDLResponse</span></span>](expanddlresponse.md)
    
- [<span data-ttu-id="cb86b-190">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="cb86b-190">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="cb86b-191">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="cb86b-191">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
    
- [<span data-ttu-id="cb86b-192">MessageText</span><span class="sxs-lookup"><span data-stu-id="cb86b-192">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="cb86b-193">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="cb86b-193">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="cb86b-194">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="cb86b-194">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="cb86b-195">ExpandDL 操作の応答メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="cb86b-195">To find other options for the response message of the ExpandDL operation, explore the schema hierarchy.</span></span> <span data-ttu-id="cb86b-196">[ExpandDLResponse](expanddlresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="cb86b-196">Start at the [ExpandDLResponse](expanddlresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="cb86b-197">関連項目</span><span class="sxs-lookup"><span data-stu-id="cb86b-197">See also</span></span>

- [<span data-ttu-id="cb86b-198">ResolveNames 操作</span><span class="sxs-lookup"><span data-stu-id="cb86b-198">ResolveNames operation</span></span>](resolvenames-operation.md)
- [<span data-ttu-id="cb86b-199">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="cb86b-199">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

