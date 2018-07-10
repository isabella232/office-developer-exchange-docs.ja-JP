---
title: 追加し、Exchange の EWS を使用して、デリゲートを削除します。
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: cc7760bf-633b-483a-84ae-b52f437af2d3
description: Exchange の EWS マネージ API または EWS を使用してユーザーのメールボックスに対して代理人を追加または削除する方法について説明します。
ms.openlocfilehash: d55ef6c5c4e434603d293dbe30c6147ceb73b08b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758912"
---
# <a name="add-and-remove-delegates-by-using-ews-in-exchange"></a><span data-ttu-id="111c2-103">追加し、Exchange の EWS を使用して、デリゲートを削除します。</span><span class="sxs-lookup"><span data-stu-id="111c2-103">Add and remove delegates by using EWS in Exchange</span></span>

<span data-ttu-id="111c2-104">Exchange の EWS マネージ API または EWS を使用してユーザーのメールボックスに対して代理人を追加または削除する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="111c2-104">Learn how to add delegates to or remove delegates from users' mailboxes by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="111c2-105">メールボックス所有者の代理として機能またはメールボックスへの代理人のアクセスを削除するのにデリゲートを有効にするのには、EWS のマネージ API または EWS を使用できます。</span><span class="sxs-lookup"><span data-stu-id="111c2-105">You can use the EWS Managed API or EWS to enable delegates to act on behalf of a mailbox owner or remove a delegate's access to a mailbox.</span></span> <span data-ttu-id="111c2-106">代理人として追加し、アクセス許可が与えられますユーザーは、メールボックス所有者の代理としてのタスクを実行できます。</span><span class="sxs-lookup"><span data-stu-id="111c2-106">Users who are added as a delegate, and are given permissions, can perform tasks on behalf of the mailbox owner.</span></span> <span data-ttu-id="111c2-107">など、作成し会議出席依頼を送信、電子メールを送信できに会議出席依頼をメールボックスの所有者の代わりに応答できます。</span><span class="sxs-lookup"><span data-stu-id="111c2-107">For example, they can create and send meeting invitations, send emails, and respond to meeting requests on the mailbox owner's behalf.</span></span> 
  
<span data-ttu-id="111c2-108">**表 1 です。EWS のマネージ API のメソッドおよび EWS の操作を追加すると、デリゲートを削除します。**</span><span class="sxs-lookup"><span data-stu-id="111c2-108">**Table 1. EWS Managed API methods and EWS operations for adding and removing delegates**</span></span>

|<span data-ttu-id="111c2-109">**タスク**</span><span class="sxs-lookup"><span data-stu-id="111c2-109">**Task**</span></span>|<span data-ttu-id="111c2-110">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="111c2-110">**EWS Managed API method**</span></span>|<span data-ttu-id="111c2-111">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="111c2-111">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="111c2-112">代理人を追加する</span><span class="sxs-lookup"><span data-stu-id="111c2-112">Add delegates</span></span>  <br/> |[<span data-ttu-id="111c2-113">ExchangeService.AddDelegates</span><span class="sxs-lookup"><span data-stu-id="111c2-113">ExchangeService.AddDelegates</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="111c2-114">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="111c2-114">AddDelegate</span></span>](http://msdn.microsoft.com/library/646fb994-229e-4d90-8b95-6541191cb3ae%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="111c2-115">代理人を削除する</span><span class="sxs-lookup"><span data-stu-id="111c2-115">Remove delegates</span></span>  <br/> |[<span data-ttu-id="111c2-116">ExchangeService.RemoveDelegates</span><span class="sxs-lookup"><span data-stu-id="111c2-116">ExchangeService.RemoveDelegates</span></span>](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="111c2-117">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="111c2-117">RemoveDelegate</span></span>](http://msdn.microsoft.com/library/f21c5171-62e7-47c8-99b1-22e1ff5883bb%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="111c2-118">デリゲートがフォルダーへのアクセス許可を与えられて後、は、それらの[アクセス許可を委任](delegate-access-and-ews-in-exchange.md#bk_delegateperms)することによってフォルダーとすべてのサブフォルダー内のアイテムで動作できます。</span><span class="sxs-lookup"><span data-stu-id="111c2-118">After a delegate is granted permissions to a folder, they can act on items in the folder and any subfolders, according to their [delegate permissions](delegate-access-and-ews-in-exchange.md#bk_delegateperms).</span></span> <span data-ttu-id="111c2-119">デリゲートのアクセス許可は、代理アクセス権が付与された後に作成されるサブフォルダーにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="111c2-119">Permissions for delegates only apply to subfolders that are created after the delegate access was granted.</span></span> <span data-ttu-id="111c2-120">既存のフォルダー、またはその他のフォルダーのフォルダーのアクセス許可を更新するには、 [Exchange EWS を使用して別のユーザーのフォルダーのアクセス許可の設定](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="111c2-120">To update folder permissions for pre-existing folders, or other folders, see [Set folder permissions for another user by using EWS in Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="111c2-p103">メールが有効なセキュリティ グループなど、メールボックスが有効なアカウントにのみ代理人を追加できます。既定では、1 つの EWS 代理人アクセス権限呼び出しで、最大 255 の異なるメールボックスにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="111c2-p103">Note that delegates can only be added to mailbox-enabled accounts, including mail-enabled security groups. By default, a single EWS delegate access call can access a maximum of 255 different mailboxes.</span></span>

<span data-ttu-id="111c2-123"><a name="bk_adddelegateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="111c2-123"></span></span>

## <a name="add-delegates-by-using-the-ews-managed-api"></a><span data-ttu-id="111c2-124">EWS マネージ API を使用して代理人を追加する</span><span class="sxs-lookup"><span data-stu-id="111c2-124">Add delegates by using the EWS Managed API</span></span>

<span data-ttu-id="111c2-125">[AddDelegates](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) EWS 管理 API メソッドを使用してメールボックスに代理人を追加できます。</span><span class="sxs-lookup"><span data-stu-id="111c2-125">You can add delegates to a mailbox by using the [AddDelegates](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) EWS Managed API method.</span></span> <span data-ttu-id="111c2-126">次の使用例、新しい予定表、連絡先、および電子メール[DelegateUser](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.delegateuser%28v=exchg.80%29.aspx)のオブジェクトが作成され、それぞれの代理人にはそれぞれのフォルダーの[エディターのアクセス許可](delegate-access-and-ews-in-exchange.md#bk_delegateperms)が与えられます。</span><span class="sxs-lookup"><span data-stu-id="111c2-126">In this example, a new calendar, contact, and email [DelegateUser](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.delegateuser%28v=exchg.80%29.aspx) object is created, and each delegate is given [Editor permissions](delegate-access-and-ews-in-exchange.md#bk_delegateperms) for their respective folder.</span></span> <span data-ttu-id="111c2-127">[DelegatePermissions プロパティ](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.delegatepermissions_properties%28v=exchg.80%29.aspx)によって指定されたフォルダーのいずれかにデリゲートを追加する例を変更することができ、アクセス許可を設定するには、 [DelegateFolderPermissionLevel](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.delegatefolderpermissionlevel%28v=exchg.80%29.aspx)列挙体で指定された値のいずれかにします。</span><span class="sxs-lookup"><span data-stu-id="111c2-127">You can modify the example to add a delegate to any of the folders specified by the [DelegatePermissions properties](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.delegatepermissions_properties%28v=exchg.80%29.aspx), and you can set the permissions to any of the values specified by the [DelegateFolderPermissionLevel](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.delegatefolderpermissionlevel%28v=exchg.80%29.aspx) enumeration.</span></span> 
  
<span data-ttu-id="111c2-128">この例でその**サービス**は、メールボックスの所有者の有効な[ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトは、ユーザーが Exchange サーバーに認証されているとします。</span><span class="sxs-lookup"><span data-stu-id="111c2-128">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner, and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static Collection<DelegateUserResponse> AddDelegates(ExchangeService service)
{
    // Create a list to hold the new delegates to add.
    List<DelegateUser> newDelegates = new System.Collections.Generic.List<DelegateUser>();
    // Create a new delegate that has editor access to the mailbox owner's Calendar folder.
    DelegateUser calendarDelegate = new DelegateUser("calendardelegate@contoso.com");
    calendarDelegate.Permissions.CalendarFolderPermissionLevel = DelegateFolderPermissionLevel.Editor;
    // Add the delegate to the list of new delegates.
    newDelegates.Add(calendarDelegate);
    // Create a new delegate that has editor access to the mailbox owner's Contacts folder.
    DelegateUser contactDelegate = new DelegateUser("contactdelegate@contoso.com");
    contactDelegate.Permissions.ContactsFolderPermissionLevel = DelegateFolderPermissionLevel.Editor;
    // Add the delegate to the list of new delegates.
    newDelegates.Add(contactDelegate);
            
    // Create a new delegate that has editor access to the mailbox owner's Inbox folder.
    DelegateUser emailDelegate = new DelegateUser("emaildelegate@contoso.com");
    emailDelegate.Permissions.InboxFolderPermissionLevel = DelegateFolderPermissionLevel.Editor;
    // Add the delegate to the list of new delegates.
    newDelegates.Add(emailDelegate);
    // Create a mailbox object that represents the mailbox owner.
    Mailbox mailbox = new Mailbox("primary@contoso.com");
    // Call the AddDelegates method to add the delegates to the target mailbox.
    Collection<DelegateUserResponse> response = service.AddDelegates(mailbox, MeetingRequestsDeliveryScope.DelegatesAndSendInformationToMe, newDelegates);
            
    foreach (DelegateUserResponse resp in response)
    {
        // Print out the result and the last eight characters of the item ID.
        Console.WriteLine("For delegate " + resp.DelegateUser.UserId.PrimarySmtpAddress.ToString());
        Console.WriteLine("Result: {0}", resp.Result);
        Console.WriteLine("Error Code: {0}", resp.ErrorCode);
        Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
        Console.WriteLine("\r\n");
    }
    return response;
}
```

<span data-ttu-id="111c2-129"><a name="bk_adddelegateews"> </a></span><span class="sxs-lookup"><span data-stu-id="111c2-129"></span></span>

## <a name="add-delegates-by-using-ews"></a><span data-ttu-id="111c2-130">EWS を使用して代理人を追加する</span><span class="sxs-lookup"><span data-stu-id="111c2-130">Add delegates by using EWS</span></span>

<span data-ttu-id="111c2-131">[AddDelegate](http://msdn.microsoft.com/library/012d8cc5-648c-4ba0-a155-15c422b1e994%28Office.15%29.aspx) EWS 操作を使用して別の予定表、連絡先、および電子メールの代理人を追加するのには次のコード例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="111c2-131">The following code example shows how to add separate calendar, contact, and email delegates by using the [AddDelegate](http://msdn.microsoft.com/library/012d8cc5-648c-4ba0-a155-15c422b1e994%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="111c2-132">メールボックスを変更するのには、要素によって指定された、[メールボックス](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx)、および[DelegateUser](http://msdn.microsoft.com/library/aac4e74e-f69b-4c41-a0c9-489610330fbf%28Office.15%29.aspx)要素で各デリゲートの[アクセス許可](delegate-access-and-ews-in-exchange.md#bk_delegateperms)の設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="111c2-132">The mailbox to modify is specified by the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element, and the [permission](delegate-access-and-ews-in-exchange.md#bk_delegateperms) settings for each delegate are contained in the [DelegateUser](http://msdn.microsoft.com/library/aac4e74e-f69b-4c41-a0c9-489610330fbf%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="111c2-133">代理人のそれぞれは、編集者アクセス権の対象となるフォルダーを与えられています。</span><span class="sxs-lookup"><span data-stu-id="111c2-133">Each of the delegates has been granted Editor permissions to their target folder.</span></span> 
  
<span data-ttu-id="111c2-134">EWS のマネージ API が[代理人を追加](#bk_adddelegateewsma)するのには**AddDelegates**メソッドを使用するときに送信する XML 要求にもです。</span><span class="sxs-lookup"><span data-stu-id="111c2-134">This is also the XML request that the EWS Managed API sends when you use the **AddDelegates** method to [add delegates](#bk_adddelegateewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:AddDelegate>
      <m:Mailbox>
        <t:EmailAddress>primary@contoso.com</t:EmailAddress>
      </m:Mailbox>
      <m:DelegateUsers>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>calendardelegate@contoso.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:CalendarFolderPermissionLevel>Editor</t:CalendarFolderPermissionLevel>
            <t:TasksFolderPermissionLevel>None</t:TasksFolderPermissionLevel>
            <t:InboxFolderPermissionLevel>None</t:InboxFolderPermissionLevel>
            <t:ContactsFolderPermissionLevel>None</t:ContactsFolderPermissionLevel>
            <t:NotesFolderPermissionLevel>None</t:NotesFolderPermissionLevel>
            <t:JournalFolderPermissionLevel>None</t:JournalFolderPermissionLevel>
          </t:DelegatePermissions>
          <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
          <t:ViewPrivateItems>false</t:ViewPrivateItems>
        </t:DelegateUser>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>contactdelegate@contoso.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:CalendarFolderPermissionLevel>None</t:CalendarFolderPermissionLevel>
            <t:TasksFolderPermissionLevel>None</t:TasksFolderPermissionLevel>
            <t:InboxFolderPermissionLevel>None</t:InboxFolderPermissionLevel>
            <t:ContactsFolderPermissionLevel>Editor</t:ContactsFolderPermissionLevel>
            <t:NotesFolderPermissionLevel>None</t:NotesFolderPermissionLevel>
            <t:JournalFolderPermissionLevel>None</t:JournalFolderPermissionLevel>
          </t:DelegatePermissions>
          <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
          <t:ViewPrivateItems>false</t:ViewPrivateItems>
        </t:DelegateUser>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>emaildelegate@contoso.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:CalendarFolderPermissionLevel>None</t:CalendarFolderPermissionLevel>
            <t:TasksFolderPermissionLevel>None</t:TasksFolderPermissionLevel>
            <t:InboxFolderPermissionLevel>Editor</t:InboxFolderPermissionLevel>
            <t:ContactsFolderPermissionLevel>None</t:ContactsFolderPermissionLevel>
            <t:NotesFolderPermissionLevel>None</t:NotesFolderPermissionLevel>
            <t:JournalFolderPermissionLevel>None</t:JournalFolderPermissionLevel>
          </t:DelegatePermissions>
          <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
          <t:ViewPrivateItems>false</t:ViewPrivateItems>
        </t:DelegateUser>
      </m:DelegateUsers>
      <m:DeliverMeetingRequests>DelegatesAndSendInformationToMe</m:DeliverMeetingRequests>
    </m:AddDelegate>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="111c2-135">サーバーは、 **NoError**を代理人が正常に作成されたことを示すは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素の値が含まれています[AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx)メッセージから**AddDelegate**要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="111c2-135">The server responds to the **AddDelegate** request with an [AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the delegates were successfully created.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="888"
                         MinorBuildNumber="9"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:AddDelegateResponse ResponseClass="Success"
                           xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
            <t:UserId>
              <t:SID>S-1-5-21-1337771579-694202782-848329751-1535221</t:SID>
              <t:PrimarySmtpAddress>calendardelegate@contoso.com</t:PrimarySmtpAddress>
              <t:DisplayName>calendardelegate</t:DisplayName>
            </t:UserId>
            <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
          </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
            <t:UserId>
              <t:SID>S-1-5-21-1337771579-694202782-848329751-1535264</t:SID>
              <t:PrimarySmtpAddress>contactdelegate@contoso.com</t:PrimarySmtpAddress>
              <t:DisplayName>contactdelegate</t:DisplayName>
            </t:UserId>
            <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
          </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
            <t:UserId>
              <t:SID>S-1-5-21-1337771579-694202782-848329751-1535223</t:SID>
              <t:PrimarySmtpAddress>emaildelegate@contoso.com</t:PrimarySmtpAddress>
              <t:DisplayName>emaildelegate</t:DisplayName>
            </t:UserId>
            <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
          </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
    </m:AddDelegateResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="111c2-136"><a name="bk_removedelegateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="111c2-136"></span></span>

## <a name="remove-delegates-by-using-the-ews-managed-api"></a><span data-ttu-id="111c2-137">EWS マネージ API を使用して代理人を削除する</span><span class="sxs-lookup"><span data-stu-id="111c2-137">Remove delegates by using the EWS Managed API</span></span>

<span data-ttu-id="111c2-138">[ExchangeService.RemoveDelegates](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) EWS 管理 API メソッドを使用して、移動先のメールボックスからデリゲートを削除できます。</span><span class="sxs-lookup"><span data-stu-id="111c2-138">You can remove delegates from a target mailbox by using the [ExchangeService.RemoveDelegates](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) EWS Managed API method.</span></span> <span data-ttu-id="111c2-139">この例では、[デリゲートの使用例を追加](#bk_adddelegateewsma)する代理人アクセス権セットが削除されます。</span><span class="sxs-lookup"><span data-stu-id="111c2-139">In this example, the delegate permissions set in the [add a delegate example](#bk_adddelegateewsma) are removed.</span></span> 
  
<span data-ttu-id="111c2-140">この例でその**サービス**は、メールボックスの所有者の有効な[ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトは、ユーザーが Exchange サーバーに認証されているとします。</span><span class="sxs-lookup"><span data-stu-id="111c2-140">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner, and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static Collection<DelegateUserResponse> RemoveDelegates(ExchangeService service)
{
    // Create a list to hold the delegates to delete.
    List<UserId> deletedDelegates = new System.Collections.Generic.List<UserId>();
    // Add the delegate to the list of new delegates.
    deletedDelegates.Add("calendardelegate@contoso.com");
    // Add the delegate to the list of new delegates.
    deletedDelegates.Add("contactdelegate@contoso.com");
    // Add the delegate to the list of new delegates.
    deletedDelegates.Add("emaildelegate@contoso.com");
    // Create a mailbox object that represents the mailbox owner.
    Mailbox mailbox = new Mailbox("primary@contoso.com");
    // Call the AddDelegates method to add the delegates to the target mailbox.
    Collection<DelegateUserResponse> response = service.RemoveDelegates(mailbox, deletedDelegates);
    foreach (DelegateUserResponse resp in response)
    {
        // Print out the result and the last eight characters of the item ID.
        Console.WriteLine("Result: {0}", resp.Result);
        Console.WriteLine("Error Code: {0}", resp.ErrorCode);
        Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
    }
    return response;
}
```

<span data-ttu-id="111c2-141"><a name="bk_removedelegateews"> </a></span><span class="sxs-lookup"><span data-stu-id="111c2-141"></span></span>

## <a name="remove-delegates-by-using-ews"></a><span data-ttu-id="111c2-142">EWS を使用して代理人を削除する</span><span class="sxs-lookup"><span data-stu-id="111c2-142">Remove delegates by using EWS</span></span>

<span data-ttu-id="111c2-143">[RemoveDelegate](http://msdn.microsoft.com/library/1d42d5ff-8fde-4f8a-b18d-57b1ef7a946a%28Office.15%29.aspx) EWS 操作を使用して、メールボックスからデリゲートを削除できます。</span><span class="sxs-lookup"><span data-stu-id="111c2-143">You can remove delegates from a mailbox by using the [RemoveDelegate](http://msdn.microsoft.com/library/1d42d5ff-8fde-4f8a-b18d-57b1ef7a946a%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="111c2-144">この例では、[デリゲートの使用例を追加](#bk_adddelegateews)する代理人アクセス権セットが削除されます。</span><span class="sxs-lookup"><span data-stu-id="111c2-144">In this example, the delegate permissions set in the [add a delegate example](#bk_adddelegateews) are removed.</span></span> 
  
<span data-ttu-id="111c2-145">EWS のマネージ API が[デリゲートを削除](#bk_removedelegateewsma)するのには**RemoveDelegates**メソッドを使用するときに送信する XML 要求にもです。</span><span class="sxs-lookup"><span data-stu-id="111c2-145">This is also the XML request that the EWS Managed API sends when you use the **RemoveDelegates** method to [remove delegates](#bk_removedelegateewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:RemoveDelegate>
      <m:Mailbox>
        <t:EmailAddress>primary@contoso.com</t:EmailAddress>
      </m:Mailbox>
      <m:UserIds>
        <t:UserId>
          <t:PrimarySmtpAddress>calendardelegate@contoso.com</t:PrimarySmtpAddress>
        </t:UserId>
        <t:UserId>
          <t:PrimarySmtpAddress>contactdelegate@contoso.com</t:PrimarySmtpAddress>
        </t:UserId>
        <t:UserId>
          <t:PrimarySmtpAddress>emaildelegate@contoso.com</t:PrimarySmtpAddress>
        </t:UserId>
      </m:UserIds>
    </m:RemoveDelegate>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="111c2-146">サーバーは、 **NoError**を代理人が正常に削除されたことを示すは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素の値を含む[AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx)メッセージの**RemoveDelegate**の要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="111c2-146">The server responds to the **RemoveDelegate** request with a [AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the delegates were successfully removed.</span></span>

<span data-ttu-id="111c2-147"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="111c2-147"></span></span>

## <a name="next-steps"></a><span data-ttu-id="111c2-148">次の手順</span><span class="sxs-lookup"><span data-stu-id="111c2-148">Next steps</span></span>

<span data-ttu-id="111c2-p108">予定表、メール、およびタスクのフォルダーに代理人を追加すると、代理人はフォルダー内のアイテムにアクセスできるようになります。詳細については、次の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="111c2-p108">After you add delegates to calendar, email, and task folders, the delegate can access the items in the folders. To learn more, see the following articles:</span></span>
  
- [<span data-ttu-id="111c2-151">EWS を使用して Exchange 内で代理人として電子メールにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="111c2-151">Access email as a delegate by using EWS in Exchange</span></span>](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="111c2-152">EWS を使用して Exchange 内で代理人に予定表にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="111c2-152">Access a calendar as a delegate by using EWS in Exchange</span></span>](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="111c2-153">Exchange EWS を使用して代理人としてアクセス連絡先</span><span class="sxs-lookup"><span data-stu-id="111c2-153">Access contacts as a delegate by using EWS in Exchange</span></span>](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
<span data-ttu-id="111c2-154">代理人を追加したフォルダーには、代理アクセス権を付与する前に作成された子フォルダーが含まれている場合、代理人を追加の権限がない場合、それらのフォルダーにアクセスすることはできません。</span><span class="sxs-lookup"><span data-stu-id="111c2-154">If the folders for which you added delegates include child folders that were created before you granted the delegate access, the delegate will not be able to access those folders without additional permissions.</span></span> <span data-ttu-id="111c2-155">これらのアクセス許可を追加または他のフォルダーのアクセス許可を変更する、 [Exchange で EWS を使用して別のユーザーのフォルダーのアクセス許可の設定](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="111c2-155">To add these permissions, or modify permissions for any other folders, see [Set folder permissions for another user by using EWS in Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="111c2-156">関連項目</span><span class="sxs-lookup"><span data-stu-id="111c2-156">See also</span></span>

- [<span data-ttu-id="111c2-157">Exchange での代理人アクセスと EWS</span><span class="sxs-lookup"><span data-stu-id="111c2-157">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)
- [<span data-ttu-id="111c2-158">追加の Exchange 2013: プログラムを使用してユーザーが電子メール アカウントを委任します。</span><span class="sxs-lookup"><span data-stu-id="111c2-158">Exchange 2013: Add delegate users to an email account programmatically</span></span>](http://code.msdn.microsoft.com/exchange/Exchange-2013-Adding-1024511f)   
- [<span data-ttu-id="111c2-159">Exchange 2013: プログラムでの電子メール アカウントに関連付けられているデリゲートを更新します。</span><span class="sxs-lookup"><span data-stu-id="111c2-159">Exchange 2013: Update delegates associated with email accounts programmatically</span></span>](http://code.msdn.microsoft.com/exchange/Exchange-2013-Update-b40d3bac)   
- [<span data-ttu-id="111c2-160">Exchange 2013: プログラムでの電子メール アカウントに関連付けられているデリゲートを削除します。</span><span class="sxs-lookup"><span data-stu-id="111c2-160">Exchange 2013: Remove delegates associated with email accounts programmatically</span></span>](http://code.msdn.microsoft.com/exchange/Exchange-2013-Remove-686f7714)
    

