---
title: Exchange で EWS を使用して X ヘッダーを準備する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 45a99a14-a85f-47f8-af48-18eb6c6cc230
description: Exchange で EWS マネージ API または EWS を使用して、メールボックスの X ヘッダーを準備する方法について説明します。
ms.openlocfilehash: e60092e0d40d5815cdf3fd4ed588e2f74978c245
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521117"
---
# <a name="provision-x-headers-by-using-ews-in-exchange"></a>Exchange で EWS を使用して X ヘッダーを準備する

Exchange で EWS マネージ API または EWS を使用して、メールボックスの X ヘッダーを準備する方法について説明します。
  
X ヘッダーは、情報を伝達するために電子メールのヘッダー コレクションに追加される非標準のヘッダーです。たとえば、Exchange は **X-MS-Exchange-Organization-SCL** ヘッダーでメッセージにスタンプを設定し、電子メールに設定された spam confidence level (SCL) 属性を示します。Outlook などの電子メール クライアントは、この情報を使用して、電子メールで実行するアクションの種類を判別します (たとえば、Outlook ではユーザーがアクションを実行しない限りイメージを表示しないようにできます)。 
  
Exchange は、電子メールと共に X ヘッダーを受信する初回に、名前付きプロパティとしてその X ヘッダーをメールボックス スキーマに追加します。X ヘッダー値は最初の電子メールには保存されませんが、その X ヘッダーが含まれる後続の電子メールにはすべて保存されます。このため、アプリケーションでは、ユーザーが X ヘッダーを使用する前に X ヘッダーを準備する必要があります。メールボックスへの電子メールのトランスポート配信のときに、名前付きプロパティと X ヘッダー間のマッピングが行われます。つまり、トランスポート配信で電子メールを受信する必要があります。X ヘッダーが含まれる電子メールだけをメールボックスに保存して、名前付きプロパティに対するマッピングを作成することはできません。
  
> [!NOTE]
> X ヘッダーが保存されていないことが確認された場合、[トランスポート エージェント](https://code.msdn.microsoft.com/Exchange-2013-Build-an-32f62f5a)または[ヘッダー ファイアウォール](https://technet.microsoft.com/library/bb232136%28v=exchg.150%29.aspx)によって、X ヘッダーがメールボックスに到着する前にフィルタリング処理されているかどうかを判別します。 r
  
## <a name="provision-an-x-header-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して X ヘッダーを準備する
<a name="bk_example1"> </a>

次のコード例は、EWS マネージ API [EmailMessage.Send](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) メソッドを使用して、メールボックスの X ヘッダーを準備する方法を示しています。 この例では、**service** は有効な [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、対象のメールボックスは [名前付きプロパティのクォータ](https://technet.microsoft.com/library/bb851492%28v=EXCHG.80%29.aspx)を超過していないことを前提としています。
  
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

## <a name="provision-an-x-header-by-using-ews"></a>EWS を使用して X ヘッダーを準備する
<a name="bk_example1"> </a>

次のコード例は、EWS [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) 操作を行って、X ヘッダーが含まれるメールボックスを準備するために電子メールを作成し送信する方法を示しています。 これは、[EWS マネージ API を使用して X ヘッダーを準備する](#bk_example1)場合に、EWS マネージ API が送信する XML 要求でもあります。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

## <a name="version-differences"></a>バージョンの相違点
<a name="bk_example1"> </a>

Exchange Online で、Office 365 の一部としての Exchange Online で、または Exchange Server 2010 以降の Exchange オンプレミス バージョンで X ヘッダーを初めて準備する場合、格納されているメッセージに新しいカスタム X ヘッダーの値は書き込まれません。これは、X ヘッダーが、ユーザーのメールボックスの名前付きプロパティに最初にマップされる必要があるためです。このマッピングは、名前付きプロパティを追加するための最初の要求時に発生します。名前付きプロパティを作成する後続の要求が発生すると、プロパティと値はメッセージに格納されます。Exchange 2007 では、X ヘッダーが最初にメールボックス データベースに書き込まれます。その際に、メールボックス データベースにおける名前付きプロパティに対する X ヘッダーのマッピングが作成されます。名前付きプロパティを作成する後続の要求が発生すると、X ヘッダーが処理されて、Exchange 2007 データベースのメールボックス用に格納されます。
  
## <a name="next-steps"></a>次の手順
<a name="bk_example1"> </a>

この資料では、ユーザーに電子メールを送信して、1 つのメールボックスの 1 つの X ヘッダーを準備する方法を取り上げました。 多数のユーザーの X ヘッダーを準備することもできます。その場合には、呼び出し元の組織で[受信者の一覧にバッチ電子メールを送信](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)します。 
  
## <a name="see-also"></a>関連項目


- [Exchange における EWS のプロパティと拡張プロパティ](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Exchange 2013: プログラムを使用してカスタム X ヘッダーをプロビジョニングする](https://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [名前付きプロパティ、X ヘッダー、ユーザー](https://blogs.technet.com/b/exchange/archive/2009/04/06/3407221.aspx)
    
- [名前付きプロパティ、ラウンド 2: 展望](https://blogs.technet.com/b/exchange/archive/2009/06/12/3407672.aspx)
    
- [ヘッダー ファイアウォール](https://technet.microsoft.com/library/bb232136%28v=exchg.150%29.aspx)
    
- [EWS、MIME、および欠落しているインターネット メッセージ ヘッダー](https://msdn.microsoft.com/library/office/hh545614%28v=exchg.140%29.aspx)
    
- [Exchange で EWS を使用してバッチ処理でメール メッセージを処理する](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    

