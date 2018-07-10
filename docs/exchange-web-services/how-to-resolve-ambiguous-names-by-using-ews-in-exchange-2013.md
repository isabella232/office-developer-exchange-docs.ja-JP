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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759047"
---
# <a name="resolve-ambiguous-names-by-using-ews-in-exchange-2013"></a><span data-ttu-id="6d509-103">Exchange 2013 の EWS を使用してあいまいな名前を解決するには</span><span class="sxs-lookup"><span data-stu-id="6d509-103">Resolve ambiguous names by using EWS in Exchange 2013</span></span>

<span data-ttu-id="6d509-104">Active Directory ドメイン サービス (AD DS) や、ユーザーのメールボックスの連絡先フォルダーから候補を取得することにより、あいまいな名前を解決するのには、EWS のマネージ API または EWS を使用する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="6d509-104">Learn how to use the EWS Managed API or EWS to resolve ambiguous names by getting possible matches from Active Directory Domain Services (AD DS) or a contacts folder in your user's mailbox.</span></span>
  
<span data-ttu-id="6d509-105">組織内のユーザーには、トレーニング ・ セッションに参加する従業員の名前と住所の手書きのリストが与えられます。</span><span class="sxs-lookup"><span data-stu-id="6d509-105">A user in your organization is given a hand-written list of names and addresses for employees that attended a training session.</span></span> <span data-ttu-id="6d509-106">リストで、ユーザーにいくつか追加の情報を使用して電子メールを送信するが、これらすべてのユーザーの電子メール アドレスを読み取ることができません。</span><span class="sxs-lookup"><span data-stu-id="6d509-106">They want to send an email with some additional information to people on the list, but they can't read everyone's email address.</span></span> <span data-ttu-id="6d509-107">アプリケーションでユーザーにこの問題を解決する場合は、EWS が役立つことがあります。</span><span class="sxs-lookup"><span data-stu-id="6d509-107">If you want to solve this problem for your users in your application, EWS can help.</span></span> <span data-ttu-id="6d509-108">[ExchangeService.ResolveName](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) EWS のマネージ API のメソッドまたは[ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS の操作を使用するには、最後の名前の一部などのテキストの選択範囲の潜在的な候補の一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="6d509-108">You can use the [ExchangeService.ResolveName](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) EWS Managed API method or the [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS operation to return a list of potential matches for a selection of text, such as part of a last name.</span></span> <span data-ttu-id="6d509-109">返される項目には、パブリックのユーザーのメールボックス、配布グループ、および取引先担当者を指定できます。</span><span class="sxs-lookup"><span data-stu-id="6d509-109">The returned items can be public user mailboxes, distribution groups, and contacts.</span></span> 
  
<span data-ttu-id="6d509-110">Exchange がプレフィックスが付けられたルーティングの種類、smtp など、複数値配列内の sip 電子メール アドレスを保存することに注意してください。</span><span class="sxs-lookup"><span data-stu-id="6d509-110">Note that Exchange saves email addresses with prefixed routing types, such as smtp or sip, in a multivalue array.</span></span> <span data-ttu-id="6d509-111">**ResolveName**メソッドと**ResolveNames**操作は、ルーティングの種類を「sip: User1」など、未解決の名前の先頭に追加すると、その配列各値に対して部分的に一致するを実行します。</span><span class="sxs-lookup"><span data-stu-id="6d509-111">The **ResolveName** method and the **ResolveNames** operation perform a partial match against each value of that array when you add the routing type at the beginning of the unresolved name, such as "sip:User1".</span></span> <span data-ttu-id="6d509-112">ルーティングの種類を指定しない場合メソッドまたは操作は既定の smtp プライマリ smtp アドレスのプロパティに一致して、複数値の配列を検索します。</span><span class="sxs-lookup"><span data-stu-id="6d509-112">If you don't specify a routing type, the method or operation will default to smtp, match it to a primary smtp address property, and not search the multivalue array.</span></span> <span data-ttu-id="6d509-113">たとえば、User1 を検索して sip のプレフィックスが含まれていない場合を受け取りません sip:User1@Contoso.com その結果、有効なメールボックスがある場合でも。</span><span class="sxs-lookup"><span data-stu-id="6d509-113">For example, if you search for User1 and do not include the sip prefix, you will not receive sip:User1@Contoso.com as a result, even if that is a valid mailbox.</span></span> 
  
<span data-ttu-id="6d509-114">あいまいな名前の 1 つは、1 つの要求でのみ指定できます。</span><span class="sxs-lookup"><span data-stu-id="6d509-114">You can only specify one ambiguous name in a single request.</span></span> <span data-ttu-id="6d509-115">解決するのにはあいまいな名前のリストがある場合、ボックスの一覧をループ処理し、メソッドまたは各エントリの操作を呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="6d509-115">If you have a list of ambiguous names to resolve, you will need to loop through the list and call the method or operation for each entry.</span></span> <span data-ttu-id="6d509-116">ユーザーの連絡先フォルダーからの候補者は、追加情報を取得するために[Contact.Bind](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx)メソッドの呼び出しまたは[GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx)操作の要求で、使用する非 null のアイテム ID の値があります。</span><span class="sxs-lookup"><span data-stu-id="6d509-116">Candidates from a user's Contacts folder will have a non-null item ID value, which can then be used in a [Contact.Bind](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) method call or [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) operation request to retrieve additional information.</span></span> <span data-ttu-id="6d509-117">候補者が配布グループの場合は、メンバーの一覧を取得するのには[ExpandGroup(ItemId)](http://msdn.microsoft.com/ja-jp/library/office/ee356407%28v=exchg.80%29.aspx)の EWS のマネージ API のメソッドまたは[ExpandDL](http://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx)の EWS の操作を使用できます。</span><span class="sxs-lookup"><span data-stu-id="6d509-117">If the candidate is a distribution group, you can use the [ExpandGroup(ItemId)](http://msdn.microsoft.com/ja-jp/library/office/ee356407%28v=exchg.80%29.aspx) EWS Managed API method or the [ExpandDL](http://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx) EWS operation to get the list of members.</span></span> <span data-ttu-id="6d509-118">_ReturnContactDetails_パラメーターまたは EWS の**ReturnFullContactData**属性の true に設定、 **ResolveName**メソッドを使用して Active Directory エントリが返されるか、 **ResolveNames**操作には追加のプロパティは、連絡先を記述するとします。</span><span class="sxs-lookup"><span data-stu-id="6d509-118">If the  _returnContactDetails_ parameter or the **ReturnFullContactData** EWS attribute is set to true, Active Directory entries returned via a **ResolveName** method or **ResolveNames** operation will include additional properties that describe the contact.</span></span> <span data-ttu-id="6d509-119">_ReturnContactDetails_パラメーターまたは**ReturnFullContactData**属性は連絡先で返されるデータには影響されず、グループにお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="6d509-119">The  _returnContactDetails_ parameter or the **ReturnFullContactData** attribute does not affect the data that is returned for contacts and contact groups.</span></span> 
  
## <a name="resolve-ambiguous-names-by-using-ews-managed-api"></a><span data-ttu-id="6d509-120">EWS マネージ API を使用して、あいまいな名前を解決する</span><span class="sxs-lookup"><span data-stu-id="6d509-120">Resolve ambiguous names by using EWS Managed API</span></span>
<span data-ttu-id="6d509-121"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="6d509-121"></span></span>

<span data-ttu-id="6d509-122">[ResolveName](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx)メソッドを使用すると、渡されるあいまいな名前に一致する候補を検索します。</span><span class="sxs-lookup"><span data-stu-id="6d509-122">You can use the [ResolveName](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) method to find candidates that match the ambiguous name you pass.</span></span> <span data-ttu-id="6d509-123">**ResolveName**メソッドのオーバー ロードを使用すると、5 つの方法で候補を検索します。</span><span class="sxs-lookup"><span data-stu-id="6d509-123">You can use overloads of the **ResolveName** method to search for candidates in five different ways.</span></span> 
  
<span data-ttu-id="6d509-124">**表 1 です。ResolveName メソッドのオーバー ロードされました。**</span><span class="sxs-lookup"><span data-stu-id="6d509-124">**Table 1. Overloaded ResolveName methods**</span></span>

|<span data-ttu-id="6d509-125">**メソッド**</span><span class="sxs-lookup"><span data-stu-id="6d509-125">**Method**</span></span>|<span data-ttu-id="6d509-126">**しくみ**</span><span class="sxs-lookup"><span data-stu-id="6d509-126">**How it works**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d509-127">ResolveName(String)</span><span class="sxs-lookup"><span data-stu-id="6d509-127">ResolveName(String)</span></span>](http://msdn.microsoft.com/ja-jp/library/dd635548%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="6d509-p105">ユーザーの連絡先フォルダーにある連絡先、およびグローバル アドレス一覧 (GAL) にある連絡先を、この順番で検索します。その文字列変数は、解決しようとしているあいまいな名前です。</span><span class="sxs-lookup"><span data-stu-id="6d509-p105">Finds contacts in the user's Contacts folder and the Global Address List (GAL) — in that order. The string variable is the ambiguous name you are trying to resolve.</span></span>  <br/> |
|[<span data-ttu-id="6d509-130">ResolveName (文字列、ResolveNameSearchLocation、ブール値)</span><span class="sxs-lookup"><span data-stu-id="6d509-130">ResolveName(String, ResolveNameSearchLocation, Boolean)</span></span>](http://msdn.microsoft.com/ja-jp/library/dd634595%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="6d509-p106">既定の連絡先フォルダーにある連絡先と、グローバル アドレス一覧 (GAL) にある連絡先の一方または両方を検索します。文字列値はあいまいな名前で、検索場所は連絡先フォルダーとグローバル アドレス一覧の一方または両方を指定し、ブール値は連絡先の全情報を返すかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6d509-p106">Finds contacts in the default Contacts folder and/or the Global Address List (GAL). The string value is the ambiguous name, the search location specifies the Contacts folder and/or the GAL, and the Boolean value indicates whether to return the full contact information.</span></span>  <br/> |
|[<span data-ttu-id="6d509-133">ResolveName (文字列、ResolveNameSearchLocation、ブール値、プロパティ設定)</span><span class="sxs-lookup"><span data-stu-id="6d509-133">ResolveName(String, ResolveNameSearchLocation, Boolean, PropertySet)</span></span>](http://msdn.microsoft.com/ja-jp/library/hh532803%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="6d509-p107">既定の連絡先フォルダーにある連絡先と、グローバル アドレス一覧 (GAL) にある連絡先の一方または両方を検索します。このメソッドを使用すると、返されるプロパティを設定できます。</span><span class="sxs-lookup"><span data-stu-id="6d509-p107">Finds contacts in the default Contacts folder and/or Global Address List (GAL). This method enables you to set the properties that are returned.</span></span>  <br/> |
|[<span data-ttu-id="6d509-136">ResolveName (文字列、IEnumerable\<フォルダー Id\>、ResolveNameSearchLocation、ブール値)</span><span class="sxs-lookup"><span data-stu-id="6d509-136">ResolveName(String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean)</span></span>](http://msdn.microsoft.com/ja-jp/library/dd636014%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="6d509-p108">指定した連絡先フォルダーにある連絡先と、グローバル アドレス一覧 (GAL) にある連絡先の一方または両方を検索します。このメソッドを利用して、検索するフォルダーのコレクションを渡すことができます。これにより、既定の連絡先フォルダー以外の連絡先フォルダーを検索することができます。</span><span class="sxs-lookup"><span data-stu-id="6d509-p108">Finds contacts in specified contact folders and/or the Global Address List (GAL). You can use this method to pass a collection of folders to search. This enables you to look in contact folders other than the default Contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="6d509-140">ResolveName (文字列、IEnumerable\<フォルダー Id\>、ResolveNameSearchLocation、ブール値、プロパティ設定)</span><span class="sxs-lookup"><span data-stu-id="6d509-140">ResolveName(String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean, PropertySet)</span></span>](http://msdn.microsoft.com/ja-jp/library/hh532581%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="6d509-p109">グローバル アドレス一覧 (GAL) にある連絡先と、指定した連絡先フォルダーにある連絡先の一方または両方を検索します。このメソッドを使用すると、返されるプロパティを設定できます。</span><span class="sxs-lookup"><span data-stu-id="6d509-p109">Finds contacts in the Global Address List (GAL) and/or in specific contact folders. This method enables you to set the properties that are returned.</span></span>  <br/> |
   
<span data-ttu-id="6d509-143">簡単な例から始めましょう。</span><span class="sxs-lookup"><span data-stu-id="6d509-143">Let's start with a simple example.</span></span> <span data-ttu-id="6d509-144">次の例では、"dan という"テキスト文字列を解決するには、検出されたそれぞれの応募者の名前と電子メール アドレスを出力する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="6d509-144">The following example shows how to resolve the text string "dan" and output the name and email address of each candidate found.</span></span> <span data-ttu-id="6d509-145">この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="6d509-145">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

<span data-ttu-id="6d509-146">応答は、100 以上の候補があるかもしれませんが、100 の候補の最大を返します。</span><span class="sxs-lookup"><span data-stu-id="6d509-146">The response returns a maximum of 100 candidates, although there might be more than 100 potential candidates.</span></span> <span data-ttu-id="6d509-147">多くの候補者の最初の 100 個の候補のみが返されたかどうかを確認するのには、 [NameResolutionCollection](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx)オブジェクトの[IncludesAllResolutions](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx)の値を確認します。</span><span class="sxs-lookup"><span data-stu-id="6d509-147">To determine whether only the first 100 candidates of a larger number of candidates were returned, check the value of [IncludesAllResolutions](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx) in the [NameResolutionCollection](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) object.</span></span> <span data-ttu-id="6d509-148">値が true の場合はこれ以上の候補です。値が false の場合は、メソッドより多くの潜在的な候補者の最初の 100 人だけ返されます。</span><span class="sxs-lookup"><span data-stu-id="6d509-148">If the value is true, there are no more possible candidates; if the value is false, the method only returned the first 100 of a larger number of potential candidates.</span></span> 
  
<span data-ttu-id="6d509-149">大規模な組織で作業している場合に、"dan"などの名前が 100 の候補の最大数を返すことが可能性があります。</span><span class="sxs-lookup"><span data-stu-id="6d509-149">If you work in a large organization, it's likely that a name like "dan" will return the maximum number of 100 candidates.</span></span> <span data-ttu-id="6d509-150">返される候補の数を減らすためには、検索する場所を制限します。</span><span class="sxs-lookup"><span data-stu-id="6d509-150">To reduce the number of candidates returned, limit where you search.</span></span> <span data-ttu-id="6d509-151">次の例では、あいまいな名前を解決するのには検索するのに場所を指定するのに[ResolveNameSearchLocation](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx)列挙体を使用します。</span><span class="sxs-lookup"><span data-stu-id="6d509-151">The next example uses the [ResolveNameSearchLocation](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx) enumeration to specify where to search to resolve the ambiguous name.</span></span> 
  
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

<span data-ttu-id="6d509-152">既知の連絡先フォルダー以外のフォルダーに連絡先を格納する場合は、候補を検索する場所を指定するオーバー ロードされたメソッドのいずれかを使用します。</span><span class="sxs-lookup"><span data-stu-id="6d509-152">If you store your contacts in a folder other than the well-known Contacts folder, use one of the overloaded methods to specify where to look for candidates.</span></span> <span data-ttu-id="6d509-153">**ResolveName**メソッドがフォルダーの ID を基にフォルダー一覧を作成する例を次</span><span class="sxs-lookup"><span data-stu-id="6d509-153">The following example creates a folder list for the **ResolveName** method based on the folder ID.</span></span> <span data-ttu-id="6d509-154">**フォルダー Id**が小さすぎると読みやすくするためです。</span><span class="sxs-lookup"><span data-stu-id="6d509-154">The **FolderId** has been shortened for readability.</span></span> 
  
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

<span data-ttu-id="6d509-155">フィルターを適用すると、候補が返されない、 [NameResolutionCollection](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx)には 0 個のエントリが含まれます。</span><span class="sxs-lookup"><span data-stu-id="6d509-155">If you apply filters and no candidates are returned, the [NameResolutionCollection](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) will contain zero entries.</span></span> <span data-ttu-id="6d509-156">コレクションの[Count](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx)プロパティを参照して、これを確認することができます。</span><span class="sxs-lookup"><span data-stu-id="6d509-156">You can verify this by looking at the [Count](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx) property of the collection.</span></span> 
  
## <a name="resolve-ambiguous-names-by-using-ews"></a><span data-ttu-id="6d509-157">EWS を使用して、あいまいな名前を解決します</span><span class="sxs-lookup"><span data-stu-id="6d509-157">Resolve ambiguous names by using EWS</span></span>
<span data-ttu-id="6d509-158"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="6d509-158"></span></span>

<span data-ttu-id="6d509-159">[ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS の操作を使用するにはあいまいな名前の候補を識別します。</span><span class="sxs-lookup"><span data-stu-id="6d509-159">You can use the [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS operation to identify possible candidates for an ambiguous name.</span></span> <span data-ttu-id="6d509-160">[UnresolvedEntry](http://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx)要素には、解決する場合、あいまいな名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6d509-160">The [UnresolvedEntry](http://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx) element contains the ambiguous name you want to resolve.</span></span> <span data-ttu-id="6d509-161">Sadie の名前を解決するのには次の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6d509-161">The following example shows how to resolve the name Sadie.</span></span> <span data-ttu-id="6d509-162">[ResolveName メソッドを使用して](#bk_EWSMA)、it 部門以外は、有効な出力の例については別の名前を使用する場合、EWS のマネージ API を使用している XML の要求にもです。</span><span class="sxs-lookup"><span data-stu-id="6d509-162">This is also the XML request that the EWS Managed API uses when you [use the ResolveName method](#bk_EWSMA), except that it uses a different name for valid output examples.</span></span>
  
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

<span data-ttu-id="6d509-163">応答より多くの候補者の最初の 100 個の候補のみが返されたかどうかを決定する、 [IncludesLastItemInRange](http://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx)の値を確認する 100 以上の候補があるかもしれませんが、100 の候補の最大を返します[ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx)要素の属性です。</span><span class="sxs-lookup"><span data-stu-id="6d509-163">The response returns a maximum of 100 candidates, although there might be more than 100 potential candidates To determine whether only the first 100 candidates of a larger number of candidates were returned, check the value of the [IncludesLastItemInRange](http://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx) attribute of the [ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="6d509-164">値が true の場合はこれ以上の候補です。値が false の場合は、操作より多くの潜在的な候補者の最初の 100 人だけ返されます。</span><span class="sxs-lookup"><span data-stu-id="6d509-164">If the value is true, there are no more possible candidates; if the value is false, the operation only returned the first 100 of a larger number of potential candidates.</span></span> 
  
<span data-ttu-id="6d509-165">次の例は、1 つの候補が見つかった場合、XML 応答を示します。</span><span class="sxs-lookup"><span data-stu-id="6d509-165">The following example shows the XML response when one candidate is found.</span></span> <span data-ttu-id="6d509-166">ただし、 [ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx)は、[解像度](http://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx)の要素とその子要素を表す、最大 100 個の候補者を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="6d509-166">Remember, the [ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) can contain up to 100 candidates, each one represented by the [Resolution](http://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx) element and its child elements.</span></span> 
  
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

<span data-ttu-id="6d509-p118">あいまいな名前の候補がいつも検索できるとは限りません。次の例では、候補が見つからなかった場合に、エラーとして返される XML 応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="6d509-p118">You're not always going to come up with candidates for your ambiguous name. The following example shows the XML response, as an error, when no candidates are found.</span></span>
  
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

## <a name="see-also"></a><span data-ttu-id="6d509-169">関連項目</span><span class="sxs-lookup"><span data-stu-id="6d509-169">See also</span></span>


- [<span data-ttu-id="6d509-170">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="6d509-170">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)
    
- [<span data-ttu-id="6d509-171">Exchange 2013 の EWS を使用して配布グループを展開します。</span><span class="sxs-lookup"><span data-stu-id="6d509-171">Expand distribution groups by using EWS in Exchange 2013</span></span>](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

