---
title: Exchange での EWS を使用したパブリック フォルダー アクセス
manager: sethgros
ms.date: 7/17/2015
ms.audience: Developer
ms.assetid: d9372057-1deb-45de-8f98-b9149604429a
description: パブリック フォルダーへのアクセスとパブリック フォルダー要求のルーティングに、Exchange の EWS と EWS マネージ API を使用する方法について説明します。
localization_priority: Priority
ms.openlocfilehash: e921a77b250e11e974b0c47b1d28a8e020837d44
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460212"
---
# <a name="public-folder-access-with-ews-in-exchange"></a>Exchange での EWS を使用したパブリック フォルダー アクセス

パブリック フォルダーへのアクセスとパブリック フォルダー要求のルーティングに、Exchange の EWS と EWS マネージ API を使用する方法について説明します。
  
パブリック フォルダーは、組織内のユーザーがアクセスできるアイテムの共有リポジトリを提供します。 Office 365、Exchange Online、および Exchange 2013 以降の Exchange のオンプレミス バージョンでは、新しいアーキテクチャのパブリック フォルダーが導入されています。 Exchange のパブリック フォルダーは、特別なメールボックスの設計 (パブリック フォルダー データベースの代わり) を使用して、パブリック フォルダー階層とパブリック フォルダーの内容を格納します。 パブリック フォルダーのアクセス許可は役割ベースのアクセス制御 (RBAC) で管理します。
  
Exchange Web サービス (EWS) や EWS マネージ API などのクライアント アクセス テクノロジにより、パブリック フォルダー階層とパブリック フォルダー データベース内のコンテンツ アイテムにプログラムからアクセスできます。この記事では、パブリック フォルダーとパブリック フォルダー データにアクセスするために、EWS と EWS マネージ API を使用する方法について説明します。  
  
## <a name="ews-operations-and-ews-managed-api-methods-for-public-folder-access"></a>パブリック フォルダーへのアクセスのための EWS 操作と EWS マネージ API
<a name="bk_functionality"> </a>

主要な EWS 操作のほとんどは、パブリック フォルダーへのアクセスをサポートしています。次の表に示したフォルダーとアイテムの操作および EWS マネージ API のメソッドは、パブリック フォルダーに使用できます。
  
EWS マネージ API のメソッドの詳細については、「[EWS マネージ API の名前空間](https://msdn.microsoft.com/library/jj220535%28v=exchg.80%29.aspx)」を参照してください。
  
|**EWS 操作**|**EWS マネージ API メソッド**|
|:-----|:-----|
|[CreateFolder 操作](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |**Folder.Save()** <br/> |
|[UpdateFolder 操作](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |**Folder.Update()** <br/> |
|[DeleteFolder 操作](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |**Folder.Delete()** <br/> |
|[MoveFolder 操作](https://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx)<sup>1</sup> <br/> |**Folder.Move()** <br/> |
|[CopyFolder 操作](https://msdn.microsoft.com/library/c7ea0d68-9793-4144-b378-d99536776db9%28Office.15%29.aspx)<sup>2</sup> <br/> |**Folder.Copy()** <br/> |
|[GetFolder 操作](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |**Folder.Bind()** <br/> |
|[EmptyFolder 操作](https://msdn.microsoft.com/library/98161486-e2f2-480f-8d5d-708ba81b208a%28Office.15%29.aspx)<sup>3</sup> <br/> |**Folder.Empty()** <br/> |
|[FindFolder 操作](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |**ExchangeService.FindFolders()** <br/> **Folder.FindFolders()** <br/> |
|[CreateItem 操作](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |**Item.Save()** <br/> |
|[MoveItem 操作](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |**Item.Move()** <br/> |
|[CopyItem 操作](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |**Item.Copy()** <br/> |
|[UpdateItem 操作](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |**Item.Update()** <br/> |
|[DeleteItem 操作](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |**Item.Delete()** <br/> |
|[FindItem 操作](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)<sup>4</sup> <br/> |**ExchangeService.FindItems()** <br/> **Folder.FindItems()** <br/> |
|[GetItem 操作](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |**Item.Bind()** <br/> |
|[ConvertId 操作](https://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx)<sup>5</sup> <br/> |**ExchangeService.ConvertId()** <br/> **ExchangeService.ConvertIds()** <br/> |
   
<sup>1</sup> パブリック フォルダーと非公開フォルダー間のフォルダー移動は、Exchange 2013 以降の Exchange のバージョンでは利用できません。 
  
<sup>2</sup> この操作は、Exchange Server 2007 と Exchange Server 2010 のパブリック フォルダーにのみ適用されます。 
  
<sup>3</sup> この操作は、Exchange 2010 のパブリック フォルダーにのみ適用されます。 
  
<sup>4</sup> QueryString 検索オプションによる単一パブリック フォルダー内でのテキスト全体のインデックス付き検索は、Exchange 2013 以降の Exchange のバージョンでサポートされています。 
  
<sup>5</sup> ConvertId 操作では、パブリック フォルダーの識別子は EWS の識別子からストアの識別子に正しく変換されません。 [回避策](https://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx#bk_usingConvertId)として、返された識別子を手動で更新してください。
  
次に示す操作は、Exchange 2013 以降の Exchange のバージョンではサポートされていません (または、部分的にサポートされています)。
  
- **CopyFolder** (サポート対象外)。**CopyItems** 操作で **CreateFolder** を使用すると、**CopyFolder** 操作の機能を実装できます。 
    
- **EmptyFolder** (サポート対象外)。**DeleteItem** 操作で **FindItem** を使用すると、**EmptyFolder** 操作の機能を実装できます。 
    
- **MoveFolder** (部分的にサポート)。プライベート フォルダーとパブリック フォルダーの間でフォルダーを移動することはできません。Exchange 2007 と Exchange 2010 では、プライベート フォルダーとパブリック フォルダーの間でフォルダーを移動できます。Exchange のすべてのバージョンで、パブリック フォルダー内でのフォルダーの移動が可能です。 
    
EWS と EWS マネージ API では、パブリック フォルダーに対する次の機能がサポートされません。
  
- **SyncFolderHierarchy** の使用。 パブリック フォルダー メールボックス内のアイテムとフォルダーを同期する場合は、**FindFolder**、**GetFolder**、および **SyncFolderItems** の操作を使用します。 
    
- パブリック フォルダー階層の一括 (Deep Traversal) 検索。パブリック フォルダー階層をスキャンする場合は、再帰的な **FindFolder** 操作の呼び出しを使用してください。 
    
- パブリック フォルダーのフォルダー階層を作成するための **CreateFolderPath** 操作の使用。パブリック フォルダー メールボックスを対象にする場合は、別のフォルダー階層でフォルダー レベルごとに **CreateFolder** 操作を使用することが必要になります。 
    
- 送信した電子メール メッセージのコピーを保存するための **CreateItem** 操作の使用。代わりに、**MoveItem** 操作を使用してメッセージのコピーをパブリック フォルダーに移動します。 
    
## <a name="scenarios-for-using-ews-and-the-ews-managed-api-to-work-with-public-folders"></a>パブリック フォルダーの操作に EWS と EWS マネージ API を使用するシナリオ
<a name="bk_scenarios"> </a>

Exchange メールボックス ユーザーにとって重要なシナリオの多くは、パブリック フォルダーによって可能になります。EWS と EWS マネージ API を使用して、パブリック フォルダーにアクセスしてそのコンテンツを使用するためのカスタム ソリューションを実装することで、ユーザーの能力を強化できます。  
  
### <a name="programmatically-access-email-messages-that-have-been-sent-to-distribution-lists"></a>配布リストに送信された電子メール メッセージへのプログラムによるアクセス

Exchange メールボックスのユーザーは、配布リストに送信された電子メール メッセージを保存するために、パブリック フォルダーを使用できます。 これは、配布リストの履歴を保存する際に便利な方法です。 EWS の [FindItem 操作](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)、または EWS マネージ API の **ExchangeService.FindItems()** メソッドと **Folder.FindItems()** メソッドを使用すると、保存されている配布リストの電子メール メッセージにアクセスできます。 
  
### <a name="share-important-email-messages-and-other-mailbox-items"></a>重要な電子メール メッセージなどのメールボックス アイテムの共有

メールボックス ユーザーは、メールボックス アイテムの共有リポジトリとしてパブリック フォルダーを使用できます。 組織内の異なるユーザーは、パブリック フォルダーを使用して重要な電子メール メッセージや連絡先を共有できます。 EWS により、このように共有されたメールボックスのアイテムにアクセスできます。 EWS の [MoveItem 操作](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx)、または EWS マネージ API の **Item.Move()** メソッドを使用すると、電子メール メッセージや連絡先などのメールボックスのアイテムをパブリック フォルダーから出し入れできます。 
  
### <a name="public-discussions-with-post-items"></a>投稿アイテムによるパブリック ディスカッション

パブリック フォルダーは、投稿アイテムの便利なコンテナーになります。 投稿アイテムは、ユーザー間で電子メールを送信することなく、スレッド化された会話を行う方法を提供します。 ユーザーは、組織内の異なるメールボックス ユーザー間のスレッド化された会話をホストおよび維持管理するために、パブリック フォルダーと投稿アイテムを使用できます。 この方法により、メールボックス ユーザーは、会話に加わっていない場合でも、投稿アイテムを使用する会話の共有された履歴にアクセスできます。 EWS の [CreateItem 操作](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)、または EWS マネージ API の **Item.Save()** メソッドを使用すると、パブリック フォルダーに保存される投稿アイテムの作成と応答が可能になります。 
  
## <a name="routing-public-folder-requests"></a>パブリック フォルダー要求のルーティング
<a name="bk_routing"> </a>

パブリック フォルダーのコンテンツは、複数のメールボックス サーバーに保存できます。パブリック フォルダー階層を保存するメールボックスと、パブリック フォルダーのコンテンツを保存するメールボックスを別にすることができます。そのため、それらのサーバーとユーザーが情報を要求するメールボックス サーバーが異なることもあります。このような場合は、追加の X-AnchorMailbox ヘッダーと X-PublicFolderMailbox ヘッダーをパブリック フォルダー要求に含めることで、パブリック フォルダーに関する正確な情報を受け取れるようにすることが重要です。
  
X-AnchorMailbox と X-PublicFolderMailbox の値は、実行している要求がフォルダー階層に関連するものか、フォルダー コンテンツに関連するものかによって異なることがあります。次の表では、EWS マネージ API メソッドまたは EWS 操作ごとに従う手順を示しています。
  
**パブリック フォルダーの要求をルーティングするための EWS マネージ API のメソッドと EWS の操作**

|**呼び出すメソッド**|**呼び出す操作**|**使用する手順**|
|:-----|:-----|:-----|
|[Folder.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Folder.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [Folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [Folder.Move](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [MoveFolder](https://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |パブリック フォルダー階層の要求をルーティングする  <br/> |
|[Item.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [Item.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> [Item.Copy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> [Item.Move](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> [Item.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> [Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> [Folder.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> |[CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> [CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |パブリック フォルダー コンテンツ要求をルーティングする  <br/> |
   
## <a name="version-differences"></a>バージョンの相違点
<a name="VersionDifferences"> </a>

Exchange 2007 と Exchange 2010 では、パブリック フォルダーの識別子を EWS 識別子からストア識別子に変換する **ConvertId** 操作は期待どおりに動作します。 
  
## <a name="see-also"></a>関連項目


- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    
- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)
    
- [パブリック フォルダーの制限](https://technet.microsoft.com/library/dn594582%28v=exchg.150%29.aspx)
    
- [FAQ: パブリック フォルダー](https://technet.microsoft.com/library/jj552408.aspx)
    
- [パブリック フォルダーの手順](https://technet.microsoft.com/library/jj657481.aspx)
    

