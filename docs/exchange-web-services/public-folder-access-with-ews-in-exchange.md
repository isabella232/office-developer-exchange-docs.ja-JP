---
title: Exchange での EWS を使用したパブリック フォルダー アクセス
manager: sethgros
ms.date: 7/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d9372057-1deb-45de-8f98-b9149604429a
description: EWS および EWS のマネージ API を使用して、パブリック フォルダーにアクセスし、Exchange パブリック フォルダーの要求をルーティングする方法について説明します。
ms.openlocfilehash: cfa089ba617dc760ed12883590e141debb5ecd9b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759184"
---
# <a name="public-folder-access-with-ews-in-exchange"></a>Exchange での EWS を使用したパブリック フォルダー アクセス

EWS および EWS のマネージ API を使用して、パブリック フォルダーにアクセスし、Exchange パブリック フォルダーの要求をルーティングする方法について説明します。
  
パブリック フォルダーでは、組織内のユーザーがアクセスできるアイテムの共有リポジトリを提供します。 Office 365、Exchange Online では、および設置型のバージョンの Exchange が Exchange 2013 で始まるは、パブリック フォルダー用の新しいアーキテクチャを紹介します。 Exchange のパブリック フォルダーは、パブリック フォルダー階層とパブリック フォルダーの内容を保存する (パブリック フォルダー データベース) ではなく特別なメールボックスのデザインを使用します。 パブリック フォルダーのアクセス許可は、役割ベースのアクセス制御 (RBAC) によって管理されます。
  
Exchange Web サービス (EWS) や EWS マネージ API などのクライアント アクセス テクノロジにより、パブリック フォルダー階層とパブリック フォルダー データベース内のコンテンツ アイテムにプログラムからアクセスできます。この記事では、パブリック フォルダーとパブリック フォルダー データにアクセスするために、EWS と EWS マネージ API を使用する方法について説明します。  
  
## <a name="ews-operations-and-ews-managed-api-methods-for-public-folder-access"></a>パブリック フォルダーへのアクセスのための EWS 操作と EWS マネージ API 
<a name="bk_functionality"> </a>

主要な EWS 操作のほとんどは、パブリック フォルダーへのアクセスをサポートしています。次の表に示したフォルダーとアイテムの操作および EWS マネージ API のメソッドは、パブリック フォルダーに使用できます。
  
EWS のマネージ API のメソッドの詳細については、 [EWS のマネージ API の名前空間](http://msdn.microsoft.com/en-us/library/jj220535%28v=exchg.80%29.aspx)を参照してください。
  
|**EWS 操作**|**EWS マネージ API メソッド**|
|:-----|:-----|
|
  [CreateFolder 操作](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |**Folder.Save()** <br/> |
|
  [UpdateFolder 操作](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |**Folder.Update()** <br/> |
|[DeleteFolder 操作](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |**Folder.Delete()** <br/> |
|[MoveFolder 操作](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx)<sup>1</sup> <br/> |**Folder.Move()** <br/> |
|[CopyFolder 操作](http://msdn.microsoft.com/library/c7ea0d68-9793-4144-b378-d99536776db9%28Office.15%29.aspx)<sup>2</sup> <br/> |**Folder.Copy()** <br/> |
|
  [GetFolder 操作](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |**Folder.Bind()** <br/> |
|[EmptyFolder 操作](http://msdn.microsoft.com/library/98161486-e2f2-480f-8d5d-708ba81b208a%28Office.15%29.aspx)<sup>3</sup> <br/> |**Folder.Empty()** <br/> |
|
  [FindFolder 操作](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |**ExchangeService.FindFolders()** <br/> **Folder.FindFolders()** <br/> |
|
  [CreateItem 操作](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |**Item.Save()** <br/> |
|
  [MoveItem 操作](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |**Item.Move()** <br/> |
|
  [CopyItem 操作](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |**Item.Copy()** <br/> |
|
  [UpdateItem 操作](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |**Item.Update()** <br/> |
|[DeleteItem の操作](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |**Item.Delete()** <br/> |
|[FindItem 操作](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)<sup>4</sup> <br/> |**ExchangeService.FindItems()** <br/> **Folder.FindItems()** <br/> |
|
  [GetItem 操作](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |**Item.Bind()** <br/> |
|[ConvertId 操作](http://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx)<sup>5</sup> <br/> |**ExchangeService.ConvertId()** <br/> **ExchangeService.ConvertIds()** <br/> |
   
<sup>1</sup>パブリック フォルダーとプライベート フォルダー間でフォルダーの移動では使用できませんのバージョンの Exchange が Exchange 2013 で開始します。 
  
<sup>2</sup>この操作は、Exchange Server 2007 と Exchange Server 2010 のパブリック フォルダーに該当する場合のみです。 
  
<sup>3</sup>この操作はパブリック フォルダーを Exchange 2010 です。 
  
<sup>4</sup>バージョンの Exchange が Exchange 2013 で始まるクエリ文字列の検索] オプションを使用して単一のパブリック フォルダーのフルテキスト インデックスを使った検索がサポートされます。 
  
<sup>5</sup> ConvertId 操作正しくに変換できないパブリック フォルダーの識別子 EWS 識別子からストア識別子。 [回避策](http://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx#bk_usingConvertId)として返される id を手動で更新することができます。
  
次の操作はサポートされていませんか、部分的にサポートされて、バージョンの Exchange が Exchange 2013 で始まるパブリック フォルダーの。
  
- **CopyFolder**(サポートされていません)。 **CopyFolder**操作機能を実装するために、 **CopyItems**操作で**CreateFolder**を使用できます。 
    
- **EmptyFolder**(サポートされていません)。 **EmptyFolder**操作機能を実装するのに**DeleteItem**操作**FindItem**を使用できます。 
    
- **MoveFolder**(部分的にサポートされている)。 プライベートおよびパブリック フォルダー間でフォルダーを移動できません。 フォルダーは、Exchange 2007 でのプライベートおよびパブリック フォルダーと Exchange 2010 の間で移動できます。 すべてのバージョンの Exchange のパブリック フォルダー内でフォルダーを移動できます。 
    
EWS と EWS マネージ API では、パブリック フォルダーに対する次の機能がサポートされません。
  
- **SyncFolderHierarchy**を使用します。 **FindFolder**、 **GetFolder** **SyncFolderItems**の操作を使用して、パブリック フォルダーのメールボックスのアイテムとフォルダーを同期します。 
    
- パブリック フォルダー階層の深いトラバーサル検索します。 パブリック フォルダー階層の走査を使用して再帰的な**FindFolder**操作呼び出し。 
    
- **CreateFolderPath**操作を使用して、パブリック フォルダーのフォルダー階層を作成します。 パブリック フォルダーのメールボックスを対象とする場合、個別のフォルダー階層のフォルダー レベルごとに**CreateFolder**操作を使用する必要があります。 
    
- **CreateItem**操作を使用して、送信済み電子メール メッセージのコピーを保存します。 代わりに、パブリック フォルダーにメッセージのコピーを移動するのには、 **MoveItem**操作を使用します。 
    
## <a name="scenarios-for-using-ews-and-the-ews-managed-api-to-work-with-public-folders"></a>パブリック フォルダーの操作に EWS と EWS マネージ API を使用するシナリオ
<a name="bk_scenarios"> </a>

Exchange メールボックス ユーザーにとって重要なシナリオの多くは、パブリック フォルダーによって可能になります。EWS と EWS マネージ API を使用して、パブリック フォルダーにアクセスしてそのコンテンツを使用するためのカスタム ソリューションを実装することで、ユーザーの能力を強化できます。  
  
### <a name="programmatically-access-email-messages-that-have-been-sent-to-distribution-lists"></a>配布リストに送信された電子メール メッセージへのプログラムによるアクセス

Exchange メールボックスのユーザーは、配布リストに送信される電子メール メッセージを格納するのにパブリック フォルダーを使用することができます。 これは、配布リストの履歴を保存する場合に便利です。 EWS の[FindItem 操作](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)または EWS のマネージ API の**ExchangeService.FindItems()** および**Folder.FindItems()** メソッドを使用するには、ストアドの配布リストの電子メール メッセージにアクセスします。 
  
### <a name="share-important-email-messages-and-other-mailbox-items"></a>重要な電子メール メッセージなどのメールボックス アイテムの共有

メールボックス ユーザーは、メールボックスのアイテムの共有リポジトリとしてパブリック フォルダーを使用できます。 組織内の別のユーザーは、パブリック フォルダーを使用して、重要な電子メール メッセージや連絡先を共有できます。 EWS では、これらのアイテムの共有メールボックスへのアクセスを提供できます。 EWS は、 [MoveItem 操作](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx)または EWS のマネージ API では、 **Item.Move()** メソッドを使用すると、パブリック フォルダーとの間に、電子メール メッセージ、連絡先、およびその他のメールボックス アイテムを移動します。 
  
### <a name="public-discussions-with-post-items"></a>投稿アイテムによるパブリック ディスカッション

パブリック フォルダーは、投稿アイテムの便利なコンテナーです。 投稿アイテムは、ユーザー間で電子メール メッセージを送信することがなく、スレッド化された会話を使用する方法を提供します。 ユーザーは、パブリック フォルダーを使用しをホストし、組織内の別のメールボックスのユーザーの間でスレッド化された会話を管理するアイテムを投稿できます。 この方法では、メールボックス ユーザーは共有を使用してアイテムを投稿する、会話に参加されなかった場合でも、[会話の履歴にアクセスできます。 EWS は、 [CreateItem 操作](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)または EWS のマネージ API では、 **Item.Save()** メソッドを使用するには、両方を作成し、パブリック フォルダーに格納されているアイテムを投稿するのには応答します。 
  
## <a name="routing-public-folder-requests"></a>パブリック フォルダー要求のルーティング
<a name="bk_routing"> </a>

パブリック フォルダーのコンテンツは、複数のメールボックス サーバーに保存できます。パブリック フォルダー階層を保存するメールボックスと、パブリック フォルダーのコンテンツを保存するメールボックスを別にすることができます。そのため、それらのサーバーとユーザーが情報を要求するメールボックス サーバーが異なることもあります。このような場合は、追加の X-AnchorMailbox ヘッダーと X-PublicFolderMailbox ヘッダーをパブリック フォルダー要求に含めることで、パブリック フォルダーに関する正確な情報を受け取れるようにすることが重要です。
  
X-AnchorMailbox と X-PublicFolderMailbox の値は、実行している要求がフォルダー階層に関連するものか、フォルダー コンテンツに関連するものかによって異なることがあります。次の表では、EWS マネージ API メソッドまたは EWS 操作ごとに従う手順を示しています。
  
**EWS のマネージ API のメソッドとパブリック フォルダーの要求を送信する EWS 運用**

|**これらのメソッドを呼び出すときに**|**これらの操作を呼び出すときに**|**この手順を使用します。**|
|:-----|:-----|:-----|
|[Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [Folder.Move](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [MoveFolder](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |パブリック フォルダー階層の要求をルーティングする  <br/> |
|[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [Item.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> [Item.Copy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> [Item.Move](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> [Item.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> [Folder.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> [CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |パブリック フォルダー コンテンツ要求をルーティングする  <br/> |
   
## <a name="version-differences"></a>バージョンの相違点
<a name="VersionDifferences"> </a>

Exchange 2007 および Exchange 2010 では、 **ConvertId**操作は、EWS 識別子からパブリック フォルダーの識別子をストア識別子に変換するときに期待どおりに動作します。 
  
## <a name="see-also"></a>関連項目


- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    
- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)
    
- [パブリック フォルダーの制限](http://technet.microsoft.com/en-us/library/dn594582%28v=exchg.150%29.aspx)
    
- [よく寄せられる質問: パブリック フォルダー](http://technet.microsoft.com/en-us/library/jj552408.aspx)
    
- [パブリック フォルダーの手順](http://technet.microsoft.com/en-us/library/jj657481.aspx)
    

