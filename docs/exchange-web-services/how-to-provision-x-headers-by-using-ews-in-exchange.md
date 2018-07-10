---
title: Exchange EWS を使用してプロビジョニング x-ヘッダー
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 45a99a14-a85f-47f8-af48-18eb6c6cc230
description: Exchange で EWS マネージ API または EWS を使用して、メールボックスの X ヘッダーを準備する方法について説明します。
ms.openlocfilehash: de572764921da432cfa203b3dcf166d1d34dd0cd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759041"
---
# <a name="provision-x-headers-by-using-ews-in-exchange"></a><span data-ttu-id="731a4-103">Exchange EWS を使用してプロビジョニング x-ヘッダー</span><span class="sxs-lookup"><span data-stu-id="731a4-103">Provision x-headers by using EWS in Exchange</span></span>

<span data-ttu-id="731a4-104">Exchange で EWS マネージ API または EWS を使用して、メールボックスの X ヘッダーを準備する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="731a4-104">Learn how to provision x-headers for a mailbox by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="731a4-105">X ヘッダーは、標準のヘッダー情報を通信するために電子メールのヘッダーのコレクションに追加されます。</span><span class="sxs-lookup"><span data-stu-id="731a4-105">X-headers are non-standard headers that are added to the header collection of an email to communicate information.</span></span> <span data-ttu-id="731a4-106">たとえば、電子メールにスパム信頼レベル (SCL) を示すために**X の MS-Exchange の組織の SCL**のヘッダーを持つメッセージをスタンプを交換します。</span><span class="sxs-lookup"><span data-stu-id="731a4-106">For example, Exchange stamps messages with the **X-MS-Exchange-Organization-SCL** header to indicate the spam confidence level (SCL) attributed to the email.</span></span> <span data-ttu-id="731a4-107">Outlook はその情報を使用して、電子メールに対して実行するアクションの種類を決定と同様に、電子メール クライアント (Outlook では、ユーザーがアクションを実行しない限り、表示するのにイメージを防ぐことができます)。</span><span class="sxs-lookup"><span data-stu-id="731a4-107">Email clients like Outlook can use that information to determine what type of action to take on the email (for example, Outlook can prevent images from displaying unless the user takes an action).</span></span> 
  
<span data-ttu-id="731a4-p102">Exchange は、電子メールと共に X ヘッダーを受信する初回に、名前付きプロパティとしてその X ヘッダーをメールボックス スキーマに追加します。X ヘッダー値は最初の電子メールには保存されませんが、その X ヘッダーが含まれる後続の電子メールにはすべて保存されます。このため、アプリケーションでは、ユーザーが X ヘッダーを使用する前に X ヘッダーを準備する必要があります。メールボックスへの電子メールのトランスポート配信のときに、名前付きプロパティと X ヘッダー間のマッピングが行われます。つまり、トランスポート配信で電子メールを受信する必要があります。X ヘッダーが含まれる電子メールだけをメールボックスに保存して、名前付きプロパティに対するマッピングを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="731a4-p102">Exchange adds incoming x-headers to the mailbox schema as a named property the first time it receives an email with that x-header. The x-header value is not saved on that first email; however, it is saved on all subsequent emails that include the x-header. For this reason, your application should provision x-headers before you expect to use them. The mapping between a named property and an x-header occurs in the transport delivery of the email to the mailbox. This means that you need to receive the email via transport delivery; you cannot just save an email that includes the x-header to a mailbox to create the mapping to a named property.</span></span>
  
> [!NOTE]
> <span data-ttu-id="731a4-113">X ヘッダーが保存されないことを確認する場合は、かどうか、[トランスポート エージェント](http://code.msdn.microsoft.com/Exchange-2013-Build-an-32f62f5a)または[ヘッダー ファイアウォール](http://technet.microsoft.com/ja-jp/library/bb232136%28v=exchg.150%29.aspx)フィルターは、x ヘッダーをメールボックスを取得する前に決定します。</span><span class="sxs-lookup"><span data-stu-id="731a4-113">If you find that x-headers aren't being saved, determine whether a [transport agent](http://code.msdn.microsoft.com/Exchange-2013-Build-an-32f62f5a) or [header firewall](http://technet.microsoft.com/ja-jp/library/bb232136%28v=exchg.150%29.aspx) is filtering out your x-headers before they get to the mailbox.</span></span> 
  
## <a name="provision-an-x-header-by-using-the-ews-managed-api"></a><span data-ttu-id="731a4-114">EWS マネージ API を使用して X ヘッダーを準備する</span><span class="sxs-lookup"><span data-stu-id="731a4-114">Provision an x-header by using the EWS Managed API</span></span>
<span data-ttu-id="731a4-115"><a name="bk_example1"> </a></span><span class="sxs-lookup"><span data-stu-id="731a4-115"></span></span>

<span data-ttu-id="731a4-116">次のコード例では、EWS のマネージ API の[EmailMessage.Send](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx)メソッドを使用してメールボックスの x ヘッダーを準備する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="731a4-116">The following code example shows how to use the EWS Managed API [EmailMessage.Send](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) method to provision an x-header for a mailbox.</span></span> <span data-ttu-id="731a4-117">この例では、その**サービス**は有効な[ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトと移動先のメールボックス[のクォータは名前付きプロパティ](http://technet.microsoft.com/ja-jp/library/bb851492%28v=EXCHG.80%29.aspx)の経過していないこと。</span><span class="sxs-lookup"><span data-stu-id="731a4-117">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the target mailbox hasn't exceeded the [quota for named properties](http://technet.microsoft.com/ja-jp/library/bb851492%28v=EXCHG.80%29.aspx).</span></span>
  
```cs
private static void ProvisionCustomXHeaderByEmail(ExchangeService service)
{
    // Create a definition for an extended property that will represent a custom x-header. X-headers must be created in the
    // InternetHeaders property set. The x-header name must match the name of the x-header sent in the subsequent emails so
    // the x-header and value are saved on the email.
    ExtendedPropertyDefinition xExperimentalHeader = new ExtendedPropertyDefinition(DefaultExtendedPropertySet.InternetHeaders,
                                                                                            "X-Experimental",
                                                                                            MapiPropertyType.String);
    // Create an item that is used to provision the custom x-header.
    EmailMessage email = new EmailMessage(service);
    email.ToRecipients.Add("user@contoso.com");
    email.SetExtendedProperty(xExperimentalHeader, "Provision X-Experimental Internet message header");
    try
    {
        // The mapping of the named property happens in transport delivery.
        email.Send();
        if (service.ServerInfo.MajorVersion == 12)
        {
            Console.WriteLine("Provisioned the X-Experimental across the mailbox database that hosts the user's mailbox.");
        }
        else // For versions of Exchange starting with Exchange 2010
        {
            Console.WriteLine("Provisioned the X-Experimental for the user's mailbox. You will need to run this " +
                                "for each mailbox that needs to process this x-header.");
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error: {0}", ex.Message);
    }
}
```

## <a name="provision-an-x-header-by-using-ews"></a><span data-ttu-id="731a4-118">EWS を使用して X ヘッダーを準備する</span><span class="sxs-lookup"><span data-stu-id="731a4-118">Provision an x-header by using EWS</span></span>
<span data-ttu-id="731a4-119"><a name="bk_example1"> </a></span><span class="sxs-lookup"><span data-stu-id="731a4-119"></span></span>

<span data-ttu-id="731a4-120">EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)操作を使用して作成し、x ヘッダーを持つメールボックスを準備するのには電子メールを送信する方法を次のコード例に示します。</span><span class="sxs-lookup"><span data-stu-id="731a4-120">The following code example shows how to use the EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) operation to create and send an email to provision a mailbox with an x-header.</span></span> <span data-ttu-id="731a4-121">これは、EWS のマネージ API で送信される XML 要求と、 [EWS のマネージ API を使用して、x ヘッダーを提供](#bk_example1)します。</span><span class="sxs-lookup"><span data-stu-id="731a4-121">This is the XML request that is sent by the EWS Managed API when you [Provision an x-header by using the EWS Managed API](#bk_example1).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendOnly">
      <m:Items>
        <t:Message>
          <t:ExtendedProperty>
            <t:ExtendedFieldURI DistinguishedPropertySetId="InternetHeaders"
                                PropertyName="X-Experimental"
                                PropertyType="String" />
            <t:Value>Provision X-Experimental Internet message header</t:Value>
          </t:ExtendedProperty>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>user@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

## <a name="version-differences"></a><span data-ttu-id="731a4-122">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="731a4-122">Version differences</span></span>
<span data-ttu-id="731a4-123"><a name="bk_example1"> </a></span><span class="sxs-lookup"><span data-stu-id="731a4-123"></span></span>

<span data-ttu-id="731a4-p105">Exchange Online で、Office 365 の一部としての Exchange Online で、または Exchange Server 2010 以降の Exchange オンプレミス バージョンで X ヘッダーを初めて準備する場合、格納されているメッセージに新しいカスタム X ヘッダーの値は書き込まれません。これは、X ヘッダーが、ユーザーのメールボックスの名前付きプロパティに最初にマップされる必要があるためです。このマッピングは、名前付きプロパティを追加するための最初の要求時に発生します。名前付きプロパティを作成する後続の要求が発生すると、プロパティと値はメッセージに格納されます。Exchange 2007 では、X ヘッダーが最初にメールボックス データベースに書き込まれます。その際に、メールボックス データベースにおける名前付きプロパティに対する X ヘッダーのマッピングが作成されます。名前付きプロパティを作成する後続の要求が発生すると、X ヘッダーが処理されて、Exchange 2007 データベースのメールボックス用に格納されます。</span><span class="sxs-lookup"><span data-stu-id="731a4-p105">The first time that you provision an x-header in Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange Server 2010, the value of a new custom x-header will not be written to the stored message. This is because the x-header must first be mapped to a named property in the user's mailbox. The mapping occurs upon the first request to add the named properties. When a subsequent request to create the named property occurs, the property and value are stored on the message. In Exchange 2007, the first time an x-header is written to a mailbox database, a mapping is created for the x-header to a named property across the mailbox database. When a subsequent request to create the named property occurs, the x-header is processed and stored for any mailbox in the Exchange 2007 database.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="731a4-130">次の手順</span><span class="sxs-lookup"><span data-stu-id="731a4-130">Next steps</span></span>
<span data-ttu-id="731a4-131"><a name="bk_example1"> </a></span><span class="sxs-lookup"><span data-stu-id="731a4-131"></span></span>

<span data-ttu-id="731a4-132">この資料では、ユーザーに電子メールを送信してメールボックスを 1 つの x ヘッダーを提供する方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="731a4-132">This article shows you how to provision an x-header for a single mailbox by sending an email to a user.</span></span> <span data-ttu-id="731a4-133">多くのユーザーの x ヘッダーは、呼び出し元の組織内の[受信者のリストをバッチの電子メールを送信する](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)でもプロビジョニングできます。</span><span class="sxs-lookup"><span data-stu-id="731a4-133">You can also provision an x-header for many users by [sending a batch email to a list of recipients](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md) in the caller's organization.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="731a4-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="731a4-134">See also</span></span>


- [<span data-ttu-id="731a4-135">Exchange における EWS のプロパティと拡張プロパティ</span><span class="sxs-lookup"><span data-stu-id="731a4-135">Properties and extended properties in EWS in Exchange</span></span>](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [<span data-ttu-id="731a4-136">Exchange 2013: プログラムでカスタム X ヘッダーを提供します。</span><span class="sxs-lookup"><span data-stu-id="731a4-136">Exchange 2013: Provision custom X-headers programmatically</span></span>](http://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [<span data-ttu-id="731a4-137">名前付きプロパティは、X-ヘッダーとします。</span><span class="sxs-lookup"><span data-stu-id="731a4-137">Named Properties, X-Headers, and You</span></span>](http://blogs.technet.com/b/exchange/archive/2009/04/06/3407221.aspx)
    
- [<span data-ttu-id="731a4-138">名前付きプロパティでは、ラウンド 2: どのような配置先</span><span class="sxs-lookup"><span data-stu-id="731a4-138">Named Properties, Round 2: What lies Ahead</span></span>](http://blogs.technet.com/b/exchange/archive/2009/06/12/3407672.aspx)
    
- [<span data-ttu-id="731a4-139">ヘッダー ファイアウォール</span><span class="sxs-lookup"><span data-stu-id="731a4-139">Header Firewall</span></span>](http://technet.microsoft.com/ja-jp/library/bb232136%28v=exchg.150%29.aspx)
    
- [<span data-ttu-id="731a4-140">EWS、MIME、および不足しているインターネット メッセージのヘッダー</span><span class="sxs-lookup"><span data-stu-id="731a4-140">EWS, MIME, and the missing Internet message headers</span></span>](http://msdn.microsoft.com/library/office/hh545614%28v=exchg.140%29.aspx)
    
- [<span data-ttu-id="731a4-141">電子メール メッセージを Exchange で EWS を使用してバッチ プロセス</span><span class="sxs-lookup"><span data-stu-id="731a4-141">Process email messages in batches by using EWS in Exchange</span></span>](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    

