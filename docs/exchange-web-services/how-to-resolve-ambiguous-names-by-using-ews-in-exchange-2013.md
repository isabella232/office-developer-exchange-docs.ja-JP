---
title: Exchange 2013 の EWS を使用して、あいまいな名前を解決する
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1ba21c54-ecd2-4a1e-80d4-0f4171dea84f
description: EWS マネージ API または EWS を使用して、Active Directory ドメイン サービス (AD DS) や、ユーザーのメールボックスの連絡先フォルダーから候補を取得し、あいまいな名前を解決する方法について説明します。
ms.openlocfilehash: 05a88043083a27d2e6d445cd71e5f3919c5a775d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759047"
---
# <a name="resolve-ambiguous-names-by-using-ews-in-exchange-2013"></a><span data-ttu-id="2e8ec-103">Exchange 2013 の EWS を使用して、あいまいな名前を解決する</span><span class="sxs-lookup"><span data-stu-id="2e8ec-103">How to: Resolve ambiguous names by using EWS in Exchange 2013</span></span>

<span data-ttu-id="2e8ec-104">EWS マネージ API または EWS を使用して、Active Directory ドメイン サービス (AD DS) や、ユーザーのメールボックスの連絡先フォルダーから候補を取得し、あいまいな名前を解決する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-104">Learn how to use the EWS Managed API or EWS to resolve ambiguous names by getting possible matches from Active Directory Domain Services (AD DS) or a contacts folder in your user's mailbox.</span></span>
  
<span data-ttu-id="2e8ec-105">組織内のユーザーには、トレーニング セッションに参加した従業員の名前と住所を記した手書きのリストが渡されます。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-105">A user in your organization is given a hand-written list of names and addresses for employees that attended a training session.</span></span> <span data-ttu-id="2e8ec-106">リストに記載された人物に電子メールで何らかの追加情報を発信したいと思っても、すべてのユーザーの電子メール アドレスを読み取ることはできません。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-106">They want to send an email with some additional information to people on the list, but they can't read everyone's email address.</span></span> <span data-ttu-id="2e8ec-107">アプリケーションのユーザーに代わり、この問題を解決したい場合は、EWS が役立つことがあります。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-107">If you want to solve this problem for your users in your application, EWS can help.</span></span> <span data-ttu-id="2e8ec-108">[ExchangeService.ResolveName](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) EWS マネージ API メソッド、または [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS 操作を使用して、姓の一部など、テキストの一部に一致する候補のリストを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-108">You can use the [ExchangeService.ResolveName](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) EWS Managed API method or the [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS operation to return a list of potential matches for a selection of text, such as part of a last name.</span></span> <span data-ttu-id="2e8ec-109">返されるアイテムは、パブリックのユーザー メールボックス、配布グループ、および連絡先である場合があります。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-109">The returned items can be public user mailboxes, distribution groups, and contacts.</span></span> 
  
<span data-ttu-id="2e8ec-110">Exchange は、複数値配列内の smtp や sip などのルーティングの種類を先頭につけて、電子メール アドレスを保存しますので、ご注意ください。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-110">Note that Exchange saves email addresses with prefixed routing types, such as smtp or sip, in a multivalue array.</span></span> <span data-ttu-id="2e8ec-111">未解決の名前の先頭に、「sip:User1」などのルーティングの種類を付け加えた場合、**ResolveName** メソッドや **ResolveNames** 操作は、その配列の各値の部分一致を実施します。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-111">The **ResolveName** method and the **ResolveNames** operation perform a partial match against each value of that array when you add the routing type at the beginning of the unresolved name, such as "sip:User1".</span></span> <span data-ttu-id="2e8ec-112">ルーティングの種類を指定しない場合、メソッドまたは操作の既定値は smtp となり、プライマリ smtp アドレス プロパティに一致させ、複数値配列は検索しません。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-112">If you don't specify a routing type, the method or operation will default to smtp, match it to a primary smtp address property, and not search the multivalue array.</span></span> <span data-ttu-id="2e8ec-113">たとえば、User1 を検索して sip のプレフィックスを含めない場合は、有効なメールボックスであっても、sip:User1@Contoso.com を検索結果として受け取ることはありません。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-113">For example, if you search for User1 and do not include the sip prefix, you will not receive sip:User1@Contoso.com as a result, even if that is a valid mailbox.</span></span> 
  
<span data-ttu-id="2e8ec-114">要求 1 つに対して、あいまいな名前は 1 つしか指定できません。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-114">You can only specify one ambiguous name in a single request.</span></span> <span data-ttu-id="2e8ec-115">解決が必要なあいまいな名前の一覧がある場合、一覧をループ処理し、各エントリのメソッドまたは操作を呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-115">If you have a list of ambiguous names to resolve, you will need to loop through the list and call the method or operation for each entry.</span></span> <span data-ttu-id="2e8ec-116">ユーザーの連絡先フォルダーにある候補のアイテム ID 値は null 以外となり、その ID 値は [Contact.Bind](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) メソッドの呼び出し、または追加情報を取得するための [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) 操作要求に使用できます。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-116">Candidates from a user's Contacts folder will have a non-null item ID value, which can then be used in a [Contact.Bind](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) method call or [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) operation request to retrieve additional information.</span></span> <span data-ttu-id="2e8ec-117">その候補が配布グループの場合、[ExpandGroup(ItemId)](http://msdn.microsoft.com/ja-JP/library/office/ee356407%28v=exchg.80%29.aspx) EWS マネージ API メソッド、または [ExpandDL](http://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx) EWS 操作を使用して、メンバーの一覧を取得できます。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-117">If the candidate is a distribution group, you can use the [ExpandGroup(ItemId)](http://msdn.microsoft.com/ja-JP/library/office/ee356407%28v=exchg.80%29.aspx) EWS Managed API method or the [ExpandDL](http://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx) EWS operation to get the list of members.</span></span> <span data-ttu-id="2e8ec-118">_returnContactDetails_ パラメーター、または **ReturnFullContactData** EWS 属性が true に設定されている場合、**ResolveName** メソッドまたは **ResolveNames** 操作が返す Active Directory のエントリには、連絡先を記す追加プロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-118">If the  _returnContactDetails_ parameter or the **ReturnFullContactData** EWS attribute is set to true, Active Directory entries returned via a **ResolveName** method or **ResolveNames** operation will include additional properties that describe the contact.</span></span> <span data-ttu-id="2e8ec-119">_returnContactDetails_ パラメーター、または **ReturnFullContactData** 属性は、連絡先用および連絡先グループ用に返されるデータに影響をおよぼしません。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-119">The  _returnContactDetails_ parameter or the **ReturnFullContactData** attribute does not affect the data that is returned for contacts and contact groups.</span></span> 
  
## <a name="resolve-ambiguous-names-by-using-ews-managed-api"></a><span data-ttu-id="2e8ec-120">EWS マネージ API を使用して、あいまいな名前を解決する</span><span class="sxs-lookup"><span data-stu-id="2e8ec-120">Resolve ambiguous names by using EWS Managed API</span></span>
<span data-ttu-id="2e8ec-121"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="2e8ec-121"></span></span>

<span data-ttu-id="2e8ec-122">[ResolveName](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) メソッドを使用して、渡されるあいまいな名前に一致する候補を検索します。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-122">You can use the [ResolveName](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) method to find candidates that match the ambiguous name you pass.</span></span> <span data-ttu-id="2e8ec-123">**ResolveName** メソッドのオーバーロードを使用して、5 通りの方法で候補を検索できます。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-123">You can use overloads of the **ResolveName** method to search for candidates in five different ways.</span></span> 
  
<span data-ttu-id="2e8ec-124">** 表 1. オーバーロードされた ResolveName メソッド**</span><span class="sxs-lookup"><span data-stu-id="2e8ec-124">**Table 1. Overloaded ResolveName methods**</span></span>

|<span data-ttu-id="2e8ec-125">**メソッド**</span><span class="sxs-lookup"><span data-stu-id="2e8ec-125">**Method**</span></span>|<span data-ttu-id="2e8ec-126">**動作のしくみ**</span><span class="sxs-lookup"><span data-stu-id="2e8ec-126">**How it works**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2e8ec-127">ResolveName(String)</span><span class="sxs-lookup"><span data-stu-id="2e8ec-127">ResolveName(String)</span></span>](http://msdn.microsoft.com/ja-JP/library/dd635548%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="2e8ec-p105">ユーザーの連絡先フォルダーにある連絡先、およびグローバル アドレス一覧 (GAL) にある連絡先を、この順番で検索します。その文字列変数は、解決しようとしているあいまいな名前です。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-p105">Finds contacts in the user's Contacts folder and the Global Address List (GAL) — in that order. The string variable is the ambiguous name you are trying to resolve.</span></span>  <br/> |
|[<span data-ttu-id="2e8ec-130">ResolveName(String, ResolveNameSearchLocation, Boolean)</span><span class="sxs-lookup"><span data-stu-id="2e8ec-130">ResolveName(String, ResolveNameSearchLocation, Boolean)</span></span>](http://msdn.microsoft.com/ja-JP/library/dd634595%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="2e8ec-p106">既定の連絡先フォルダーにある連絡先と、グローバル アドレス一覧 (GAL) にある連絡先の一方または両方を検索します。文字列値はあいまいな名前で、検索場所は連絡先フォルダーとグローバル アドレス一覧の一方または両方を指定し、ブール値は連絡先の全情報を返すかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-p106">Finds contacts in the default Contacts folder and/or the Global Address List (GAL). The string value is the ambiguous name, the search location specifies the Contacts folder and/or the GAL, and the Boolean value indicates whether to return the full contact information.</span></span>  <br/> |
|[<span data-ttu-id="2e8ec-133">ResolveName(String, ResolveNameSearchLocation, Boolean, PropertySet)</span><span class="sxs-lookup"><span data-stu-id="2e8ec-133">ResolveName(String, ResolveNameSearchLocation, Boolean, PropertySet)</span></span>](http://msdn.microsoft.com/ja-JP/library/hh532803%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="2e8ec-p107">既定の連絡先フォルダーにある連絡先と、グローバル アドレス一覧 (GAL) にある連絡先の一方または両方を検索します。このメソッドを使用すると、返されるプロパティを設定できます。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-p107">Finds contacts in the default Contacts folder and/or Global Address List (GAL). This method enables you to set the properties that are returned.</span></span>  <br/> |
|[<span data-ttu-id="2e8ec-136">ResolveName(String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean)</span><span class="sxs-lookup"><span data-stu-id="2e8ec-136">ResolveName(String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean)</span></span>](http://msdn.microsoft.com/ja-JP/library/dd636014%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="2e8ec-p108">指定した連絡先フォルダーにある連絡先と、グローバル アドレス一覧 (GAL) にある連絡先の一方または両方を検索します。このメソッドを利用して、検索するフォルダーのコレクションを渡すことができます。これにより、既定の連絡先フォルダー以外の連絡先フォルダーを検索することができます。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-p108">Finds contacts in specified contact folders and/or the Global Address List (GAL). You can use this method to pass a collection of folders to search. This enables you to look in contact folders other than the default Contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="2e8ec-140">ResolveName(String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean, PropertySet)</span><span class="sxs-lookup"><span data-stu-id="2e8ec-140">ResolveName(String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean, PropertySet)</span></span>](http://msdn.microsoft.com/ja-JP/library/hh532581%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="2e8ec-p109">グローバル アドレス一覧 (GAL) にある連絡先と、指定した連絡先フォルダーにある連絡先の一方または両方を検索します。このメソッドを使用すると、返されるプロパティを設定できます。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-p109">Finds contacts in the Global Address List (GAL) and/or in specific contact folders. This method enables you to set the properties that are returned.</span></span>  <br/> |
   
<span data-ttu-id="2e8ec-143">簡単な例から始めましょう。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-143">Let's start with a simple example.</span></span> <span data-ttu-id="2e8ec-144">次の例では、「dan」というテキスト文字列を解決して、検索された各候補の名前と電子メール アドレスを出力する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-144">The following example shows how to resolve the text string "dan" and output the name and email address of each candidate found.</span></span> <span data-ttu-id="2e8ec-145">この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-145">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

<span data-ttu-id="2e8ec-146">100 を超える候補が存在する場合でも、この応答は最大で 100 候補しか返しません。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-146">The response returns a maximum of 100 candidates, although there might be more than 100 potential candidates.</span></span> <span data-ttu-id="2e8ec-147">より多くの候補から最初の 100 候補だけが返されたのかどうかを判定するには、[NameResolutionCollection](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) オブジェクトの [IncludesAllResolutions](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx) の値を確認してください。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-147">To determine whether only the first 100 candidates of a larger number of candidates were returned, check the value of [IncludesAllResolutions](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx) in the [NameResolutionCollection](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) object.</span></span> <span data-ttu-id="2e8ec-148">値が true の場合は、これ以上の候補は存在しません。値が false の場合は、このメソッドはより多くの潜在的候補から最初の 100 候補だけを返しました。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-148">If the value is true, there are no more possible candidates; if the value is false, the method only returned the first 100 of a larger number of potential candidates.</span></span> 
  
<span data-ttu-id="2e8ec-149">大規模な組織で働いている場合は、「dan」などの名前は最大数の 100 候補を返すことがあり得ます。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-149">If you work in a large organization, it's likely that a name like "dan" will return the maximum number of 100 candidates.</span></span> <span data-ttu-id="2e8ec-150">返す候補数を少なくするには、検索先を絞ってください。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-150">To reduce the number of candidates returned, limit where you search.</span></span> <span data-ttu-id="2e8ec-151">次の例では、[ResolveNameSearchLocation](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx) 列挙体を使用して検索先を指定し、あいまいな名前を解決します。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-151">The next example uses the [ResolveNameSearchLocation](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx) enumeration to specify where to search to resolve the ambiguous name.</span></span> 
  
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

<span data-ttu-id="2e8ec-152">既知の連絡先フォルダー以外のフォルダーに連絡先を格納する場合は、オーバーロードされたメソッドのいずれかを使用して、候補の検索先を指定してください。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-152">If you store your contacts in a folder other than the well-known Contacts folder, use one of the overloaded methods to specify where to look for candidates. The following example creates a folder list for the ResolveName method based on the folder ID. The FolderId has been shortened for readability.</span></span> <span data-ttu-id="2e8ec-153">次の例では、フォルダー ID に基づいて **ResolveName** メソッド用のフォルダー一覧を作成します。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-153">The following example creates a folder list for the **ResolveName** method based on the folder ID.</span></span> <span data-ttu-id="2e8ec-154">**FolderId** は、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-154">The ItemId value has been shortened for readability.</span></span> 
  
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

<span data-ttu-id="2e8ec-155">フィルターを適用して候補が返されない場合、[NameResolutionCollection](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) にはエントリは含まれません。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-155">If you apply filters and no candidates are returned, the [NameResolutionCollection](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) will contain zero entries.</span></span> <span data-ttu-id="2e8ec-156">コレクションの [Count](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx) プロパティを参照して、これを確認することができます。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-156">You can verify this by looking at the [Count](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx) property of the collection.</span></span> 
  
## <a name="resolve-ambiguous-names-by-using-ews"></a><span data-ttu-id="2e8ec-157">EWS を使用して、あいまいな名前を解決します</span><span class="sxs-lookup"><span data-stu-id="2e8ec-157">Resolve ambiguous names by using EWS</span></span>
<span data-ttu-id="2e8ec-158"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="2e8ec-158"></span></span>

<span data-ttu-id="2e8ec-159">[ResolveName](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS 操作を使用して、あいまいな名前の候補を特定します。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-159">You can use the [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS operation to identify possible candidates for an ambiguous name.</span></span> <span data-ttu-id="2e8ec-160">[UnresolvedEntry](http://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx) 要素は、解決したいあいまいな名前を含んでいます。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-160">The [UnresolvedEntry](http://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx) element contains the ambiguous name you want to resolve.</span></span> <span data-ttu-id="2e8ec-161">次の例は、Sadie という名前を解決する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-161">The following example shows how to resolve the name Sadie.</span></span> <span data-ttu-id="2e8ec-162">これは、有効な出力例に異なる名前を使用する場合以外で、[ResolveName メソッドを使用する](#bk_EWSMA)場合に EWS マネージ API が使用する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-162">You can use the ResolveNames EWS operation to identify possible candidates for an ambiguous name. The UnresolvedEntry element contains the ambiguous name you want to resolve. The following example shows how to resolve the name Sadie. This is also the XML request that the EWS Managed API uses when you [use the ResolveName method](#bk_EWSMA), except that it uses a different name for valid output examples.</span></span>
  
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

<span data-ttu-id="2e8ec-163">100 を超える候補が存在する場合でも、この応答は最大で 100 候補しか返しません。より多くの候補から最初の 100 候補だけが返されたどうかを判定するには、[ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) 要素の [IncludesLastItemInRange](http://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx) 属性の値を確認してください。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-163">The response returns a maximum of 100 candidates, although there might be more than 100 potential candidates To determine whether only the first 100 candidates of a larger number of candidates were returned, check the value of the [IncludesLastItemInRange](http://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx) attribute of the [ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) element. If the value is true, there are no more possible candidates; if the value is false, the operation only returned the first 100 of a larger number of potential candidates.</span></span> <span data-ttu-id="2e8ec-164">値が true の場合は、これ以上の候補は存在しません。値が false の場合は、この操作はより多くの潜在的候補から最初の 100 候補だけを返しました。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-164">If the value is true, there are no more possible candidates; if the value is false, the operation only returned the first 100 of a larger number of potential candidates.</span></span> 
  
<span data-ttu-id="2e8ec-165">次の例では、1 候補が検出された場合の XML 応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-165">The following example shows the XML response when one candidate is found.</span></span> <span data-ttu-id="2e8ec-166">[ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) は最大で 100 候補を含めることができ、各候補は [Resolution](http://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx) 要素とその子要素で表されていることを、覚えておいてください。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-166">The following example shows the XML response when one candidate is found. Remember, the [ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) can contain up to 100 candidates, each one represented by the [Resolution](http://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx) element and its child elements.</span></span> 
  
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

<span data-ttu-id="2e8ec-p118">あいまいな名前の候補がいつも検索できるとは限りません。次の例では、候補が見つからなかった場合に、エラーとして返される XML 応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="2e8ec-p118">You're not always going to come up with candidates for your ambiguous name. The following example shows the XML response, as an error, when no candidates are found.</span></span>
  
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

## <a name="see-also"></a><span data-ttu-id="2e8ec-169">関連項目</span><span class="sxs-lookup"><span data-stu-id="2e8ec-169">See also</span></span>


- [<span data-ttu-id="2e8ec-170">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="2e8ec-170">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)
    
- [<span data-ttu-id="2e8ec-171">Exchange 2013 の EWS を使用して配布グループを展開する</span><span class="sxs-lookup"><span data-stu-id="2e8ec-171">How to: Expand distribution groups by using EWS in Exchange 2013</span></span>](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

