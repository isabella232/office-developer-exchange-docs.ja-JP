---
title: Exchange 2013 の EWS を使用してあいまいな名前を解決するには
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1ba21c54-ecd2-4a1e-80d4-0f4171dea84f
description: Active Directory ドメイン サービス (AD DS) や、ユーザーのメールボックスの連絡先フォルダーから候補を取得することにより、あいまいな名前を解決するのには、EWS のマネージ API または EWS を使用する方法について説明します。
ms.openlocfilehash: 05a88043083a27d2e6d445cd71e5f3919c5a775d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759047"
---
# <a name="resolve-ambiguous-names-by-using-ews-in-exchange-2013"></a>Exchange 2013 の EWS を使用してあいまいな名前を解決するには

Active Directory ドメイン サービス (AD DS) や、ユーザーのメールボックスの連絡先フォルダーから候補を取得することにより、あいまいな名前を解決するのには、EWS のマネージ API または EWS を使用する方法について説明します。
  
組織内のユーザーには、トレーニング ・ セッションに参加する従業員の名前と住所の手書きのリストが与えられます。 リストで、ユーザーにいくつか追加の情報を使用して電子メールを送信するが、これらすべてのユーザーの電子メール アドレスを読み取ることができません。 アプリケーションでユーザーにこの問題を解決する場合は、EWS が役立つことがあります。 [ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) EWS のマネージ API のメソッドまたは[ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS の操作を使用するには、最後の名前の一部などのテキストの選択範囲の潜在的な候補の一覧を返します。 返される項目には、パブリックのユーザーのメールボックス、配布グループ、および取引先担当者を指定できます。 
  
Exchange がプレフィックスが付けられたルーティングの種類、smtp など、複数値配列内の sip 電子メール アドレスを保存することに注意してください。 **ResolveName**メソッドと**ResolveNames**操作は、ルーティングの種類を「sip: User1」など、未解決の名前の先頭に追加すると、その配列各値に対して部分的に一致するを実行します。 ルーティングの種類を指定しない場合メソッドまたは操作は既定の smtp プライマリ smtp アドレスのプロパティに一致して、複数値の配列を検索します。 たとえば、User1 を検索して sip のプレフィックスが含まれていない場合を受け取りません sip:User1@Contoso.com その結果、有効なメールボックスがある場合でも。 
  
あいまいな名前の 1 つは、1 つの要求でのみ指定できます。 解決するのにはあいまいな名前のリストがある場合、ボックスの一覧をループ処理し、メソッドまたは各エントリの操作を呼び出す必要があります。 ユーザーの連絡先フォルダーからの候補者は、追加情報を取得するために[Contact.Bind](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx)メソッドの呼び出しまたは[GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx)操作の要求で、使用する非 null のアイテム ID の値があります。 候補者が配布グループの場合は、メンバーの一覧を取得するのには[ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx)の EWS のマネージ API のメソッドまたは[ExpandDL](http://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx)の EWS の操作を使用できます。 _ReturnContactDetails_パラメーターまたは EWS の**ReturnFullContactData**属性の true に設定、 **ResolveName**メソッドを使用して Active Directory エントリが返されるか、 **ResolveNames**操作には追加のプロパティは、連絡先を記述するとします。 _ReturnContactDetails_パラメーターまたは**ReturnFullContactData**属性は連絡先で返されるデータには影響されず、グループにお問い合わせください。 
  
## <a name="resolve-ambiguous-names-by-using-ews-managed-api"></a>EWS マネージ API を使用して、あいまいな名前を解決する
<a name="bk_EWSMA"> </a>

[ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx)メソッドを使用すると、渡されるあいまいな名前に一致する候補を検索します。 **ResolveName**メソッドのオーバー ロードを使用すると、5 つの方法で候補を検索します。 
  
**表 1 です。ResolveName メソッドのオーバー ロードされました。**

|**メソッド**|**しくみ**|
|:-----|:-----|
|[ResolveName(String)](http://msdn.microsoft.com/en-us/library/dd635548%28v=exchg.80%29.aspx) <br/> |ユーザーの連絡先フォルダーにある連絡先、およびグローバル アドレス一覧 (GAL) にある連絡先を、この順番で検索します。その文字列変数は、解決しようとしているあいまいな名前です。  <br/> |
|[ResolveName (文字列、ResolveNameSearchLocation、ブール値)](http://msdn.microsoft.com/en-us/library/dd634595%28v=exchg.80%29.aspx) <br/> |既定の連絡先フォルダーにある連絡先と、グローバル アドレス一覧 (GAL) にある連絡先の一方または両方を検索します。文字列値はあいまいな名前で、検索場所は連絡先フォルダーとグローバル アドレス一覧の一方または両方を指定し、ブール値は連絡先の全情報を返すかどうかを示します。  <br/> |
|[ResolveName (文字列、ResolveNameSearchLocation、ブール値、プロパティ設定)](http://msdn.microsoft.com/en-us/library/hh532803%28v=exchg.80%29.aspx) <br/> |既定の連絡先フォルダーにある連絡先と、グローバル アドレス一覧 (GAL) にある連絡先の一方または両方を検索します。このメソッドを使用すると、返されるプロパティを設定できます。  <br/> |
|[ResolveName (文字列、IEnumerable\<フォルダー Id\>、ResolveNameSearchLocation、ブール値)](http://msdn.microsoft.com/en-us/library/dd636014%28v=exchg.80%29.aspx) <br/> |指定した連絡先フォルダーにある連絡先と、グローバル アドレス一覧 (GAL) にある連絡先の一方または両方を検索します。このメソッドを利用して、検索するフォルダーのコレクションを渡すことができます。これにより、既定の連絡先フォルダー以外の連絡先フォルダーを検索することができます。  <br/> |
|[ResolveName (文字列、IEnumerable\<フォルダー Id\>、ResolveNameSearchLocation、ブール値、プロパティ設定)](http://msdn.microsoft.com/en-us/library/hh532581%28v=exchg.80%29.aspx) <br/> |グローバル アドレス一覧 (GAL) にある連絡先と、指定した連絡先フォルダーにある連絡先の一方または両方を検索します。このメソッドを使用すると、返されるプロパティを設定できます。  <br/> |
   
簡単な例から始めましょう。 次の例では、"dan という"テキスト文字列を解決するには、検出されたそれぞれの応募者の名前と電子メール アドレスを出力する方法を示します。 この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。 
  
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

応答は、100 以上の候補があるかもしれませんが、100 の候補の最大を返します。 多くの候補者の最初の 100 個の候補のみが返されたかどうかを確認するのには、 [NameResolutionCollection](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx)オブジェクトの[IncludesAllResolutions](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx)の値を確認します。 値が true の場合はこれ以上の候補です。値が false の場合は、メソッドより多くの潜在的な候補者の最初の 100 人だけ返されます。 
  
大規模な組織で作業している場合に、"dan"などの名前が 100 の候補の最大数を返すことが可能性があります。 返される候補の数を減らすためには、検索する場所を制限します。 次の例では、あいまいな名前を解決するのには検索するのに場所を指定するのに[ResolveNameSearchLocation](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx)列挙体を使用します。 
  
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

既知の連絡先フォルダー以外のフォルダーに連絡先を格納する場合は、候補を検索する場所を指定するオーバー ロードされたメソッドのいずれかを使用します。 **ResolveName**メソッドがフォルダーの ID を基にフォルダー一覧を作成する例を次 **フォルダー Id**が小さすぎると読みやすくするためです。 
  
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

フィルターを適用すると、候補が返されない、 [NameResolutionCollection](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx)には 0 個のエントリが含まれます。 コレクションの[Count](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx)プロパティを参照して、これを確認することができます。 
  
## <a name="resolve-ambiguous-names-by-using-ews"></a>EWS を使用して、あいまいな名前を解決します
<a name="bk_EWSMA"> </a>

[ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS の操作を使用するにはあいまいな名前の候補を識別します。 [UnresolvedEntry](http://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx)要素には、解決する場合、あいまいな名前が含まれています。 Sadie の名前を解決するのには次の例を次に示します。 [ResolveName メソッドを使用して](#bk_EWSMA)、it 部門以外は、有効な出力の例については別の名前を使用する場合、EWS のマネージ API を使用している XML の要求にもです。
  
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
      <UnresolvedEntry>Sadie</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

応答より多くの候補者の最初の 100 個の候補のみが返されたかどうかを決定する、 [IncludesLastItemInRange](http://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx)の値を確認する 100 以上の候補があるかもしれませんが、100 の候補の最大を返します[ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx)要素の属性です。 値が true の場合はこれ以上の候補です。値が false の場合は、操作より多くの潜在的な候補者の最初の 100 人だけ返されます。 
  
次の例は、1 つの候補が見つかった場合、XML 応答を示します。 ただし、 [ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx)は、[解像度](http://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx)の要素とその子要素を表す、最大 100 個の候補者を含めることができます。 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
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
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
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

## <a name="see-also"></a>関連項目


- [Exchange 内の EWS のユーザーと連絡先](people-and-contacts-in-ews-in-exchange.md)
    
- [Exchange 2013 の EWS を使用して配布グループを展開します。](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

