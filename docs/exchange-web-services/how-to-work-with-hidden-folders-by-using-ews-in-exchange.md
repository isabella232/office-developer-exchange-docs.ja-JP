---
title: Exchange EWS を使用して非表示のフォルダーの操作します。
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7ae7c045-cd90-4c9f-baf5-0464d5058f45
description: Exchange で EWS マネージ API または EWS を使用して、フォルダーを非表示にしたり、隠しフォルダーを検索したりする方法について説明します。
ms.openlocfilehash: 72efc16ecc247d307b7300526e7d345fe6bdd3ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759078"
---
# <a name="work-with-hidden-folders-by-using-ews-in-exchange"></a><span data-ttu-id="f0a52-103">Exchange EWS を使用して非表示のフォルダーの操作します。</span><span class="sxs-lookup"><span data-stu-id="f0a52-103">Work with hidden folders by using EWS in Exchange</span></span>

<span data-ttu-id="f0a52-104">Exchange で EWS マネージ API または EWS を使用して、フォルダーを非表示にしたり、隠しフォルダーを検索したりする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="f0a52-104">Learn how to make a folder hidden and find hidden folders by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="f0a52-105">1 つの例外を除き、Exchange メールボックス (IPM 以外のサブツリー) のルートにフォルダーが非表示にします。</span><span class="sxs-lookup"><span data-stu-id="f0a52-105">With one exception, folders in the root of an Exchange mailbox (the non-IPM subtree) are hidden from the user.</span></span> <span data-ttu-id="f0a52-106">逆に、 **MsgFolderRoot** (IPM サブツリー) のすべてのフォルダーは、ユーザーに表示します。</span><span class="sxs-lookup"><span data-stu-id="f0a52-106">Conversely, all folders in the **MsgFolderRoot** (the IPM subtree) are visible to the user.</span></span> <span data-ttu-id="f0a52-107">**MsgFolderRoot**の下のフォルダーを非表示にする方法は、でしょうか。</span><span class="sxs-lookup"><span data-stu-id="f0a52-107">So how do you hide a folder under the **MsgFolderRoot**?</span></span> <span data-ttu-id="f0a52-108">厄介なことはありません-それは 1 つの[PidTagAttributeHidden](http://msdn.microsoft.com/ja-jp/library/cc433490%28v=exchg.80%29.aspx) (0x10F4000B) 拡張プロパティにします。</span><span class="sxs-lookup"><span data-stu-id="f0a52-108">It's not that tricky — it comes down to just one property, the [PidTagAttributeHidden](http://msdn.microsoft.com/ja-jp/library/cc433490%28v=exchg.80%29.aspx) (0x10F4000B) extended property.</span></span> <span data-ttu-id="f0a52-109">このプロパティが**true**に設定、Outlook またはフォルダーの表示/非表示を決定するプロパティを使用して別のクライアントが非表示にユーザーのビューからフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="f0a52-109">When this property is set to **true**, Outlook or another client that uses the property to determine folder visibility will hide the folder from the user's view.</span></span> <span data-ttu-id="f0a52-110">これは拡張プロパティであるため、ため、この資料の指示に従って、主なシナリオを使用して、平均フォルダーのプロパティよりも複雑ですが。</span><span class="sxs-lookup"><span data-stu-id="f0a52-110">Because this is an extended property, it's more complex to use than your average folder property, so this article will walk you through the main scenarios.</span></span>
  
<span data-ttu-id="f0a52-111">**表 1 です。EWS のマネージ API のメソッドと非表示のフォルダーを操作するための EWS の操作**</span><span class="sxs-lookup"><span data-stu-id="f0a52-111">**Table 1. EWS Managed API methods and EWS operations for working with hidden folders**</span></span>

|<span data-ttu-id="f0a52-112">**タスク**</span><span class="sxs-lookup"><span data-stu-id="f0a52-112">**Task**</span></span>|<span data-ttu-id="f0a52-113">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="f0a52-113">**EWS Managed API method**</span></span>|<span data-ttu-id="f0a52-114">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="f0a52-114">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f0a52-115">フォルダーの非表示</span><span class="sxs-lookup"><span data-stu-id="f0a52-115">Hide a folder</span></span>  <br/> |<span data-ttu-id="f0a52-116">[Folder.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) [Folder.Update](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx)の後に</span><span class="sxs-lookup"><span data-stu-id="f0a52-116">[Folder.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) followed by [Folder.Update](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="f0a52-117">[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)の後に</span><span class="sxs-lookup"><span data-stu-id="f0a52-117">[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) followed by [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="f0a52-118">隠しフォルダーの検索</span><span class="sxs-lookup"><span data-stu-id="f0a52-118">Find hidden folders</span></span>  <br/> |[<span data-ttu-id="f0a52-119">FindFolders</span><span class="sxs-lookup"><span data-stu-id="f0a52-119">FindFolders</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="f0a52-120">FindFolder</span><span class="sxs-lookup"><span data-stu-id="f0a52-120">FindFolder</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="f0a52-121">かわからない 1 つの例外とは何です-は、ルートには、どのようなフォルダーは、ユーザーに表示されるでしょうか。</span><span class="sxs-lookup"><span data-stu-id="f0a52-121">Are you wondering what the one exception is — that is, what folder in the root IS visible to users?</span></span> <span data-ttu-id="f0a52-122">ユーザーの検索フォルダーが含まれている検索フォルダー (**使用して**[WellKnownFolder](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx)の列挙値、または**使用して**[DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx)要素の値とも呼ばれます) することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="f0a52-122">It's the Finder folder (also known as the **SearchFolders**[WellKnownFolder](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) enumeration value, or the **searchfolders**[DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) element value), which contains users' search folders.</span></span> <span data-ttu-id="f0a52-123">Finder フォルダーに作成される検索フォルダーは、Outlook ユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="f0a52-123">Search folders created in the Finder folder are visible to Outlook users.</span></span> <span data-ttu-id="f0a52-124">ユーザーに表示されていない検索フォルダーを作成する場合は、非表示にするにはルート フォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="f0a52-124">If you need to create a search folder that is not visible to users, move it under the root folder to hide it.</span></span> <span data-ttu-id="f0a52-125">異なり、他のフォルダーの**PidTagAttributeHidden**プロパティを**true**に設定が非表示に検索フォルダー検索フォルダーにします。</span><span class="sxs-lookup"><span data-stu-id="f0a52-125">Unlike for other folders, setting the **PidTagAttributeHidden** property to **true** will not hide a search folder in the Finder folder.</span></span> 
  
## <a name="hide-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="f0a52-126">EWS マネージ API を使用してフォルダーを非表示にする</span><span class="sxs-lookup"><span data-stu-id="f0a52-126">Hide a folder by using the EWS Managed API</span></span>
<span data-ttu-id="f0a52-127"><a name="bk_hideewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="f0a52-127"></span></span>

<span data-ttu-id="f0a52-128">[PidTagAttributeHidden](http://msdn.microsoft.com/ja-jp/library/cc433490%28v=exchg.80%29.aspx)の拡張プロパティを**true**に変更することでフォルダーを非表示[、既存のフォルダーを作成](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma)できます。</span><span class="sxs-lookup"><span data-stu-id="f0a52-128">You can [make an existing folder](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) a hidden folder by changing the [PidTagAttributeHidden](http://msdn.microsoft.com/ja-jp/library/cc433490%28v=exchg.80%29.aspx) extended property to **true**.</span></span> <span data-ttu-id="f0a52-129">[プロパティの拡張プロパティの定義](properties-and-extended-properties-in-ews-in-exchange.md)を最初に作成するには。</span><span class="sxs-lookup"><span data-stu-id="f0a52-129">First, create an [extended property definition for the property](properties-and-extended-properties-in-ews-in-exchange.md).</span></span> <span data-ttu-id="f0a52-130">次に、 [Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx)メソッドを使用して、フォルダーを取得し、 **PidTagAttributeHidden**プロパティを true にすると、 [Update](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx)メソッドを使用して、変更を保存するの値を更新します。</span><span class="sxs-lookup"><span data-stu-id="f0a52-130">Next, use the [Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method to get to the folder, then update the value of the **PidTagAttributeHidden** property to true, and use the [Update](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
  
<span data-ttu-id="f0a52-131">この例では、その**サービス**が有効な[ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)を Exchange サーバーに、ユーザーが認証されて、その**フォルダー Id**は非表示にするフォルダーを識別する有効な[Folder.Id](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx)メールボックスの所有者のオブジェクトします。</span><span class="sxs-lookup"><span data-stu-id="f0a52-131">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner, that the user has been authenticated to an Exchange server, and that **folderId** is a valid [Folder.Id](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) that identifies the folder to hide.</span></span> 
  
```cs
private static void MakeHidden(FolderId folderId, ExchangeService service)
{
    // Create an extended property definition for the PidTagAttributeHidden property.
    ExtendedPropertyDefinition isHiddenProp = new ExtendedPropertyDefinition(0x10f4, MapiPropertyType.Boolean);
    PropertySet propSet = new PropertySet(isHiddenProp);
    // Bind to a folder and retrieve the PidTagAttributeHidden property.
    Folder folder = Folder.Bind(service, folderId, propSet);
    // Set the PidTagAttributeHidden property to true.
    folder.SetExtendedProperty(isHiddenProp, true);
    // Save the changes.
    folder.Update();
}
```

## <a name="hide-a-folder-by-using-ews"></a><span data-ttu-id="f0a52-132">EWS を使用してフォルダーを非表示にする</span><span class="sxs-lookup"><span data-stu-id="f0a52-132">Hide a folder by using EWS</span></span>
<span data-ttu-id="f0a52-133"><a name="bk_hideews"> </a></span><span class="sxs-lookup"><span data-stu-id="f0a52-133"></span></span>

<span data-ttu-id="f0a52-134">フォルダーを非表示[、既存のフォルダーを作成](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma)するのには EWS を使用するには、拡張プロパティを**true**に[PidTagAttributeHidden](http://msdn.microsoft.com/ja-jp/library/cc433490%28v=exchg.80%29.aspx)を変更します。</span><span class="sxs-lookup"><span data-stu-id="f0a52-134">You can use EWS to [make an existing folder](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) a hidden folder by changing the [PidTagAttributeHidden](http://msdn.microsoft.com/ja-jp/library/cc433490%28v=exchg.80%29.aspx) extended property to **true**.</span></span> <span data-ttu-id="f0a52-135">最初に、 [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)操作を使用して、フォルダーに、 **PidTagAttributeHidden**プロパティを取得するには、 [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx)の要素を含めると、4340 に**PropertyTag**の値と**を登録するときの設定**ブール値です。</span><span class="sxs-lookup"><span data-stu-id="f0a52-135">First, use the [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation to get to the folder, then retrieve the **PidTagAttributeHidden** property by including the [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) element, and setting the **PropertyTag** value to 4340 and the **PropertyType** value to Boolean.</span></span> 
  
<span data-ttu-id="f0a52-136">EWS のマネージ API が[、隠しフォルダーを作成](#bk_hideewsma)する前にフォルダーを取得するのには、 **Bind**メソッドを使用する場合に送信する XML 要求にもです。</span><span class="sxs-lookup"><span data-stu-id="f0a52-136">This is also the XML request that the EWS Managed API sends when you use the **Bind** method to get a folder before [making it a hidden folder](#bk_hideewsma).</span></span>
  
<span data-ttu-id="f0a52-137">[フォルダー Id](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx)の値は、読みやすくするために短縮されます。</span><span class="sxs-lookup"><span data-stu-id="f0a52-137">The [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) value is shortened for readability.</span></span> 
  
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
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:FolderIds>
        <t:FolderId Id="IQywAAAA==" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

**NoError**フォルダーが正常に取得されたことを示すは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素の値を含む[GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx)メッセージで**GetFolder**要求にサーバーが応答します。 応答には、 [ExtendedProperty](http://msdn.microsoft.com/library/f9701409-b620-4afe-b9ee-4c1e95507af7%28Office.15%29.aspx)の[値](http://msdn.microsoft.com/library/196278d4-5e77-4e0a-8af6-8ac065610510%28Office.15%29.aspx)も含まれています。 <span data-ttu-id="f0a52-140">この例では、 **false を指定**するフォルダーは、現在非表示にする**値**が設定されます。</span><span class="sxs-lookup"><span data-stu-id="f0a52-140">In this example, the **Value** is set to **false**, which means that the folder is currently not hidden.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="898"
                         MinorBuildNumber="23"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="IQywAAAA=="
                          ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAAABED" />
              <t:ExtendedProperty>
                <t:ExtendedFieldURI PropertyTag="0x10f4"
                                    PropertyType="Boolean" />
                <t:Value>false</t:Value>
              </t:ExtendedProperty>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="f0a52-141">**ExtendedProperty**の値を true に変更するには、 [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="f0a52-141">To change the value of the **ExtendedProperty** to true, use the [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="f0a52-142">**ExtendedProperty**、 **ExtendedFieldURI**、および**値**要素が含まれます、 **PidTagAttributeHidden**拡張プロパティ、および要素**の値**を**true**に設定、フォルダーを非表示にするのです。</span><span class="sxs-lookup"><span data-stu-id="f0a52-142">Include the **ExtendedProperty**, **ExtendedFieldURI**, and **Value** elements for the **PidTagAttributeHidden** extended property, and set the **Value** element to **true** to hide the folder.</span></span> 
  
<span data-ttu-id="f0a52-143">EWS のマネージ API が[非表示のフォルダー](#bk_hideewsma)にフォルダーを更新する**Update**メソッドを使用する場合に送信する XML 要求にもです。</span><span class="sxs-lookup"><span data-stu-id="f0a52-143">This is also the XML request that the EWS Managed API sends when you use the **Update** method to update a folder to [make it a hidden folder](#bk_hideewsma).</span></span>
  
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
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="IQywAAAA=="
                      ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAAABED" />
          <t:Updates>
            <t:SetFolderField>
              <t:ExtendedFieldURI PropertyTag="4340"
                                  PropertyType="Boolean" />
              <t:Folder>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="4340"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="f0a52-144">**NoError**フォルダーが正常に更新されたが非表示であることを示すは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素の値が含まれています[UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx)メッセージから**UpdateFolder**要求にサーバーが応答します。</span><span class="sxs-lookup"><span data-stu-id="f0a52-144">The server responds to the **UpdateFolder** request with an [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was updated successfully, and is now hidden.</span></span>
  
## <a name="find-all-hidden-folders-by-using-the-ews-managed-api"></a><span data-ttu-id="f0a52-145">EWS マネージ API を使用してすべての隠しフォルダーを検索する</span><span class="sxs-lookup"><span data-stu-id="f0a52-145">Find all hidden folders by using the EWS Managed API</span></span>
<span data-ttu-id="f0a52-146"><a name="bk_findhiddenewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="f0a52-146"></span></span>

<span data-ttu-id="f0a52-147">拡張プロパティ、 **PidTagAttributeHidden**の[拡張プロパティの定義](properties-and-extended-properties-in-ews-in-exchange.md)を作成して、**を含むフォルダーを検索するのには、 [FindFolders](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)メソッドを使用して親フォルダーの下のすべての隠しフォルダーを見つけることができます。PidTagAttributeHidden**を**true**に設定されている値です。</span><span class="sxs-lookup"><span data-stu-id="f0a52-147">You can find all hidden folders under a parent folder by creating an [extended property definition](properties-and-extended-properties-in-ews-in-exchange.md) for the **PidTagAttributeHidden** extended property, and then using the [FindFolders](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) method to find folders with a **PidTagAttributeHidden** value that is set to **true**.</span></span> <span data-ttu-id="f0a52-148">この例では、親フォルダーで検索するとインフォメーション ストアの最上位、または IPM サブツリーとも呼ばれます、MsgFolderRoot を使用します。</span><span class="sxs-lookup"><span data-stu-id="f0a52-148">This example uses the MsgFolderRoot, also known as the Top of Information Store, or IPM Subtree, as the parent folder to search under.</span></span>
  
<span data-ttu-id="f0a52-149">この例でその**サービス**は、メールボックスの所有者の有効な[ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトは、ユーザーが Exchange サーバーに認証されているとします。</span><span class="sxs-lookup"><span data-stu-id="f0a52-149">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner, and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
private static void FindHiddenFolders(ExchangeService service)
{
    // Create an extended property definition for the PidTagAttributeHidden property.
    ExtendedPropertyDefinition isHiddenProp = new ExtendedPropertyDefinition(0x10f4, MapiPropertyType.Boolean);
    // Create a folder view to retrieve up to 100 folders and 
    // retrieve only the PidTagAttributeHidden and the display name.
    FolderView folderView = new FolderView(100);
    folderView.PropertySet = new PropertySet(isHiddenProp, FolderSchema.DisplayName);
    // Indicate a Traversal value of Deep, so that all subfolders are retrieved.
    folderView.Traversal = FolderTraversal.Deep;
    // Find all hidden folders under the MsgFolderRoot.
    // This call results in a FindFolder call to EWS.
    FindFoldersResults findFolder = service.FindFolders(WellKnownFolderName.MsgFolderRoot,
            new SearchFilter.IsEqualTo(isHiddenProp, true), folderView);
    // Display the folder ID and display name of each hidden folder.
    foreach (Folder folder in findFolder)
    {
        Console.WriteLine("FolderId: {0}", folder.Id);
        Console.WriteLine("DisplayName: {0}", folder.DisplayName);
        Console.WriteLine("\r\n");
    }
}
```

## <a name="find-all-hidden-folders-by-using-ews"></a><span data-ttu-id="f0a52-150">EWS を使用してすべての隠しフォルダーを検索する</span><span class="sxs-lookup"><span data-stu-id="f0a52-150">Find all hidden folders by using EWS</span></span>
<span data-ttu-id="f0a52-151"><a name="bk_findhiddenews"> </a></span><span class="sxs-lookup"><span data-stu-id="f0a52-151"></span></span>

<span data-ttu-id="f0a52-152">[FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)操作を呼び出すことによって、既存のフォルダーの下のすべての隠しフォルダーを検索するのには、EWS を使用することができ、検索フォルダーの[PidTagAttributeHidden](http://msdn.microsoft.com/ja-jp/library/cc433490%28v=exchg.80%29.aspx)拡張プロパティが**true**に設定します。</span><span class="sxs-lookup"><span data-stu-id="f0a52-152">You can use EWS to find all hidden folders under an existing folder by calling the [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) operation and searching for folders whose [PidTagAttributeHidden](http://msdn.microsoft.com/ja-jp/library/cc433490%28v=exchg.80%29.aspx) extended property is set to **true**.</span></span> <span data-ttu-id="f0a52-153">(4243 に**PropertyTag**の値とブール値を**登録するとき**の値)、 **PidTagAttributeHidden**プロパティに[ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx)要素を検索する[IsEqualTo](http://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx)[の制限](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx)は、これを行うには、します。示すように次のような要求です。</span><span class="sxs-lookup"><span data-stu-id="f0a52-153">To do this, include an [IsEqualTo](http://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx)[Restriction](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) that searches for the [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) element for the **PidTagAttributeHidden** property ( **PropertyTag** value to 4243 and the **PropertyType** value to Boolean), as shown in the following request.</span></span> <span data-ttu-id="f0a52-154">この例では、親フォルダーで検索するとインフォメーション ストアの最上位、または IPM サブツリーとも呼ばれます、MsgFolderRoot を使用します。</span><span class="sxs-lookup"><span data-stu-id="f0a52-154">This example uses the MsgFolderRoot, also known as the Top of Information Store, or IPM Subtree, as the parent folder to search under.</span></span> 
  
<span data-ttu-id="f0a52-155">EWS のマネージ API が[すべての隠しフォルダーを検索](#bk_findhiddenewsma)する**FindFolders**メソッドを使用する場合に送信する XML 要求にもです。</span><span class="sxs-lookup"><span data-stu-id="f0a52-155">This is also the XML request that the EWS Managed API sends when you use the **FindFolders** method to [find all hidden folders](#bk_findhiddenewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Central Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Deep">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
          <t:FieldURI FieldURI="folder:DisplayName" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="100"
                               Offset="0"
                               BasePoint="Beginning" />
      <m:Restriction>
        <t:IsEqualTo>
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
          <t:FieldURIOrConstant>
            <t:Constant Value="true" />
          </t:FieldURIOrConstant>
        </t:IsEqualTo>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="msgfolderroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="f0a52-156">サーバー要求に応答し、 **FindFolder** **NoError**フォルダーの検索が成功したことを示すの[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素の値が含まれています[FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx)のメッセージをすべての非表示メッセージのルート フォルダーの下のフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="f0a52-156">The server responds to the **FindFolder** request with a [FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder search was successful, as well as all the hidden folders under the root message folder.</span></span>
  
<span data-ttu-id="f0a52-157">[フォルダー Id](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx)の値は、読みやすくするために短縮されます。</span><span class="sxs-lookup"><span data-stu-id="f0a52-157">The [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) values are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="898"
                         MinorBuildNumber="23"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="6"
                        TotalItemsInView="6"
                        IncludesLastItemInRange="true">
            <t:Folders>
              <t:ContactsFolder>
                <t:FolderId Id="IBHgAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAACz" />
                <t:DisplayName>{06967759-274D-40B2-A3EB-D7F9E73727D7}</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="IBHwAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAAC7" />
                <t:DisplayName>{A9E2BC46-B3A0-4243-B315-60D991004455}</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="IBIQAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAADO" />
                <t:DisplayName>GAL Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="IBHQAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAACa" />
                <t:DisplayName>Recipient Cache</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="HAAAAA=="
                            ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAAAACS" />
                <t:DisplayName>Conversation Action Settings</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
              <t:Folder>
                <t:FolderId Id="IQywAAAA=="
                            ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAeZIBf" />
                <t:DisplayName>TestFolder</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

## 
<span data-ttu-id="f0a52-158"><a name="bk_findhiddenews"> </a></span><span class="sxs-lookup"><span data-stu-id="f0a52-158"></span></span>

<span data-ttu-id="f0a52-159">後非表示にするか、ウィンドウのフォルダー階層のフォルダーまたは[フォルダー階層を同期](how-to-synchronize-folders-by-using-ews-in-exchange.md)させようとする可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f0a52-159">After you have hidden or unhidden folders, you might want to get the folder hierarchy or [synchronize the folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="f0a52-160">どの[EWS のマネージ API を使用してフォルダーの階層を取得](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyewsma)または[EWS を使用してフォルダーの階層を取得](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyews)するも指定した階層内のどのフォルダーを表示する例としては表示されません。</span><span class="sxs-lookup"><span data-stu-id="f0a52-160">The examples that show you how to [get a folder hierarchy by using the EWS Managed API](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyewsma) or [get a folder hierarchy by using EWS](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyews) also indicate which folders in the hierarchy are hidden.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="f0a52-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="f0a52-161">See also</span></span>


- [<span data-ttu-id="f0a52-162">Exchange の EWS のフォルダーとアイテム</span><span class="sxs-lookup"><span data-stu-id="f0a52-162">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    
- [<span data-ttu-id="f0a52-163">Exchange EWS を使用してフォルダーを操作します。</span><span class="sxs-lookup"><span data-stu-id="f0a52-163">Work with folders by using EWS in Exchange</span></span>](how-to-work-with-folders-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="f0a52-164">EWS を使用して Exchange で検索フォルダーを使用します。</span><span class="sxs-lookup"><span data-stu-id="f0a52-164">Work with search folders by using EWS in Exchange</span></span>](how-to-work-with-search-folders-by-using-ews-in-exchange.md)
    

