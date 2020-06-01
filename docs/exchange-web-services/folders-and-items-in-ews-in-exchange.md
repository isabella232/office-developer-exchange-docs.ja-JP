---
title: Exchange の EWS のフォルダーとアイテム
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 9d8cf6fa-85a4-45ac-8165-e4d3ab92594e
description: フォルダーおよびメールボックスのアイテムと、EWS マネージ API または EWS クライアントでこれらのアイテムを表す方法について説明します。
localization_priority: Priority
ms.openlocfilehash: 5e206d6973d148c6f70a17a8e7891bf3de7c1533
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455989"
---
# <a name="folders-and-items-in-ews-in-exchange"></a>Exchange の EWS のフォルダーとアイテム

フォルダーおよびメールボックスのアイテムと、EWS マネージ API または EWS クライアントでこれらのアイテムを表す方法について説明します。
  
フォルダーは、Exchange メールボックスの構成要素です。フォルダーには、メール メッセージ、連絡先、予定、会議、タスクなどのメールボックス アイテムを含めたり、その他のフォルダーを含めたりすることができます。Exchange にはさまざまな種類のフォルダーが含まれていますが、フォルダーの種類は非常によく似ています。主な違いは、含まれているアイテムの種類です。
  
ただし、アイテムには固有の種類があります。 アイテムの種類ごとに、アイテムを定義するプロパティまたはスキーマの異なるセットがあります。 この記事では、利用可能なフォルダーとアイテムの種類、およびそれらの相違点について説明します。

<a name="bk_folders"> </a>

## <a name="folders"></a>フォルダー

フォルダーはすべて、同じ基本クラスまたは基本型から派生します。具体的には、EWS マネージ API では [Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) クラス、EWS では [Folder](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) 型から派生します。 次の図は、EWS マネージ API のクラスおよび EWS の型を示しています。 
  
**図 1. EWS マネージ API の Folder クラスと EWS の Folder 型**

![EWS Managed API Folder クラスから派生するクラスと EWS Folder タイプから派生するタイプ (CalendarFolder、ContactsFolder、SearchFolder、および TasksFolder) が表示された図。](media/Ex2013_Folder_OverviewTypes.png)
  
Folder クラスと Folder 型の主な違いは、Folder 型で作成できるのは特定の種類のアイテムのみであるという点です。 もう 1 つの違いは、クライアントでフォルダー内の情報が表示される方法です。 たとえば、Exchange では、予定表フォルダーで予定を作成できます。 予定を作成した後に他の種類のアイテムを予定表フォルダーに移動することはできますが、それらのアイテムは Outlook では表示されません。 Outlook では、[フォルダーに別の種類のアイテムが存在しているとしても](folders-and-items-in-ews-in-exchange.md#bk_item)、予定や会議などの予定表アイテムだけが予定表フォルダーに表示されます。 
  
**表 1. EWS マネージ API の Folder クラスと EWS の Folder 型**

|**EWS マネージ API のクラス**|**EWS の型**|**FolderClass 値**|**内容**|**メモ**|
|:-----|:-----|:-----|:-----|:-----|
|[Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) <br/> |[Folder](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) <br/> |IPF.Note  <br/> |メール メッセージまたはフォルダー。  <br/> | これは、次の EWS マネージ API の [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=EXCHG.80%29.aspx) フォルダーおよび EWS の [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) フォルダーの汎用 Folder クラスまたは型です。 <ul><li>  ルート (IPM サブツリー)</li><li>NonIpmSubtree</li><li>受信トレイ</li><li>削除済みアイテム</li><li>下書き</li><li>ジャーナル</li><li>メモ  </li><li>送信トレイ</li><li>送信済みアイテム</li><li>メッセージ フォルダー</li><li>迷惑メール</li><li>ボイス メール</li></ul> |
|[CalendarFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx) <br/> |[CalendarFolder](https://msdn.microsoft.com/library/48687a78-e757-4c04-9641-bf4302c6b565%28Office.15%29.aspx) <br/> |IPF.Appointment  <br/> |予定および会議。  <br/> |ユーザーが会議出席依頼に応答すると、予定は EWS マネージ API の [WellKnownFolderName.Calendar](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=EXCHG.80%29.aspx) または EWS の [DistinguishedFolderId.CalendarFolder](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) にのみ追加されます。 これらのフォルダーだけが、会議出席依頼や応答との自動対話をサポートします。  <br/><br/>この Folder クラスまたは Folder 型は、予定表ビューの使用をサポートしており、EWS マネージ API の [Folder.FindItem](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=EXCHG.80%29.aspx) メソッドと [CalendarView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) クラス、EWS の [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 操作と [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) 要素を使用して、開始日と終了日に基づいて予定および会議を取得します。  <br/> |
|[ContactsFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx) <br/> |[ContactsFolder](https://msdn.microsoft.com/library/6c299de8-2087-4aeb-8e66-2bc7586509a6%28Office.15%29.aspx) <br/> |IPF.Contact  <br/> |連絡先と配布リスト。  <br/> |なし。  <br/> |
|[SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) <br/> |[SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) <br/> |IPF.Note  <br/> |内容は、制限またはフィルターによって決まります。検索フォルダーにサブフォルダーは含まれていません。  <br/> |検索条件に一致するアイテムは、実際には検索フォルダーに含まれていません。そうではなく、メールボックスの他の場所にあります。  <br/> 検索フォルダーを Outlook で使用可能にするには、検索 (Finder) フォルダーに検索 (Search) フォルダーを作成します。  <br/> |
|[TasksFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) <br/> |[TasksFolder](https://msdn.microsoft.com/library/5a9a4612-8064-4986-b467-c44f268c64df%28Office.15%29.aspx) <br/> |IPF.Task  <br/> |行うべき作業アイテムが含まれています。  <br/> |なし。  <br/> |
   
### <a name="folder-structure"></a>フォルダー構造

フォルダーは、メールボックスの構造を提供します。 これには、EWS の「インフォメーション ストアの先頭」と呼ばれる IPM サブツリーが含まれます。ここで、ほとんどのユーザーは、自分のメールボックスに加え、EWS の非 IPM サブツリーまたはルートに存在する、普段目にすることがないシステム フォルダーを操作します。 ユーザー用のフォルダー構造を示す次の図に、どのフォルダーがユーザーのアイテムで、どれがシステム フォルダーであるかを示します。
  
**図 2. メールボックスのアイテムおよびシステム フォルダー**

![ルート内のシステム フォルダー (インフォメーション ストア内の Favorites、Finder、FreeBusy Data、Top など) が示された図。インフォメーション ストアの Top には、Calendar、Contacts などのユーザー フォルダーがあります。](media/Ex2013_Folder_OverviewSampleHierarchy.png)
  
### <a name="well-known-folders"></a>既知のフォルダー

メールボックス内には、特殊なフォルダーもあります。これらは、EWS マネージ API の既知のフォルダーまたは EWS の識別フォルダーのことです。これらのフォルダーの一部には、フォルダー名、フォルダー構造内での場所、フォルダーを削除可能かどうかについての制限があります。他の「汎用」(特殊ではない) フォルダーには、こうした制限はありません。次の既知のフォルダーまたは識別フォルダーについて理解することは重要です。これらは、ルート システム、ユーザー、検索フォルダーであり、ほとんどの実装に適用できるからです。  
  
**表 2. 基本的な既知のフォルダーおよび識別フォルダー**

|**フレンドリ名**|**EWS マネージ API の **WellKnownFolderName** 値**|**EWS の **DistinguishedFolderId** 値**|**説明**|
|:-----|:-----|:-----|:-----|
|ルート (非 IPM サブツリー)  <br/> |WellKnownFolderName.Root  <br/> |DistinguishedFolderId.root  <br/> |非 IPM サブツリーとも呼ばれる、メールボックスのルート フォルダーが含まれます。このフォルダーには親が含まれていないため、フォルダーを移動、コピー、名前変更、削除することはできません。各メッセージ ストアには 1 つのルート フォルダーだけが含まれます。  <br/> |
|インフォメーション ストアの先頭 (IPM サブツリー)  <br/> |WellKnownFolderName.MsgFolderRoot  <br/> |DistinguishedFolderId.msgfolderroot  <br/> |受信トレイやユーザーのその他のフォルダーが含まれます。  <br/> |
|検索 (検索フォルダー)  <br/> |WellKnownFolderName.SearchFolders  <br/> |DistinguishedFolderId.searchfolders  <br/> |Outlook で表示可能な検索フォルダーが含まれます。  <br/> |
   
EWS マネージ API の [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.wellknownfoldername%28v=exchg.80%29.aspx) プロパティの値の完全な一覧については、[WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=EXCHG.80%29.aspx) 列挙体を参照してください。 EWS の **DistinguishedFolderId** 値の完全な一覧については、[DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) を参照してください。
  
### <a name="folder-properties"></a>フォルダーのプロパティ

EWS マネージ API では、[フォルダーのプロパティ](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder_properties%28v=exchg.80%29.aspx)はすべて基本 [Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) クラスから派生しています。 さらに EWS では、すべてのフォルダーは、[Folder](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) 型で使用可能なフォルダーの要素を使用します。 ほとんどのフォルダー関連のプロパティおよび要素 (親フォルダーの ID、表示名など) は単純ですが、いくつかのプロパティおよび要素については、もう少し詳しい説明が必要です。 
  
EWS マネージ API の [Folder.FolderClass](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.folderclass%28v=EXCHG.80%29.aspx) プロパティまたは EWS の [FolderClass](https://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) 要素には注意すべき次の点があります。 
  
- プロパティまたは要素の値を設定する場合、その値はフォルダーの派生クラスまたは型に一致していなければなりません。 たとえば、**FolderClass** プロパティまたは要素で、そのフォルダーが連絡先フォルダーであることを示すことはできませんが、フォルダーのクラスまたは型が、そのフォルダーが予定表フォルダーであることを示します。 
    
- **FolderClass** プロパティまたは要素を設定せずに特定の型の[フォルダーを作成](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma)したり、汎用フォルダー型でフォルダーを作成して **FolderClass** プロパティまたは要素を指定したりできます。 どちらのオプションで作成しても、同じ結果になります。 
    
- 特定の型のフォルダーを作成するか、**FolderClass** プロパティまたは要素自体を設定して、**FolderClass** 値を設定した後は、その値を変更することはできません。 たとえば、IPF.Note フォルダーを IPF.Contact フォルダーに変更することはできません。 ただし、IPF.Note.Contoso フォルダーに変更することはできます。 
    
- 定義済みのどのプレフィックスも使用していない **FolderClass** 値は、IPF.Note フォルダーとして扱われます。 たとえば、IAmAFolderClass の **FolderClass** 値は、IPF.Note フォルダーとして扱われます。 
    
フォルダー クラスの値は、拡張可能です。 つまり、表 1 に記載されている既定の **FolderClass** 値はプレフィックスとして扱われ、カスタム値を追加することができます。 たとえば、IPF.Contact.Contoso の **FolderClass** 値を使用して作成するフォルダーは、連絡先フォルダーとして扱われます。 
  
EWS マネージ API の [Folder.EffectiveRights](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.effectiverights%28v=EXCHG.80%29.aspx) プロパティまたは EWS の [EffectiveRights](https://msdn.microsoft.com/library/bf5278eb-3a1a-4d27-9d16-b8be043bb023%28Office.15%29.aspx) 要素を使用して、削除、読み取り、変更など、クライアントがフォルダーに対して持っているアクセス許可を確認できます。 
  
### <a name="public-folders"></a>パブリック フォルダー

パブリック フォルダーは、共有アクセスのために設計された、情報を収集、整理してワークグループや組織内の他のユーザーと共有するための容易かつ効果的な方法です。 パブリック フォルダーを使用して、配布グループのコンテンツをアーカイブすることもできます。 パブリック フォルダーの詳細については、「[Exchange での EWS を使用したパブリック フォルダー アクセス](public-folder-access-with-ews-in-exchange.md)」を参照してください。

<a name="bk_hiddenfolders"> </a>

### <a name="hidden-folders"></a>隠しフォルダー

Exchange がメールボックスのルートに作成するすべてのフォルダーは非表示にされます。EWS マネージ API または EWS を使用して、「インフォメーション ストアの先頭」の下にある他のフォルダーを非表示にすることもできます。 隠しフォルダーの詳細については、「[Exchange で EWS を使用して隠しフォルダーを操作する](how-to-work-with-hidden-folders-by-using-ews-in-exchange.md)」を参照してください。 

<a name="bk_hiddenfolders"> </a>

### <a name="search-folders"></a>検索フォルダー

検索フォルダーは、検索フィルターを定義するプロパティまたは要素があること以外は、通常のフォルダーと同じです。 検索フォルダーは Exchange メールボックスの任意のフォルダー内に作成できます。その方法は、他のフォルダーを作成する場合と同じです。 ただし、検索フォルダーを Outlook、Outlook Web App、Outlook Live に表示するには、EWS マネージ API を使用して作成した [SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) オブジェクトは [WellKnownFolderName.SearchFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=EXCHG.80%29.aspx) フォルダーに配置し、EWS を使用して作成した [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) 型は [DistinguishedFolderId.SearchFolders](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) フォルダーに配置する必要があります。 検索フォルダーは、別の場所に作成されていても使用可能であり、カスタム クライアント アプリケーションで表示することができます。 

<a name="bk_item"> </a>

## <a name="items"></a>アイテム

Exchange での EWS はメールボックス内の個々のメール メッセージ、予定、会議、連絡先、配布リスト、タスク、投稿、および他のアイテムを表すために、**アイテム**を使用します。 アイテムは、厳密に型指定されているか (関連付けられている特定のクラスまたはスキーマが含まれるアイテム)、厳密に型指定されていないか (汎用アイテム) のいずれかになります。 汎用アイテムは、EWS マネージ API の [Item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=EXCHG.80%29.aspx) オブジェクトおよび EWS の [Item](https://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) 型です。 メール メッセージ、連絡先、配布リスト、投稿、タスクなどの共通のアイテムは、厳密に型指定されており、スキーマ化された特定のプロパティまたは要素を設定することができます。 
  
**表 3. 厳密に型指定されたアイテム**

|**EWS マネージ API のアイテムの種類**|**EWS のアイテムの要素**|
|:-----|:-----|
|[Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |[CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |
|[Contact](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |[Contact](https://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) <br/> |
|[ContactGroup](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) <br/> |[DistributionList](https://msdn.microsoft.com/library/f65aea01-e870-44a2-8571-fa6c001341cc%28Office.15%29.aspx) <br/> |
|[EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |[Message](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) <br/> |
|[PostItem](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.postitem%28v=exchg.80%29.aspx) <br/> |[PostItem](https://msdn.microsoft.com/library/7727ed84-9591-4a1c-bb04-12129926499b%28Office.15%29.aspx) <br/> |
|[Task](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |[Task](https://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) <br/> |
   
EWS マネージ API の厳密に型指定されたアイテムは、基本 [Item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=EXCHG.80%29.aspx) クラスから派生します。 ただし、通常は、**Item** クラスを直接操作するのではなく、表 3 に記載されている派生した型のいずれかを操作します。 [ItemCollection](https://msdn.microsoft.com/library/dd634001%28v=EXCHG.80%29.aspx) クラスを操作する場合は、**Item** クラスのインスタンスを直接操作することも可能です。 その場合、**Item** クラスのインスタンスが表す、ストア内のアイテムの種類を決定するロジックを実装する必要があります。 そのアイテムを操作するには、アイテムを表すクラスのインスタンスを使用してアイテムにバインドする必要があります。 
  
### <a name="items-in-folders"></a>フォルダー内のアイテム

一部のフォルダーには、格納できるアイテムの種類について制限があります。これらは、Exchange メールボックス データベースがフォルダーに適用する制限であり、クライアント ビューの制限ではありません。  
  
**表 4. フォルダーのアイテムの制限**

|**EWS マネージ API のフォルダー クラス**|**EWS のフォルダー型**|**制限**|
|:-----|:-----|:-----|
|[基本フォルダー クラス](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) <br/> |[Folder](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) <br/> |EWS マネージ API の [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) オブジェクトと [PostItem](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.postitem%28v=exchg.80%29.aspx) オブジェクト、EWS の [Message](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) 型または **PostItem** 型は、汎用フォルダー内にのみ作成できます。 汎用フォルダーに他の種類のアイテムを移動することはできますが、それらのアイテムはクライアントでは表示されません。  <br/> |
|[CalendarFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx) <br/> |[CalendarFolder](https://msdn.microsoft.com/library/48687a78-e757-4c04-9641-bf4302c6b565%28Office.15%29.aspx) <br/> |予定表フォルダー内には、EWS マネージ API の [Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) オブジェクトおよび EWS の [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) 型のみを作成することができます。 予定表フォルダーに他の種類のアイテムを移動することはできますが、それらのアイテムはクライアントでは表示されません。  <br/> |
|[ContactsFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx) <br/> |[ContactsFolder](https://msdn.microsoft.com/library/6c299de8-2087-4aeb-8e66-2bc7586509a6%28Office.15%29.aspx) <br/> |連絡先フォルダー内には、EWS マネージ API の [Contact](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) オブジェクトと [ContactGroup](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) オブジェクト、EWS の [Contact](https://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) 型または [DistributionList](https://msdn.microsoft.com/library/f65aea01-e870-44a2-8571-fa6c001341cc%28Office.15%29.aspx) 型のみを作成できます。 連絡先フォルダーに他の種類のアイテムを移動することはできますが、それらのアイテムはクライアントでは表示されません。  <br/> |
|[SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) <br/> |[SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) <br/> |制限なし。アイテムは実際には検索フォルダー内に存在しません。これらは、メールボックス内の別の場所に存在します。  <br/> |
|[TasksFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) <br/> |[TasksFolder](https://msdn.microsoft.com/library/5a9a4612-8064-4986-b467-c44f268c64df%28Office.15%29.aspx) <br/> |タスク フォルダー内には、EWS マネージ API の [Task](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) オブジェクト、EWS の [Task](https://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) 型のみを作成できます。 タスク フォルダーに他の種類のアイテムを移動することはできますが、それらのアイテムはクライアントでは表示されません。  <br/> |

<a name="bk_upgrading"> </a>

## <a name="upgrading-from-earlier-product-versions"></a>以前の製品バージョンからのアップグレード

以前の製品バージョンと現在の製品バージョンでは、フォルダーの大部分に変更はありません。 ただし、以前のバージョンの Exchange では、メッセージング レコード管理 (MRM) を実行する場合に管理フォルダーを使用することに注意してください。 Exchange Online、Office 365 の一部としての Exchange Online、Exchange 2013 以降のバージョンの Exchange では、MRM のアイテム保持ポリシーが使用されます。 [管理フォルダーをアップグレードしてアイテム保持ポリシーを使用する](https://technet.microsoft.com/library/dd298032%28v=exchg.150%29.aspx)ことができます。 
  
以前および現在の製品バージョンで、アイテムは変更されていません。

<a name="bk_inthissection"> </a>

## <a name="in-this-section"></a>このセクションの内容

- [Exchange で EWS を使用してフォルダーを操作する](how-to-work-with-folders-by-using-ews-in-exchange.md)
    
- [Exchange で EWS を使用して隠しフォルダーを操作する](how-to-work-with-hidden-folders-by-using-ews-in-exchange.md)
    
- [Exchange で EWS を使用して Exchange メールボックス アイテムを操作する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)
    
- [Exchange で EWS を使用してアイテムを削除する](deleting-items-by-using-ews-in-exchange.md)
    
- [Exchange で EWS を使用してアイテムをエクスポートおよびインポートする](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>関連項目

- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)   
- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)   
- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md)
    

