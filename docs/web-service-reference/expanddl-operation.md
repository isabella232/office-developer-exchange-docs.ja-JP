---
title: ExpandDL 操作
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: 1f7837e7-9eff-4e10-9577-c40f7ed6af94
description: ExpandDL 操作は、配布リストの完全なメンバーシップを公開します。
ms.openlocfilehash: 8edaf057538e2c1136465f0ff7937c14477b2c47
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44454051"
---
# <a name="expanddl-operation"></a><span data-ttu-id="8fc91-103">ExpandDL 操作</span><span class="sxs-lookup"><span data-stu-id="8fc91-103">ExpandDL operation</span></span>

<span data-ttu-id="8fc91-104">ExpandDL 操作は、配布リストの完全なメンバーシップを公開します。</span><span class="sxs-lookup"><span data-stu-id="8fc91-104">The ExpandDL operation exposes the full membership of distribution lists.</span></span>
  
## <a name="using-the-expanddl-web-method"></a><span data-ttu-id="8fc91-105">ExpandDL Web メソッドの使用</span><span class="sxs-lookup"><span data-stu-id="8fc91-105">Using the ExpandDL Web Method</span></span>

<span data-ttu-id="8fc91-106">ExpandDL 操作では、Exchange .asmx に配置されている Web サービスを使用します。</span><span class="sxs-lookup"><span data-stu-id="8fc91-106">The ExpandDL operation uses the Web service that is located in Exchange.asmx.</span></span> <span data-ttu-id="8fc91-107">この Web サービスメソッドは、パブリック配布リストの拡張用の[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)子要素、またはプライベート配布リストの展開用の[ItemId](itemid.md)子要素のいずれかを含むことができる[Mailbox](mailbox.md)要素を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="8fc91-107">This Web service method accepts a [Mailbox](mailbox.md) element that can contain either an [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) child element for an expansion of a public distribution list or an [ItemId](itemid.md) child element for the expansion of a private distribution list.</span></span> 
  
<span data-ttu-id="8fc91-108">パブリック配布リストは、次のいずれかを使用して展開できます。</span><span class="sxs-lookup"><span data-stu-id="8fc91-108">Public distribution lists can be expanded by using one of the following:</span></span>
  
1. <span data-ttu-id="8fc91-109">配布リストのエイリアス</span><span class="sxs-lookup"><span data-stu-id="8fc91-109">Distribution list alias</span></span>
    
2. <span data-ttu-id="8fc91-110">簡易メール転送プロトコル (SMTP) アドレス</span><span class="sxs-lookup"><span data-stu-id="8fc91-110">The Simple Mail Transfer Protocol (SMTP) address</span></span>
    
3. <span data-ttu-id="8fc91-111">X400</span><span class="sxs-lookup"><span data-stu-id="8fc91-111">X400</span></span>
    
4. <span data-ttu-id="8fc91-112">X500</span><span class="sxs-lookup"><span data-stu-id="8fc91-112">X500</span></span>
    
5. <span data-ttu-id="8fc91-113">Exchange 従来のアドレス</span><span class="sxs-lookup"><span data-stu-id="8fc91-113">Exchange Legacy address</span></span>
    
6. <span data-ttu-id="8fc91-114">配布リストの名前</span><span class="sxs-lookup"><span data-stu-id="8fc91-114">The distribution list name</span></span>
    
7. <span data-ttu-id="8fc91-115">表示名</span><span class="sxs-lookup"><span data-stu-id="8fc91-115">The display name</span></span>
    
> [!IMPORTANT]
> <span data-ttu-id="8fc91-116">表示名が一意ではありません。</span><span class="sxs-lookup"><span data-stu-id="8fc91-116">Display names are not unique.</span></span> <span data-ttu-id="8fc91-117">複数のアカウントで同じ表示名を共有できます。</span><span class="sxs-lookup"><span data-stu-id="8fc91-117">Multiple accounts can share the same display name.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8fc91-118">注釈</span><span class="sxs-lookup"><span data-stu-id="8fc91-118">Remarks</span></span>

<span data-ttu-id="8fc91-119">再帰的な展開はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8fc91-119">Recursive expansion is not supported.</span></span> <span data-ttu-id="8fc91-120">1回の呼び出しで展開できる配布リストは1つだけです。</span><span class="sxs-lookup"><span data-stu-id="8fc91-120">Only one distribution list can be expanded in a single call.</span></span> <span data-ttu-id="8fc91-121">複数の配布リストが条件に一致する場合、Web サービスはエラーを報告します。</span><span class="sxs-lookup"><span data-stu-id="8fc91-121">If more than one distribution list match the criteria, the Web service reports an error.</span></span> <span data-ttu-id="8fc91-122">クライアントアプリケーションはあいまいな名前解決 (ANR) を使用してあいまいな配布リストを見つけ、必要な配布リストの正しい電子メールアドレスを[Expanddl 操作](expanddl-operation.md)のパラメーターとして選択することができます。</span><span class="sxs-lookup"><span data-stu-id="8fc91-122">A client application can use ambiguous name resolution (ANR) to find ambiguous distribution lists and then chose the correct e-mail address of the required distribution list as a parameter for the [ExpandDL operation](expanddl-operation.md).</span></span> <span data-ttu-id="8fc91-123">詳細については、「 [ResolveNames operation](resolvenames-operation.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8fc91-123">For more information, see [ResolveNames operation](resolvenames-operation.md).</span></span>
  
<span data-ttu-id="8fc91-124">パブリック配布リストは、Active Directory にあります。</span><span class="sxs-lookup"><span data-stu-id="8fc91-124">Public distribution lists are located in Active Directory.</span></span> <span data-ttu-id="8fc91-125">任意のメールが有効な配布グループまたは動的配布グループを指定できます。</span><span class="sxs-lookup"><span data-stu-id="8fc91-125">They can be any mail-enabled or dynamic distribution group.</span></span> <span data-ttu-id="8fc91-126">このグループは、アドレス一覧から非表示にしないでください。また、各メンバーには空ではない電子メールアドレスを設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8fc91-126">The group should not be hidden from the address list and each member should have a non-empty e-mail address.</span></span> <span data-ttu-id="8fc91-127">配布リストのメンバーには、メールが有効なユーザーと連絡先、パブリックフォルダー、およびメールが有効な配布リストと動的グループを使用できます。</span><span class="sxs-lookup"><span data-stu-id="8fc91-127">Members of the distribution list can be mail-enabled users and contacts, public folders, and mail-enabled distribution lists and dynamic groups.</span></span>
  
<span data-ttu-id="8fc91-128">プライベート配布リストは、ユーザーのメールボックスの [連絡先] フォルダーにあります。</span><span class="sxs-lookup"><span data-stu-id="8fc91-128">Private distribution lists are located in the Contacts folder of a user's mailbox.</span></span> <span data-ttu-id="8fc91-129">プライベート配布リストに電子メールアドレスが含まれていないため、ストアのアイテム識別子が ExpandDL 要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="8fc91-129">Private distribution lists do not have e-mail addresses so their store item identifiers are used in an ExpandDL request.</span></span> <span data-ttu-id="8fc91-130">プライベート配布リストのメンバーは、メールが有効なユーザー、Active Directory からの連絡先または配布リスト、またはユーザーの連絡先フォルダーの連絡先またはプライベート配布リストを使用できます。</span><span class="sxs-lookup"><span data-stu-id="8fc91-130">Members of a private distribution list can be any mail-enabled user, contacts or distribution lists from Active Directory, or contacts or private distribution lists from a user's Contacts folder.</span></span>
  
<span data-ttu-id="8fc91-131">連絡先またはプライベート配布リストの場合は、アイテムの識別子が応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="8fc91-131">For contacts or private distribution lists, the item identifiers are returned in the response.</span></span> <span data-ttu-id="8fc91-132">これは、オブジェクトに関する情報を取得したり、プライベート配布リストのメンバーシップを拡張したりするために使用できます。</span><span class="sxs-lookup"><span data-stu-id="8fc91-132">This can be used to get information about the object or to expand membership in a private distribution list.</span></span>
  
## <a name="expanddl-private-distribution-list-request-example"></a><span data-ttu-id="8fc91-133">ExpandDL プライベート配布リスト要求の例</span><span class="sxs-lookup"><span data-stu-id="8fc91-133">ExpandDL Private Distribution List request example</span></span>

### <a name="description"></a><span data-ttu-id="8fc91-134">Description</span><span class="sxs-lookup"><span data-stu-id="8fc91-134">Description</span></span>

<span data-ttu-id="8fc91-135">次の ExpandDL 要求の例は、プライベート配布リストを展開するための要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="8fc91-135">The following example of an ExpandDL request shows how to form a request to expand a private distribution list.</span></span>
  
### <a name="code"></a><span data-ttu-id="8fc91-136">コード</span><span class="sxs-lookup"><span data-stu-id="8fc91-136">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ExpandDL>
      <m:Mailbox>
       <t:EmailAddress>test</t:EmailAddress>
      </m:Mailbox>
    </m:ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="8fc91-137">コメント</span><span class="sxs-lookup"><span data-stu-id="8fc91-137">Comments</span></span>

<span data-ttu-id="8fc91-138">プライベート配布リストを展開する場合、 [mailbox](mailbox.md)要素には、ユーザーのメールボックス内のプライベート配布リストを識別する[ItemId](itemid.md)要素が含まれます。</span><span class="sxs-lookup"><span data-stu-id="8fc91-138">To expand a private distribution list, the [Mailbox](mailbox.md) element will contain the [ItemId](itemid.md) element that identifies a private distribution list in the user's mailbox.</span></span> 
  
## <a name="expanddl-public-distribution-list-request-example"></a><span data-ttu-id="8fc91-139">ExpandDL パブリック配布リスト要求の例</span><span class="sxs-lookup"><span data-stu-id="8fc91-139">ExpandDL Public Distribution List request example</span></span>

### <a name="description"></a><span data-ttu-id="8fc91-140">Description</span><span class="sxs-lookup"><span data-stu-id="8fc91-140">Description</span></span>

<span data-ttu-id="8fc91-141">次の ExpandDL 要求の例は、パブリック配布リストを展開するための要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="8fc91-141">The following example of an ExpandDL request shows how to form a request to expand a public distribution list.</span></span> <span data-ttu-id="8fc91-142">この例では、表示名を使用して配布リストを展開する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="8fc91-142">The example shows the use of a display name to expand a distribution list.</span></span>
  
### <a name="code"></a><span data-ttu-id="8fc91-143">コード</span><span class="sxs-lookup"><span data-stu-id="8fc91-143">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:EmailAddress>TheDistributionList</t:EmailAddress>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="8fc91-144">コメント</span><span class="sxs-lookup"><span data-stu-id="8fc91-144">Comments</span></span>

<span data-ttu-id="8fc91-145">この要求への応答には、配布リスト内の各メールボックスを識別する**メールボックス**要素が含まれます。</span><span class="sxs-lookup"><span data-stu-id="8fc91-145">The response to this request will contain **Mailbox** elements that identify each mailbox in the distribution list.</span></span> <span data-ttu-id="8fc91-146">配布リストが配布リスト内に含まれている場合は、埋め込まれた配布リストに対して別の配布リストの展開を実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8fc91-146">If a distribution list is contained within a distribution list, a separate distribution list expansion must be performed on the embedded distribution list.</span></span> <span data-ttu-id="8fc91-147">配布リストにメンバーが含まれていない場合、または要求された配布リストが存在しない場合、 **ResponseClass**属性の値は Success と等しくなります。</span><span class="sxs-lookup"><span data-stu-id="8fc91-147">If the distribution list has no members or the requested distribution list does not exist, the **ResponseClass** attribute will contain a value equal to Success.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="8fc91-148">Request 要素</span><span class="sxs-lookup"><span data-stu-id="8fc91-148">Request elements</span></span>

<span data-ttu-id="8fc91-149">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="8fc91-149">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="8fc91-150">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="8fc91-150">ExpandDL</span></span>](expanddl.md)
    
- [<span data-ttu-id="8fc91-151">メールボックス</span><span class="sxs-lookup"><span data-stu-id="8fc91-151">Mailbox</span></span>](mailbox.md)
    
- <span data-ttu-id="8fc91-152">[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)は、パブリック配布リストを識別するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="8fc91-152">[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) is used to identify public distribution lists.</span></span> <span data-ttu-id="8fc91-153">[ItemId](itemid.md)要素は、プライベート配布リストを識別するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="8fc91-153">The [ItemId](itemid.md) element is used to identify private distribution lists.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="8fc91-154">これらの要素を説明するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="8fc91-154">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="successful-expanddl-response-example"></a><span data-ttu-id="8fc91-155">Successful ExpandDL 応答の例</span><span class="sxs-lookup"><span data-stu-id="8fc91-155">Successful ExpandDL response example</span></span>

### <a name="description"></a><span data-ttu-id="8fc91-156">Description</span><span class="sxs-lookup"><span data-stu-id="8fc91-156">Description</span></span>

<span data-ttu-id="8fc91-157">次に示す ExpandDL 応答の例は、上記の要求に対する応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="8fc91-157">The following example of an ExpandDL response shows a response to the request described above.</span></span> <span data-ttu-id="8fc91-158">配布リストの展開では、以下について説明します。</span><span class="sxs-lookup"><span data-stu-id="8fc91-158">The distribution list expansion describes the following:</span></span> 
  
- <span data-ttu-id="8fc91-159">応答で返される配布リストのメンバー数。</span><span class="sxs-lookup"><span data-stu-id="8fc91-159">The number of members of the distribution list that are returned in the response.</span></span>
    
- <span data-ttu-id="8fc91-160">応答に配布リストのすべてのメンバーが含まれているかどうか。</span><span class="sxs-lookup"><span data-stu-id="8fc91-160">Whether the response contains all the members of the distribution list.</span></span>
    
- <span data-ttu-id="8fc91-161">メールボックスの名前。</span><span class="sxs-lookup"><span data-stu-id="8fc91-161">The name of the mailbox.</span></span>
    
- <span data-ttu-id="8fc91-162">メールボックスの電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="8fc91-162">The e-mail address of the mailbox.</span></span>
    
- <span data-ttu-id="8fc91-163">メールボックスのルーティングの種類。</span><span class="sxs-lookup"><span data-stu-id="8fc91-163">The routing type for the mailbox.</span></span>
    
- <span data-ttu-id="8fc91-164">メールボックスの種類。</span><span class="sxs-lookup"><span data-stu-id="8fc91-164">The type of mailbox.</span></span>
    
> [!NOTE]
> <span data-ttu-id="8fc91-165">配布リストの名前は、応答に含まれていません。そのため、要求からの名前を記録しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="8fc91-165">The distribution list name is not included in the response; therefore, you must keep track of the name from the request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="8fc91-166">コード</span><span class="sxs-lookup"><span data-stu-id="8fc91-166">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a><span data-ttu-id="8fc91-167">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="8fc91-167">Successful response elements</span></span>

<span data-ttu-id="8fc91-168">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="8fc91-168">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="8fc91-169">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="8fc91-169">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="8fc91-170">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="8fc91-170">ExpandDLResponse</span></span>](expanddlresponse.md)
    
- [<span data-ttu-id="8fc91-171">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8fc91-171">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="8fc91-172">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8fc91-172">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
    
- [<span data-ttu-id="8fc91-173">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8fc91-173">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="8fc91-174">DLExpansion 展開</span><span class="sxs-lookup"><span data-stu-id="8fc91-174">DLExpansion</span></span>](dlexpansion.md)
    
- [<span data-ttu-id="8fc91-175">メールボックス</span><span class="sxs-lookup"><span data-stu-id="8fc91-175">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="8fc91-176">Name (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="8fc91-176">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="8fc91-177">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="8fc91-177">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="8fc91-178">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="8fc91-178">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="8fc91-179">MailboxType</span><span class="sxs-lookup"><span data-stu-id="8fc91-179">MailboxType</span></span>](mailboxtype.md)
    
<span data-ttu-id="8fc91-180">ExpandDL 操作の応答メッセージに関するその他のオプションについては、スキーマ階層を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8fc91-180">To find other options for the response message of the ExpandDL operation, explore the schema hierarchy.</span></span> <span data-ttu-id="8fc91-181">[Expanddlresponse](expanddlresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="8fc91-181">Start at the [ExpandDLResponse](expanddlresponse.md) element.</span></span> 
  
## <a name="expanddl-error-response"></a><span data-ttu-id="8fc91-182">ExpandDL エラー応答</span><span class="sxs-lookup"><span data-stu-id="8fc91-182">ExpandDL error response</span></span>

### <a name="description"></a><span data-ttu-id="8fc91-183">Description</span><span class="sxs-lookup"><span data-stu-id="8fc91-183">Description</span></span>

<span data-ttu-id="8fc91-184">次の例は、ExpandDL 要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="8fc91-184">The following example shows an error response to an ExpandDL request.</span></span>
  
### <a name="code"></a><span data-ttu-id="8fc91-185">コード</span><span class="sxs-lookup"><span data-stu-id="8fc91-185">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="8fc91-186">エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="8fc91-186">Error response elements</span></span>

<span data-ttu-id="8fc91-187">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="8fc91-187">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="8fc91-188">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="8fc91-188">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="8fc91-189">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="8fc91-189">ExpandDLResponse</span></span>](expanddlresponse.md)
    
- [<span data-ttu-id="8fc91-190">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8fc91-190">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="8fc91-191">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8fc91-191">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
    
- [<span data-ttu-id="8fc91-192">MessageText</span><span class="sxs-lookup"><span data-stu-id="8fc91-192">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="8fc91-193">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8fc91-193">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="8fc91-194">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="8fc91-194">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="8fc91-195">ExpandDL 操作の応答メッセージに関するその他のオプションについては、スキーマ階層を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8fc91-195">To find other options for the response message of the ExpandDL operation, explore the schema hierarchy.</span></span> <span data-ttu-id="8fc91-196">[Expanddlresponse](expanddlresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="8fc91-196">Start at the [ExpandDLResponse](expanddlresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="8fc91-197">関連項目</span><span class="sxs-lookup"><span data-stu-id="8fc91-197">See also</span></span>

- [<span data-ttu-id="8fc91-198">ResolveNames 操作</span><span class="sxs-lookup"><span data-stu-id="8fc91-198">ResolveNames operation</span></span>](resolvenames-operation.md)
- [<span data-ttu-id="8fc91-199">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8fc91-199">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

