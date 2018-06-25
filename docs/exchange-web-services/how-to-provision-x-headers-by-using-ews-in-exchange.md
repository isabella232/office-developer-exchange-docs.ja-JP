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
# <a name="provision-x-headers-by-using-ews-in-exchange"></a>Exchange EWS を使用してプロビジョニング x-ヘッダー

Exchange で EWS マネージ API または EWS を使用して、メールボックスの X ヘッダーを準備する方法について説明します。
  
X ヘッダーは、標準のヘッダー情報を通信するために電子メールのヘッダーのコレクションに追加されます。 たとえば、電子メールにスパム信頼レベル (SCL) を示すために**X の MS-Exchange の組織の SCL**のヘッダーを持つメッセージをスタンプを交換します。 Outlook はその情報を使用して、電子メールに対して実行するアクションの種類を決定と同様に、電子メール クライアント (Outlook では、ユーザーがアクションを実行しない限り、表示するのにイメージを防ぐことができます)。 
  
Exchange は、電子メールと共に X ヘッダーを受信する初回に、名前付きプロパティとしてその X ヘッダーをメールボックス スキーマに追加します。X ヘッダー値は最初の電子メールには保存されませんが、その X ヘッダーが含まれる後続の電子メールにはすべて保存されます。このため、アプリケーションでは、ユーザーが X ヘッダーを使用する前に X ヘッダーを準備する必要があります。メールボックスへの電子メールのトランスポート配信のときに、名前付きプロパティと X ヘッダー間のマッピングが行われます。つまり、トランスポート配信で電子メールを受信する必要があります。X ヘッダーが含まれる電子メールだけをメールボックスに保存して、名前付きプロパティに対するマッピングを作成することはできません。
  
> [!NOTE]
> X ヘッダーが保存されないことを確認する場合は、かどうか、[トランスポート エージェント](http://code.msdn.microsoft.com/Exchange-2013-Build-an-32f62f5a)または[ヘッダー ファイアウォール](http://technet.microsoft.com/en-us/library/bb232136%28v=exchg.150%29.aspx)フィルターは、x ヘッダーをメールボックスを取得する前に決定します。 
  
## <a name="provision-an-x-header-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して X ヘッダーを準備する
<a name="bk_example1"> </a>

次のコード例では、EWS のマネージ API の[EmailMessage.Send](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx)メソッドを使用してメールボックスの x ヘッダーを準備する方法を示します。 この例では、その**サービス**は有効な[ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトと移動先のメールボックス[のクォータは名前付きプロパティ](http://technet.microsoft.com/en-us/library/bb851492%28v=EXCHG.80%29.aspx)の経過していないこと。
  
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

EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)操作を使用して作成し、x ヘッダーを持つメールボックスを準備するのには電子メールを送信する方法を次のコード例に示します。 これは、EWS のマネージ API で送信される XML 要求と、 [EWS のマネージ API を使用して、x ヘッダーを提供](#bk_example1)します。
  
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

## <a name="version-differences"></a>バージョンの相違点
<a name="bk_example1"> </a>

Exchange Online で、Office 365 の一部としての Exchange Online で、または Exchange Server 2010 以降の Exchange オンプレミス バージョンで X ヘッダーを初めて準備する場合、格納されているメッセージに新しいカスタム X ヘッダーの値は書き込まれません。これは、X ヘッダーが、ユーザーのメールボックスの名前付きプロパティに最初にマップされる必要があるためです。このマッピングは、名前付きプロパティを追加するための最初の要求時に発生します。名前付きプロパティを作成する後続の要求が発生すると、プロパティと値はメッセージに格納されます。Exchange 2007 では、X ヘッダーが最初にメールボックス データベースに書き込まれます。その際に、メールボックス データベースにおける名前付きプロパティに対する X ヘッダーのマッピングが作成されます。名前付きプロパティを作成する後続の要求が発生すると、X ヘッダーが処理されて、Exchange 2007 データベースのメールボックス用に格納されます。
  
## <a name="next-steps"></a>次の手順
<a name="bk_example1"> </a>

この資料では、ユーザーに電子メールを送信してメールボックスを 1 つの x ヘッダーを提供する方法を説明します。 多くのユーザーの x ヘッダーは、呼び出し元の組織内の[受信者のリストをバッチの電子メールを送信する](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)でもプロビジョニングできます。 
  
## <a name="see-also"></a>関連項目


- [Exchange における EWS のプロパティと拡張プロパティ](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Exchange 2013: プログラムでカスタム X ヘッダーを提供します。](http://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [名前付きプロパティは、X-ヘッダーとします。](http://blogs.technet.com/b/exchange/archive/2009/04/06/3407221.aspx)
    
- [名前付きプロパティでは、ラウンド 2: どのような配置先](http://blogs.technet.com/b/exchange/archive/2009/06/12/3407672.aspx)
    
- [ヘッダー ファイアウォール](http://technet.microsoft.com/en-us/library/bb232136%28v=exchg.150%29.aspx)
    
- [EWS、MIME、および不足しているインターネット メッセージのヘッダー](http://msdn.microsoft.com/library/office/hh545614%28v=exchg.140%29.aspx)
    
- [電子メール メッセージを Exchange で EWS を使用してバッチ プロセス](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    

