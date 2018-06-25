---
title: Exchange  の EWS のフォルダーとアイテム
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9d8cf6fa-85a4-45ac-8165-e4d3ab92594e
description: フォルダーおよびメールボックスのアイテムと、EWS マネージ API または EWS クライアントでこれらのアイテムを表す方法について説明します。
ms.openlocfilehash: a3358844f2317c9b0462456ff7d2f38442c98ee3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758918"
---
# <a name="folders-and-items-in-ews-in-exchange"></a>Exchange  の EWS のフォルダーとアイテム

フォルダーおよびメールボックスのアイテムと、EWS マネージ API または EWS クライアントでこれらのアイテムを表す方法について説明します。
  
フォルダーは、Exchange メールボックスの構成要素です。フォルダーには、メール メッセージ、連絡先、予定、会議、タスクなどのメールボックス アイテムを含めたり、その他のフォルダーを含めたりすることができます。Exchange にはさまざまな種類のフォルダーが含まれていますが、フォルダーの種類は非常によく似ています。主な違いは、含まれているアイテムの種類です。
  
アイテムには、ただし、一意の型があります。 各項目の種類には、プロパティまたはそれを定義するスキーマの異なるセットがあります。 この記事では、フォルダーと利用可能な項目とそれらの間の相違点の種類について説明します。

<a name="bk_folders"> </a>

## <a name="folders"></a>フォルダー

すべてのフォルダーは、同じ基本クラスまたは基本型、EWS マネージ api では、[フォルダー](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=EXCHG.80%29.aspx)クラスまたは EWS での[フォルダー](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx)の種類から派生します。 次の図では、EWS のマネージ API のクラスおよび EWS 型を示します。 
  
**図 1 です。フォルダー クラスのマネージ API の EWS と EWS フォルダーの種類**

![EWS Managed API Folder クラスから派生するクラスと EWS Folder タイプから派生するタイプ (CalendarFolder、ContactsFolder、SearchFolder、および TasksFolder) が表示された図。](media/Ex2013_Folder_OverviewTypes.png)
  
各フォルダーのクラスとの種類のフォルダーとの間の主な相違点は、フォルダーの種類ごとに特定の種類の項目を作成することのみできます。 その他の違いの 1 つが、クライアントがフォルダー内の情報を表示する方法です。 たとえば、Exchange を使用すると、予定表フォルダーで予定を作成できます。 、それらを作成した後に Outlook が表示されない、予定表フォルダーに他の種類のアイテムを移動できます。 のみ、outlook では、[フォルダーに別の種類の項目が存在する場合でも](folders-and-items-in-ews-in-exchange.md#bk_item)、予定表フォルダーで予定や会議などの予定表アイテムが表示されます。 
  
**表 1 です。フォルダー クラスのマネージ API の EWS と EWS フォルダーの種類**

|**EWS マネージ API クラス**|**EWS 型**|**FolderClass 値**|**内容**|**メモ**|
|:-----|:-----|:-----|:-----|:-----|
|[Folder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) <br/> |[Folder](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) <br/> |IPF.Note  <br/> |メール メッセージまたはフォルダー。  <br/> | フォルダーの一般的なクラスまたは EWS のマネージ API の[WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx)の次のフォルダーおよび EWS [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx)フォルダーの種類です。 <ul><li>  ルート (IPM サブツリー)</li><li>NonIpmSubtree</li><li>受信トレイ</li><li>削除済みアイテム</li><li>下書き</li><li>ジャーナル</li><li>メモ  </li><li>送信トレイ</li><li>送信済みアイテム</li><li>メッセージ フォルダー</li><li>迷惑メール</li><li>ボイス メール</li></ul> |
|[CalendarFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx) <br/> |[CalendarFolder](http://msdn.microsoft.com/library/48687a78-e757-4c04-9641-bf4302c6b565%28Office.15%29.aspx) <br/> |IPF.Appointment  <br/> |予定および会議。  <br/> |ユーザーは、会議出席依頼に応答すると、予定は、EWS のマネージ API の[WellKnownFolderName.Calendar](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx)または、EWS [DistinguishedFolderId.CalendarFolder](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx)のみに追加されます。 これらは、会議出席依頼や返答を自動対話をサポートするフォルダーのみです。  <br/><br/>このクラスのフォルダーまたはフォルダーの種類の予定と会議の EWS のマネージ API の[Folder.FindItem](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=EXCHG.80%29.aspx)メソッドと、[予定表ビュー](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx)クラス、または[FindItem EWS を使用して開始日と終了日を基に取得する予定表ビューの使用をサポートしています。](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)操作および[予定表ビュー](http://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx)の要素です。  <br/> |
|[メッセージ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx) <br/> |[メッセージ](http://msdn.microsoft.com/library/6c299de8-2087-4aeb-8e66-2bc7586509a6%28Office.15%29.aspx) <br/> |IPF.Contact  <br/> |連絡先と配布リスト。  <br/> |なし。  <br/> |
|[SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) <br/> |[SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) <br/> |IPF.Note  <br/> |内容は、制限またはフィルターによって決まります。検索フォルダーにサブフォルダーは含まれていません。  <br/> |検索条件に一致するアイテムは、実際には検索フォルダーに含まれていません。そうではなく、メールボックスの他の場所にあります。  <br/> 検索フォルダーを Outlook で使用可能にするには、検索 (Finder) フォルダーに検索 (Search) フォルダーを作成します。  <br/> |
|[TasksFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) <br/> |[TasksFolder](http://msdn.microsoft.com/library/5a9a4612-8064-4986-b467-c44f268c64df%28Office.15%29.aspx) <br/> |IPF.Task  <br/> |行うべき作業アイテムが含まれています。  <br/> |なし。  <br/> |
   
### <a name="folder-structure"></a>フォルダー構造

フォルダーは、メールボックスの構造を提供します。 非 IPM サブツリーまたは EWS のルートではほとんどのユーザーに表示しない、システム フォルダーと同様に、ほとんどのユーザーは、自分のメールボックスと対話、EWS でインフォメーション ストアの最上部と呼ばれる、IPM サブツリーが含まれます。 次の図は、ユーザー用のフォルダー構造を示しています、示し、ユーザーのアイテムのあるフォルダーはシステム フォルダーです。
  
**図 2 になります。メールボックス内の項目とシステム フォルダー**

![ルート内のシステム フォルダー (インフォメーション ストア内の Favorites、Finder、FreeBusy Data、Top など) が示された図。インフォメーション ストアの Top には、Calendar、Contacts などのユーザー フォルダーがあります。](media/Ex2013_Folder_OverviewSampleHierarchy.png)
  
### <a name="well-known-folders"></a>既知のフォルダー

メールボックス内には、特殊なフォルダーもあります。これらは、EWS マネージ API の既知のフォルダーまたは EWS の識別フォルダーのことです。これらのフォルダーの一部には、フォルダー名、フォルダー構造内での場所、フォルダーを削除可能かどうかについての制限があります。他の「汎用」(特殊ではない) フォルダーには、こうした制限はありません。次の既知のフォルダーまたは識別フォルダーについて理解することは重要です。これらは、ルート システム、ユーザー、検索フォルダーであり、ほとんどの実装に適用できるからです。  
  
**表 2 になります。主識別し、既知のフォルダー**

|**フレンドリ名**|**EWS のマネージ API の**WellKnownFolderName**の値**|**EWS **DistinguishedFolderId**値**|**説明**|
|:-----|:-----|:-----|:-----|
|ルート (非 IPM サブツリー)  <br/> |WellKnownFolderName.Root  <br/> |DistinguishedFolderId.root  <br/> |非 IPM サブツリーとも呼ばれる、メールボックスのルート フォルダーが含まれます。このフォルダーには親が含まれていないため、フォルダーを移動、コピー、名前変更、削除することはできません。各メッセージ ストアには 1 つのルート フォルダーだけが含まれます。  <br/> |
|インフォメーション ストアの先頭 (IPM サブツリー)  <br/> |WellKnownFolderName.MsgFolderRoot  <br/> |DistinguishedFolderId.msgfolderroot  <br/> |受信トレイやユーザーのその他のフォルダーが含まれます。   <br/> |
|検索 (検索フォルダー)  <br/> |WellKnownFolderName.SearchFolders  <br/> |DistinguishedFolderId.searchfolders  <br/> |Outlook で表示可能な検索フォルダーが含まれます。  <br/> |
   
EWS のマネージ API の[WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.wellknownfoldername%28v=exchg.80%29.aspx)プロパティの値の一覧は、 [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=EXCHG.80%29.aspx)列挙体を参照してください。 EWS **DistinguishedFolderId**の値の一覧は、 [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx)を参照してください。
  
### <a name="folder-properties"></a>フォルダー プロパティ

EWS マネージ API では、[[フォルダーのプロパティ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder_properties%28v=exchg.80%29.aspx)はすべて、基本クラスから派生[フォルダー](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=EXCHG.80%29.aspx)です。 EWS、すべてのフォルダーが[フォルダー](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx)の種類で使用可能なフォルダーの要素を使用します。 フォルダー関連のプロパティおよび要素のほとんどは簡単です (親フォルダーの ID、表示名、およびなど) がいくつかは、少しより詳細な説明を必要とします。 
  
EWS のマネージ API の[Folder.FolderClass](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.folderclass%28v=EXCHG.80%29.aspx)プロパティまたは EWS [FolderClass](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx)要素に次の注意事項が適用されます。 
  
- 場合は、派生クラス型、またはフォルダーの設定、プロパティ、または要素の値が一致しなければなりません。 たとえば、 **FolderClass**プロパティまたは要素はフォルダーは、クラスの中に、[連絡先] フォルダーまたは予定表フォルダーのフォルダーの種類を示しますに示すことはできません。 
    
- 汎用フォルダーの種類のフォルダーを作成し、 **FolderClass**プロパティまたは要素を指定できます。 またはいずれかの[フォルダーを作成する](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma)特定の種類の**FolderClass**プロパティまたは要素を設定できます。 両方のオプションは、同じ結果を作成します。 
    
- フォルダーの特定の種類を作成することによって、または**FolderClass**プロパティまたは要素自体を設定することにより、 **FolderClass**の値を設定した後は変更できません。 などの IPF を変更することはできません。IPF にフォルダーをメモします。フォルダーにお問い合わせください。 IPF に変更することができます、ただし、します。Note.Contoso フォルダーです。 
    
- 定義済みのプレフィックスのいずれかを使用しない任意の**FolderClass**値は、IPF として扱われます。注フォルダーです。 たとえば、IAmAFolderClass の**FolderClass**の値は、IPF として扱われます。注フォルダーです。 
    
フォルダー クラス値は、拡張可能です。 つまり、表 1 に記載されているデフォルトの**FolderClass**値は、プレフィックスとして扱われます。 カスタム値を追加することができます。 たとえば、IPF の**FolderClass**値を持つフォルダーを作成することができます。Contact.Contoso、およびそれは、連絡先フォルダーとして扱われます。 
  
どのようなように、フォルダーに、クライアントが持っているアクセス許可を削除、読み取り、および、EWS のマネージ API の[Folder.EffectiveRights](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.effectiverights%28v=EXCHG.80%29.aspx)プロパティまたは EWS [EffectiveRights](http://msdn.microsoft.com/library/bf5278eb-3a1a-4d27-9d16-b8be043bb023%28Office.15%29.aspx)要素を使用して、変更を確認できます。 
  
### <a name="public-folders"></a>パブリック フォルダー

パブリック フォルダーは、共有のアクセス用に設計され、収集、整理、およびワークグループまたは組織内の他のユーザーと情報を共有する簡単で効果的な方法を提供します。 配布グループのコンテンツをアーカイブするのにパブリック フォルダーを使用することもできます。 パブリック フォルダーに関する詳細な情報は、 [EWS を使って Exchange パブリック フォルダーにアクセス](public-folder-access-with-ews-in-exchange.md)を参照してください。

<a name="bk_hiddenfolders"> </a>

### <a name="hidden-folders"></a>隠しフォルダー

Exchange がメールボックスのルートに作成するすべてのフォルダーは非表示、およびインフォメーション ストア上の [追加のフォルダーを非表示にするのには EWS のマネージ API または EWS を使用することができます。 隠しフォルダーの詳細については、 [Exchange で EWS を使用して非表示のフォルダーを操作](how-to-work-with-hidden-folders-by-using-ews-in-exchange.md)を参照してください。 

<a name="bk_hiddenfolders"> </a>

### <a name="search-folders"></a>検索フォルダー

検索フォルダーは、プロパティまたは検索フィルターを定義する要素がない限り、通常のフォルダーと同じようにします。 、Exchange メールボックス内の任意のフォルダーに検索フォルダーを作成することができ、他の任意のフォルダーを作成するのと同じ方法でそれらを作成します。 ただし、検索フォルダーの Outlook、Outlook Web App、または Outlook Live で表示するのには、EWS のマネージ API を使用して作成する[SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)オブジェクト置く必要があります[WellKnownFolderName.SearchFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx)フォルダー、および[SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx)EWS を使用して作成する型は、 [DistinguishedFolderId.SearchFolders](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx)フォルダーにある必要があります。 検索フォルダー作成する場合は別の場所にも使用可能になるし、カスタム クライアント アプリケーションで表示することができます。 

<a name="bk_item"> </a>

## <a name="items"></a>アイテム

Exchange 内では、**アイテム**を使用して、個々 の電子メール メッセージ、予定、会議、連絡先、配布リスト、タスク、投稿、およびメールボックス内の項目を表します。 項目は、いずれかの厳密に型指定、関連付けられている特定のクラスまたはスキーマ、または厳密に型指定されない場合とも呼ばれる汎用的なアイテムであることを意味します。 汎用アイテムは、EWS の EWS のマネージ API と[アイテム](http://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx)の種類の[項目](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx)のオブジェクトです。 電子メール メッセージ、連絡先、配布リスト、投稿などの共通の項目とタスクは、厳密に型指定にスキーマの特定のプロパティまたは要素を設定することができます。 
  
**表 3。厳密に型指定された項目**

|**EWS のマネージ API の項目の種類**|**EWS 項目要素**|
|:-----|:-----|
|[Appointment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |[カレンダー項目](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |
|[Contact](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |[Contact](http://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) <br/> |
|[ContactGroup](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) <br/> |[DistributionList](http://msdn.microsoft.com/library/f65aea01-e870-44a2-8571-fa6c001341cc%28Office.15%29.aspx) <br/> |
|[なか](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |[Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) <br/> |
|[PostItem](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.postitem%28v=exchg.80%29.aspx) <br/> |[PostItem](http://msdn.microsoft.com/library/7727ed84-9591-4a1c-bb04-12129926499b%28Office.15%29.aspx) <br/> |
|[Task](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |[タスク](http://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) <br/> |
   
EWS のマネージ API を厳密にする項目[の項目](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=EXCHG.80%29.aspx)の基本クラスから派生します。 ただし、通常直接操作する表 3 に記載されている派生型のいずれかと**アイテム**のクラスではなく。 [ItemCollection](http://msdn.microsoft.com/en-us/library/dd634001%28v=EXCHG.80%29.aspx)クラスを使用するときに、**項目**のクラスのインスタンスを直接使用する可能性があります。 その場合は、**項目**のクラスのインスタンスを表すストア内のアイテムの種類を決定するロジックを実装する必要があります。 そのアイテムを操作するには、アイテムを表すクラスのインスタンスを使用して項目に連結する必要があります。 
  
### <a name="items-in-folders"></a>フォルダー内のアイテム

一部のフォルダーには、格納できるアイテムの種類について制限があります。これらは、Exchange メールボックス データベースがフォルダーに適用する制限であり、クライアント ビューの制限ではありません。  
  
**表 4 です。フォルダーのアイテムの制限**

|**EWS で API フォルダー管理クラス**|**EWS のフォルダーの種類**|**Restriction**|
|:-----|:-----|:-----|
|[フォルダーの基本クラス](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) <br/> |[Folder](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) <br/> |EWS のマネージ API の[なか](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx)の新しいオブジェクトと[PostItem](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.postitem%28v=exchg.80%29.aspx)オブジェクトでは、EWS の[メッセージ](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx)の種類または**PostItem**の種類は、一般的なフォルダーの中にのみ作成できます。 汎用フォルダーは、他の項目の種類に移動することができますが、クライアントは表示されませんがあります。  <br/> |
|[CalendarFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx) <br/> |[CalendarFolder](http://msdn.microsoft.com/library/48687a78-e757-4c04-9641-bf4302c6b565%28Office.15%29.aspx) <br/> |EWS のマネージ API の[予定](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx)の新しいオブジェクトおよび EWS[カレンダー項目](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx)の種類は、予定表フォルダーでのみ作成できます。 予定表] フォルダーにその他の項目の種類を移動することができますが、クライアントは表示されませんがあります。  <br/> |
|[メッセージ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx) <br/> |[メッセージ](http://msdn.microsoft.com/library/6c299de8-2087-4aeb-8e66-2bc7586509a6%28Office.15%29.aspx) <br/> |新しい EWS のマネージ API の[連絡先](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx)オブジェクトと[ContactGroup](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx)オブジェクト、または EWS[連絡先](http://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx)型または[DistributionList](http://msdn.microsoft.com/library/f65aea01-e870-44a2-8571-fa6c001341cc%28Office.15%29.aspx)型は、連絡先フォルダーでのみ作成できます。 連絡先フォルダーにその他の項目の種類を移動することができますが、クライアントに表示されません。  <br/> |
|[SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) <br/> |[SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) <br/> |制限はありません。アイテムは実際には検索フォルダー内に存在しません。これらは、メールボックス内の別の場所に存在します。  <br/> |
|[TasksFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) <br/> |[TasksFolder](http://msdn.microsoft.com/library/5a9a4612-8064-4986-b467-c44f268c64df%28Office.15%29.aspx) <br/> |新しい EWS マネージ API[タスク](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx)オブジェクトまたは EWS の[タスク](http://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx)の種類は、[仕事] フォルダーでのみ作成できます。 タスク] フォルダーにその他の項目の種類を移動することができますが、クライアントに表示されません。  <br/> |

<a name="bk_upgrading"> </a>

## <a name="upgrading-from-earlier-product-versions"></a>以前の製品バージョンからのアップグレード

フォルダーの大部分は以前のバージョンおよび現在の製品バージョンで変更されていないままであります。 ただし、Exchange の以前のバージョンでの管理フォルダーを使用して、メッセージング レコード管理 (MRM) を実行することに注意してください。 Exchange のオンライン、Exchange オンライン Office 365 の一部のバージョンの Exchange が Exchange 2013 で始まるとは、MRM のリテンション ・ ポリシーを使用します。 [アップグレード ・ リテンション ・ ポリシーを使用するフォルダーを管理する](http://technet.microsoft.com/en-us/library/dd298032%28v=exchg.150%29.aspx)ことができます。 
  
以前および現在の製品バージョンで、アイテムは変更されていません。

<a name="bk_inthissection"> </a>

## <a name="in-this-section"></a>このセクションの内容

- [Exchange EWS を使用してフォルダーを操作します。](how-to-work-with-folders-by-using-ews-in-exchange.md)
    
- [Exchange EWS を使用して非表示のフォルダーの操作します。](how-to-work-with-hidden-folders-by-using-ews-in-exchange.md)
    
- [EWS を使用して Exchange で Exchange メールボックスのアイテムを扱う](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)
    
- [Exchange EWS を使用して項目を削除します。](deleting-items-by-using-ews-in-exchange.md)
    
- [エクスポートし、Exchange の EWS を使用してアイテムをインポート](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>関連項目

- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)   
- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)   
- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md)
    

