---
title: Exchange で EWS を使用して連絡先グループを作成する
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: acec6e73-c016-419d-be1a-8ec5d993addb
description: Exchange で EWS マネージ API または EWS を使用して、連絡先グループを作成する方法について説明します。
ms.openlocfilehash: 1da876bbda72f5bea08fd9855aa3f554135d54aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528140"
---
# <a name="create-contact-groups-by-using-ews-in-exchange"></a><span data-ttu-id="67333-103">Exchange で EWS を使用して連絡先グループを作成する</span><span class="sxs-lookup"><span data-stu-id="67333-103">Create contact groups by using EWS in Exchange</span></span>

<span data-ttu-id="67333-104">Exchange で EWS マネージ API または EWS を使用して、連絡先グループを作成する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="67333-104">Learn how to create a contact group by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="67333-105">EWS マネージ API または EWS を使用して、個人用[配布グループ](distribution-groups-and-ews-in-exchange.md)である連絡先グループを作成できます。</span><span class="sxs-lookup"><span data-stu-id="67333-105">You can create a contact group, which is a private [distribution group](distribution-groups-and-ews-in-exchange.md), by using the EWS Managed API or EWS.</span></span> <span data-ttu-id="67333-106">連絡先グループを作成するには、[ContactGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) EWS マネージ API クラスのメソッドを使用するか、[CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="67333-106">To create contact groups, use the methods in the [ContactGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) EWS Managed API class, or use the [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation.</span></span> 
  
<span data-ttu-id="67333-107">EWS マネージ API と EWS のどちらを使用したとしても、ユニバーサル配布グループもセキュリティ グループも作成できません。</span><span class="sxs-lookup"><span data-stu-id="67333-107">Note that you can't use the EWS Managed API or EWS to create a universal distribution group or security group.</span></span> <span data-ttu-id="67333-108">ユニバーサル配布グループまたはセキュリティ グループを作成するには、[New-DistributionGroup](https://technet.microsoft.com/library/aa998856%28v=exchg.150%29.aspx) [Exchange 管理シェル コマンドレット](https://msdn.microsoft.com/library/ff326159%28v=exchg.140%29.aspx)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="67333-108">To create a universal distribution group or security group, you can use the [New-DistributionGroup](https://technet.microsoft.com/library/aa998856%28v=exchg.150%29.aspx)[Exchange Management Shell cmdlet](https://msdn.microsoft.com/library/ff326159%28v=exchg.140%29.aspx).</span></span> 
  
## <a name="create-a-contact-group-by-using-the-ews-managed-api"></a><span data-ttu-id="67333-109">EWS マネージ API を使用して連絡先グループを作成する</span><span class="sxs-lookup"><span data-stu-id="67333-109">Create a contact group by using the EWS Managed API</span></span>
<span data-ttu-id="67333-110"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="67333-110"><a name="bk_EWSMA"> </a></span></span>

<span data-ttu-id="67333-p103">連絡先グループを作成するために必要となるのは、2 つの情報、つまりグループの名前とグループに追加するメンバーだけです。次の例は、2 人のグループ メンバーが含まれる簡単な連絡先グループを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="67333-p103">To create a contact group, you just need a couple pieces of information: a name for the group, and the members to add to the group. The following example shows how to create a simple contact group that contains a couple of group members.</span></span>
  
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

## <a name="create-a-contact-group-by-using-ews"></a><span data-ttu-id="67333-113">EWS を使用して連絡先グループを作成する</span><span class="sxs-lookup"><span data-stu-id="67333-113">Create a contact group by using EWS</span></span>
<span data-ttu-id="67333-114"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="67333-114"><a name="bk_EWSMA"> </a></span></span>

<span data-ttu-id="67333-p104">コードがさらに数行必要となる可能性がありますが、[CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS 操作を使用して連絡先グループを作成できます。次の XML 要求例は、連絡先グループを作成する方法を示しています。またこれは、[EWS マネージ API を使用して連絡先グループを作成する](#bk_EWSMA)際に、送信される XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="67333-p104">It might take a few more lines of code, but you can create a contact group by using the [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation. The following XML request example shows how you can create a contact group. This is also the XML request that is sent when you [use the EWS Managed API to create a contact group](#bk_EWSMA).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
   <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
MessageDisposition="SaveOnly">
      <Items xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
         <DistributionList xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
            <DisplayName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               My Contact Group
            </DisplayName>
            <Members xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <Member xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                  <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                     <EmailAddress xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                        sadie@contoso.com
                     </EmailAddress>
                  </Mailbox>
               </Member>
               <Member xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                  <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                     <EmailAddress xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                        alfred@contoso.com
                     </EmailAddress>
                  </Mailbox>
               </Member>
            </Members>
         </DistributionList>
      </Items>
   </CreateItem>
```

<span data-ttu-id="67333-p105">要求に対して成功した XML 応答の例を次に示します。返される値に、新しい連絡先グループのアイテム ID、および連絡先グループを変更したり、グループを展開してメンバーを表示したりするために他のコードで使用できる変更キーが含まれている点に注目してください。アイテム ID は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="67333-p105">The following is an example of a successful XML response to the request. Notice that the values returned include an item ID for the new contact group and a change key that you can use in other code to modify the contact group or expand the group to see the members. The item ID is shortened for readability.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
   <CreateItemResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <CreateItemResponseMessage ResponseClass="Success" 
             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
            <ResponseCode xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
               NoError
            </ResponseCode>
            <Items xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
               <DistributionList xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                  <ItemId xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                          Id="AAMkADBlY…" 
                          ChangeKey="EgAAABYAAAAD7hO1SJPWTbICFWZ4U3NMAABXzQiK" />
               </DistributionList>
            </Items>
         </CreateItemResponseMessage>
      </ResponseMessages>
   </CreateItemResponse>
```

## <a name="see-also"></a><span data-ttu-id="67333-121">関連項目</span><span class="sxs-lookup"><span data-stu-id="67333-121">See also</span></span>


- [<span data-ttu-id="67333-122">Exchange の配布グループと EWS</span><span class="sxs-lookup"><span data-stu-id="67333-122">Distribution groups and EWS in Exchange</span></span>](distribution-groups-and-ews-in-exchange.md)
    
- [<span data-ttu-id="67333-123">Exchange 2013 の EWS を使用して配布グループを展開する</span><span class="sxs-lookup"><span data-stu-id="67333-123">Expand distribution groups by using EWS in Exchange 2013</span></span>](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

