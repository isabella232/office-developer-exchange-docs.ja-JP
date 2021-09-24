---
title: Exchange 2013 の EWS を使用して、あいまいな名前を解決する
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 1ba21c54-ecd2-4a1e-80d4-0f4171dea84f
description: EWS マネージ API または EWS を使用して、Active Directory ドメイン サービス (AD DS) や、ユーザーのメールボックスの連絡先フォルダーから候補を取得し、あいまいな名前を解決する方法について説明します。
ms.openlocfilehash: 5946dad32639b454b3961eaa172b6069ce118b58
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521124"
---
# <a name="resolve-ambiguous-names-by-using-ews-in-exchange-2013"></a>Exchange 2013 の EWS を使用して、あいまいな名前を解決する

EWS マネージ API または EWS を使用して、Active Directory ドメイン サービス (AD DS) や、ユーザーのメールボックスの連絡先フォルダーから候補を取得し、あいまいな名前を解決する方法について説明します。
  
組織内のユーザーには、トレーニング セッションに参加した従業員の名前と住所を記した手書きのリストが渡されます。 リストに記載された人物に電子メールで何らかの追加情報を発信したいと思っても、すべてのユーザーの電子メール アドレスを読み取ることはできません。 アプリケーションのユーザーに代わり、この問題を解決したい場合は、EWS が役立つことがあります。 [ExchangeService.ResolveName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) EWS マネージ API メソッド、または [ResolveNames](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS 操作を使用して、姓の一部など、テキストの一部に一致する候補のリストを返すことができます。 返されるアイテムは、パブリックのユーザー メールボックス、配布グループ、および連絡先である場合があります。 
  
Exchange は、複数値配列内の smtp や sip などのルーティングの種類を先頭につけて、電子メール アドレスを保存しますので、ご注意ください。 未解決の名前の先頭に、「sip:User1」などのルーティングの種類を付け加えた場合、**ResolveName** メソッドや **ResolveNames** 操作は、その配列の各値の部分一致を実施します。 ルーティングの種類を指定しない場合、メソッドまたは操作の既定値は smtp となり、プライマリ smtp アドレス プロパティに一致させ、複数値配列は検索しません。 たとえば、User1 を検索して sip のプレフィックスを含めない場合は、有効なメールボックスであっても、sip:User1@Contoso.com を検索結果として受け取ることはありません。 
  
要求 1 つに対して、あいまいな名前は 1 つしか指定できません。 解決が必要なあいまいな名前の一覧がある場合、一覧をループ処理し、各エントリのメソッドまたは操作を呼び出す必要があります。 ユーザーの連絡先フォルダーにある候補のアイテム ID 値は null 以外となり、その ID 値は [Contact.Bind](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) メソッドの呼び出し、または追加情報を取得するための [GetItem](https://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) 操作要求に使用できます。 その候補が配布グループの場合、[ExpandGroup(ItemId)](https://msdn.microsoft.com/library/office/ee356407%28v=exchg.80%29.aspx) EWS マネージ API メソッド、または [ExpandDL](https://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx) EWS 操作を使用して、メンバーの一覧を取得できます。 _returnContactDetails_ パラメーター、または **ReturnFullContactData** EWS 属性が true に設定されている場合、**ResolveName** メソッドまたは **ResolveNames** 操作が返す Active Directory のエントリには、連絡先を記す追加プロパティが含まれます。 _returnContactDetails_ パラメーター、または **ReturnFullContactData** 属性は、連絡先用および連絡先グループ用に返されるデータに影響をおよぼしません。 
  
## <a name="resolve-ambiguous-names-by-using-ews-managed-api"></a>EWS マネージ API を使用して、あいまいな名前を解決する
<a name="bk_EWSMA"> </a>

[ResolveName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) メソッドを使用して、渡されるあいまいな名前に一致する候補を検索します。 **ResolveName** メソッドのオーバーロードを使用して、5 通りの方法で候補を検索できます。 
  
**表 1. オーバーロードされた ResolveName メソッド**

|**メソッド**|**動作のしくみ**|
|:-----|:-----|
|[ResolveName(String)](https://msdn.microsoft.com/library/dd635548%28v=exchg.80%29.aspx) <br/> |ユーザーの連絡先フォルダーにある連絡先、およびグローバル アドレス一覧 (GAL) にある連絡先を、この順番で検索します。その文字列変数は、解決しようとしているあいまいな名前です。  <br/> |
|[ResolveName(String, ResolveNameSearchLocation, Boolean)](https://msdn.microsoft.com/library/dd634595%28v=exchg.80%29.aspx) <br/> |既定の連絡先フォルダーにある連絡先と、グローバル アドレス一覧 (GAL) にある連絡先の一方または両方を検索します。文字列値はあいまいな名前で、検索場所は連絡先フォルダーとグローバル アドレス一覧の一方または両方を指定し、ブール値は連絡先の全情報を返すかどうかを示します。  <br/> |
|[ResolveName(String, ResolveNameSearchLocation, Boolean, PropertySet)](https://msdn.microsoft.com/library/hh532803%28v=exchg.80%29.aspx) <br/> |既定の連絡先フォルダーにある連絡先と、グローバル アドレス一覧 (GAL) にある連絡先の一方または両方を検索します。このメソッドを使用すると、返されるプロパティを設定できます。  <br/> |
|[ResolveName(String, IEnumerable \<FolderId\> , ResolveNameSearchLocation, Boolean)](https://msdn.microsoft.com/library/dd636014%28v=exchg.80%29.aspx) <br/> |指定した連絡先フォルダーにある連絡先と、グローバル アドレス一覧 (GAL) にある連絡先の一方または両方を検索します。このメソッドを利用して、検索するフォルダーのコレクションを渡すことができます。これにより、既定の連絡先フォルダー以外の連絡先フォルダーを検索することができます。  <br/> |
|[ResolveName(String, IEnumerable \<FolderId\> , ResolveNameSearchLocation, Boolean, PropertySet)](https://msdn.microsoft.com/library/hh532581%28v=exchg.80%29.aspx) <br/> |グローバル アドレス一覧 (GAL) にある連絡先と、指定した連絡先フォルダーにある連絡先の一方または両方を検索します。このメソッドを使用すると、返されるプロパティを設定できます。  <br/> |
   
簡単な例から始めましょう。 次の例では、「dan」というテキスト文字列を解決して、検索された各候補の名前と電子メール アドレスを出力する方法を示します。 この例では、**service** が有効な [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。 
  
```cs
// Resolve the ambiguous name "dan".
   NameResolutionCollection resolvedNames = service.ResolveName("dan");
   // Output the list of candidates.
   foreach (NameResolution nameRes in resolvedNames)
   {
      Console.WriteLine("Contact name: " + nameRes.Mailbox.Name);
      Console.WriteLine("Contact e-mail address: " + nameRes.Mailbox.Address);
      Console.WriteLine("Mailbox type: " + nameRes.Mailbox.MailboxType);
   }

```

100 を超える候補が存在する場合でも、この応答は最大で 100 候補しか返しません。 より多くの候補から最初の 100 候補だけが返されたのかどうかを判定するには、[NameResolutionCollection](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) オブジェクトの [IncludesAllResolutions](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx) の値を確認してください。 値が true の場合は、これ以上の候補は存在しません。値が false の場合は、このメソッドはより多くの潜在的候補から最初の 100 候補だけを返しました。 
  
大規模な組織で働いている場合は、「dan」などの名前は最大数の 100 候補を返すことがあり得ます。 返す候補数を少なくするには、検索先を絞ってください。 次の例では、[ResolveNameSearchLocation](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx) 列挙体を使用して検索先を指定し、あいまいな名前を解決します。 
  
```cs
// Resolve the ambiguous name "dan".
// Only use the Contacts folder.
   NameResolutionCollection resolvedNames = service.ResolveName("dan", ResolveNameSearchLocation.ContactsOnly, false);
   // Output the list of candidates.   
   foreach (NameResolution nameRes in resolvedNames)
   {
      Console.WriteLine("Contact name: " + nameRes.Mailbox.Name);
      Console.WriteLine("Contact e-mail address: " + nameRes.Mailbox.Address);
      Console.WriteLine("Mailbox type: " + nameRes.Mailbox.MailboxType);
   }

```

既知の連絡先フォルダー以外のフォルダーに連絡先を格納する場合は、オーバーロードされたメソッドのいずれかを使用して、候補の検索先を指定してください。次の例では、フォルダー ID に基づいて **ResolveName** メソッド用のフォルダー一覧を作成します。**FolderId** は読みやすいように短縮されています。 
  
```cs
// Create a list to store folders to search.
List<FolderId> folders = new List<FolderId>();
// Add a folder to the list based on the FolderId.
folders.Add(new FolderId("AABR8mboAAA="));
// Resolve the ambiguous name "dan".
// Only use the folders specified.
NameResolutionCollection resolvedNames = service.ResolveName("dan", folders, ResolveNameSearchLocation.ContactsOnly, false);
   foreach (NameResolution nameRes in resolvedNames)
   {
      Console.WriteLine("Contact name: " + nameRes.Mailbox.Name);
      Console.WriteLine("Contact e-mail address: " + nameRes.Mailbox.Address);
      Console.WriteLine("Mailbox type: " + nameRes.Mailbox.MailboxType);
   }

```

フィルターを適用して候補が返されない場合、[NameResolutionCollection](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) にはエントリは含まれません。 コレクションの [Count](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx) プロパティを参照して、これを確認することができます。 
  
## <a name="resolve-ambiguous-names-by-using-ews"></a>EWS を使用して、あいまいな名前を解決します
<a name="bk_EWSMA"> </a>

[ResolveName](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS 操作を使用して、あいまいな名前の候補を特定します。[UnresolvedEntry](https://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx) 要素は、解決したいあいまいな名前を含んでいます。次の例は、Sadie という名前を解決する方法を示しています。これは、有効な出力例に異なる名前を使用する場合以外で、[ResolveName メソッドを使用する](#bk_EWSMA)場合に EWS マネージ API が使用する XML 要求でもあります。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>Sadie</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

100 を超える候補が存在する場合でも、この応答は最大で 100 候補しか返しません。より多くの候補から最初の 100 候補だけが返されたどうかを判定するには、[ResolutionSet](https://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) 要素の[IncludesLastItemInRange](https://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx) 属性の値を確認してください。値が true の場合は、これ以上の候補は存在しません。値が false の場合は、この操作はより多くの潜在的候補から最初の 100 候補だけを返しました。 
  
次の例では、1 候補が検出された場合の XML 応答を示しています。[ResolutionSet](https://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) は最大で 100 候補を含めることができ、各候補は [Resolution](https://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx) 要素とその子要素で表されていることを、覚えておいてください。 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
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
                <t:Name>Sadie Daniels</t:Name>
                <t:EmailAddress>Sadie@Contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Mailbox</t:MailboxType>
              </t:Mailbox>
              <t:Contact>
                <t:DisplayName>Sadie Daniels</t:DisplayName>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress1">SMTP:Sadie@Contoso.com</t:Entry>
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

あいまいな名前の候補がいつも検索できるとは限りません。次の例では、候補が見つからなかった場合に、エラーとして返される XML 応答を示しています。
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
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

## <a name="see-also"></a>関連項目


- [Exchange 内の EWS のユーザーと連絡先](people-and-contacts-in-ews-in-exchange.md)
    
- [Exchange 2013 の EWS を使用して配布グループを展開する](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

