---
title: Exchange EWS を使用して連絡先グループを作成します。
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: acec6e73-c016-419d-be1a-8ec5d993addb
description: Exchange で EWS マネージ API または EWS を使用して、連絡先グループを作成する方法について説明します。
ms.openlocfilehash: b3357f24e07a9c1b3b37ccb63b0f4f0d0a1d6fcf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758934"
---
# <a name="create-contact-groups-by-using-ews-in-exchange"></a><span data-ttu-id="1ca2a-103">Exchange EWS を使用して連絡先グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="1ca2a-103">Create contact groups by using EWS in Exchange</span></span>

<span data-ttu-id="1ca2a-104">Exchange で EWS マネージ API または EWS を使用して、連絡先グループを作成する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="1ca2a-104">Learn how to create a contact group by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="1ca2a-105">EWS のマネージ API または EWS を使用してプライベート[配布グループ](distribution-groups-and-ews-in-exchange.md)は、連絡先グループを作成できます。</span><span class="sxs-lookup"><span data-stu-id="1ca2a-105">You can create a contact group, which is a private [distribution group](distribution-groups-and-ews-in-exchange.md), by using the EWS Managed API or EWS.</span></span> <span data-ttu-id="1ca2a-106">連絡先グループを作成するに[ContactGroup](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx)の EWS のマネージ API のクラスのメソッドを使用または[CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS の操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="1ca2a-106">To create contact groups, use the methods in the [ContactGroup](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) EWS Managed API class, or use the [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation.</span></span> 
  
<span data-ttu-id="1ca2a-107">ユニバーサル配布グループまたはセキュリティ グループを作成するのには、EWS のマネージ API または EWS を使用できません注意してください。</span><span class="sxs-lookup"><span data-stu-id="1ca2a-107">Note that you can't use the EWS Managed API or EWS to create a universal distribution group or security group.</span></span> <span data-ttu-id="1ca2a-108">ユニバーサル配布グループまたはセキュリティ グループを作成するには、[新規 DistributionGroup](http://technet.microsoft.com/ja-jp/library/aa998856%28v=exchg.150%29.aspx)[Exchange 管理シェル コマンドレット](http://msdn.microsoft.com/ja-jp/library/ff326159%28v=exchg.140%29.aspx)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="1ca2a-108">To create a universal distribution group or security group, you can use the [New-DistributionGroup](http://technet.microsoft.com/ja-jp/library/aa998856%28v=exchg.150%29.aspx)[Exchange Management Shell cmdlet](http://msdn.microsoft.com/ja-jp/library/ff326159%28v=exchg.140%29.aspx).</span></span> 
  
## <a name="create-a-contact-group-by-using-the-ews-managed-api"></a><span data-ttu-id="1ca2a-109">EWS マネージ API を使用して連絡先グループを作成する</span><span class="sxs-lookup"><span data-stu-id="1ca2a-109">Create a contact group by using the EWS Managed API</span></span>
<span data-ttu-id="1ca2a-110"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="1ca2a-110"></span></span>

<span data-ttu-id="1ca2a-p103">連絡先グループを作成するために必要となるのは、2 つの情報、つまりグループの名前とグループに追加するメンバーだけです。次の例は、2 人のグループ メンバーが含まれる簡単な連絡先グループを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="1ca2a-p103">To create a contact group, you just need a couple pieces of information: a name for the group, and the members to add to the group. The following example shows how to create a simple contact group that contains a couple of group members.</span></span>
  
```cs
// Create a new contact group object.
ContactGroup myContactGroup = new ContactGroup(service);
// Give the group a name.
myContactGroup.DisplayName = "My Contact Group";
// Add some members to the group.
myContactGroup.Members.Add(new GroupMember("sadie@contoso.com"));
myContactGroup.Members.Add(new GroupMember("alfred@contoso.com"));
// Save the group.
myContactGroup.Save();

```

## <a name="create-a-contact-group-by-using-ews"></a><span data-ttu-id="1ca2a-113">EWS を使用して連絡先グループを作成する</span><span class="sxs-lookup"><span data-stu-id="1ca2a-113">Create a contact group by using EWS</span></span>
<span data-ttu-id="1ca2a-114"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="1ca2a-114"></span></span>

<span data-ttu-id="1ca2a-115">数行のコードがかかる場合がありますが、 [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS の操作を使用して連絡先グループを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="1ca2a-115">It might take a few more lines of code, but you can create a contact group by using the [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="1ca2a-116">次の XML 要求の例は、連絡先グループを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="1ca2a-116">The following XML request example shows how you can create a contact group.</span></span> <span data-ttu-id="1ca2a-117">これは XML 要求を送信する場合でも[連絡先グループを作成するのには EWS のマネージ API を使用](#bk_EWSMA)します。</span><span class="sxs-lookup"><span data-stu-id="1ca2a-117">This is also the XML request that is sent when you [use the EWS Managed API to create a contact group](#bk_EWSMA).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
   <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
MessageDisposition="SaveOnly">
      <Items xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
         <DistributionList xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
            <DisplayName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               My Contact Group
            </DisplayName>
            <Members xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <Member xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                  <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                     <EmailAddress xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                        sadie@contoso.com
                     </EmailAddress>
                  </Mailbox>
               </Member>
               <Member xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                  <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                     <EmailAddress xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                        alfred@contoso.com
                     </EmailAddress>
                  </Mailbox>
               </Member>
            </Members>
         </DistributionList>
      </Items>
   </CreateItem>
```

<span data-ttu-id="1ca2a-p105">要求に対して成功した XML 応答の例を次に示します。返される値に、新しい連絡先グループのアイテム ID、および連絡先グループを変更したり、グループを展開してメンバーを表示したりするために他のコードで使用できる変更キーが含まれている点に注目してください。アイテム ID は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="1ca2a-p105">The following is an example of a successful XML response to the request. Notice that the values returned include an item ID for the new contact group and a change key that you can use in other code to modify the contact group or expand the group to see the members. The item ID is shortened for readability.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
   <CreateItemResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <CreateItemResponseMessage ResponseClass="Success" 
             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
            <ResponseCode xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
               NoError
            </ResponseCode>
            <Items xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
               <DistributionList xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                  <ItemId xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                          Id="AAMkADBlY…" 
                          ChangeKey="EgAAABYAAAAD7hO1SJPWTbICFWZ4U3NMAABXzQiK" />
               </DistributionList>
            </Items>
         </CreateItemResponseMessage>
      </ResponseMessages>
   </CreateItemResponse>
```

## <a name="see-also"></a><span data-ttu-id="1ca2a-121">関連項目</span><span class="sxs-lookup"><span data-stu-id="1ca2a-121">See also</span></span>


- [<span data-ttu-id="1ca2a-122">Exchange の配布グループと EWS</span><span class="sxs-lookup"><span data-stu-id="1ca2a-122">Distribution groups and EWS in Exchange</span></span>](distribution-groups-and-ews-in-exchange.md)
    
- [<span data-ttu-id="1ca2a-123">Exchange 2013 の EWS を使用して配布グループを展開します。</span><span class="sxs-lookup"><span data-stu-id="1ca2a-123">Expand distribution groups by using EWS in Exchange 2013</span></span>](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

