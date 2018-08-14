---
title: Exchange での代理人アクセスと EWS
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 240d1776-7adc-46cd-9099-88ffeba0a8aa
description: Exchange の EWS マネージ API と EWS を使用してユーザーのメールボックスに代理人アクセスできるようにする方法を説明します。
ms.openlocfilehash: 344255d86a51e13b21f1eda5113d292395d7cb8f
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354051"
---
# <a name="delegate-access-and-ews-in-exchange"></a>Exchange での代理人アクセスと EWS

Exchange の EWS マネージ API と EWS を使用してユーザーのメールボックスに代理人アクセスできるようにする方法を説明します。
  
ユーザーが他のユーザーのメールボックスにアクセスできるようにするには、次の 3 つの方法のいずれかを使用できます。 
  
- 代理人を追加し、各代理人にアクセス許可を指定します。
    
- フォルダーのアクセス許可を直接変更します。
    
- 偽装を使用します。
    
委任、およびフォルダーのアクセス許可は、各メールボックスに個別にアクセス許可を追加する必要があるため、少数のユーザーにのみアクセス許可を付与する場合に最適です。偽装は、1 つのサービス アカウントによるデータベース内のすべてのメールボックスへのアクセスを簡単に許可できるため、多数のメールボックスを処理するときに最適です。図 1 は、各種のアクセスの相違点を示しています。
  
**図 1. 他のユーザーのメールボックスにアクセスする方法**

![メールボックスのアクセス タイプ、各タイプのメールボックス所有者と代理人の関係、およびアクセス許可のタイプを示す図。委任用のアクセス許可またはフォルダー アクセス許可のために送信します。偽装のためのアクセス許可として送信します。](media/Ex15_Delegate_Overview.png)
  
メールの送信や会議のスケジュールに関して、代理人には「代理送信」のアクセス許可が与えられます。そのため、代理人から送信されたメールまたは会議出席依頼の受信者がそれを Outlook で受信した場合、「*メールボックスの所有者*の*代理人として送信*」したことが表示されます。 「代理人として送信」のテキストを含めることは、クライアント実装の詳細事項の 1 つです。これは "from" と "sender" の値を使用して作成できます。 "from" の値はメールボックスの所有者を示し、"sender" の値はメール送信した代理人を示します。 ユーザーを偽装しているサービス アカウントが、メールボックスの所有者の代わりにメールの送信や会議のスケジュールを行う場合、メッセージはメールボックスの所有者「として」送信されます。 受信者には、サービス アカウントから送信されたメールであることを確認する手段はありません。 フォルダーのアクセス許可が付与され、代理人としてのアクセス権が付与されていないユーザーは、メールボックスの所有者として送信したり、代理送信したりできません。 そのようなユーザーはメールボックスのフォルダーへのアクセス権を持ち、フォルダーにアイテムを作成できる場合もありますが、アイテムを送信することはできません。 
  
フォルダーのアクセス許可を直接変更するのが適しているのはどのような場合でしょうか。 一般に、フォルダーへのアクセスをユーザーに提供するものの「代理送信」のアクセス許可は付与しない場合、アクセス許可の要件が [DelegateFolderPermissionLevel](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.delegatefolderpermissionlevel%28v=exchg.80%29.aspx) EWS マネージ API 列挙値または [PermissionLevel](http://msdn.microsoft.com/library/87978600-3523-451e-a725-ef092c543e2a%28Office.15%29.aspx) EWS の要素の値にマップしない場合、または単一のカスタム フォルダーへのアクセスをユーザーに提供する場合です。 
  
フォルダーのアクセス許可を変更するだけで目標を達成でき、代理人を追加する必要がない場合 (つまり、「代理送信」のアクセス許可が必要ない場合) は、[「Exchange で EWS を使用して別のユーザーのフォルダーのアクセス許可を設定する」](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)を参照してください。 
  
なお、[Outlook](http://office.microsoft.com/ja-JP/outlook-help/allow-someone-else-to-manage-your-mail-and-calendar-HA102749417.aspx) または [Exchange Server PowerShell (Exchange 管理シェル)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps) を使用して代理人アクセスを設定することもできます。 
  
## <a name="how-does-delegate-access-work"></a>代理人アクセスはどのように機能するか

代理人アクセスにより、ユーザーはメールボックス所有者のフォルダーの一部または全部にアクセスし、メールボックス所有者の代理として行動できるようになります。 メールボックスの所有者はユーザーの場合もあれば、会議室のようなリソースの場合もあります。 たとえば、予約要求を処理するため、受付係に会議室の予定表フォルダーへの代理アクセス権を付与できます。 EWS マネージ API または EWS を使用すれば、メールボックスの所有者または管理者は、代理人を追加すること、代理人がアクセスできるフォルダーを指定すること、そのフォルダーに対するアクセス許可を指定することができるようになります。 代理人には、次のフォルダーへのアクセス権を与えることができます。 
  
- 予定表
    
- タスク
    
- 受信トレイ
    
- 連絡先
    
- メモ
    
- ジャーナル
    
これらのフォルダーの 1 つ以上に対する代理人アクセスを持つユーザーは、フォルダーに設定されている[アクセス許可](#bk_delegateperms)に応じて、そのフォルダーおよび子フォルダー内のアイテムの作成、取得、更新、削除、コピー、検索ができます。アプリケーションがこれらのアクションを実行する方法は、[明示的な](#bk_explicit)アクセスと[暗黙的な](#bk_implicit)アクセスのどちらが必要かに応じて異なります。 
  
## <a name="delegate-permissions"></a>代理アクセス権
<a name="bk_delegateperms"> </a>

管理者またはメールボックスの所有者がメールボックスに代理人を追加するときは、1 つ以上のフォルダーのアクセス許可レベルを設定することもできます。 フォルダーのアクセス許可レベルが設定されていない場合、アクセス許可の値の既定値は、[なし] に設定されます。 あるフォルダーに対して複数のユーザーが同じアクセス許可レベルを持つことも、ユーザーが持つアクセス許可レベルをフォルダーごとに変えることもできます。 EWS マネージ API を使用する場合は、[DelegateUser.Permissions](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.delegateuser.permissions%28v=exchg.80%29.aspx) プロパティ (各フォルダーの [DelegateFolderPermissionLevel](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.delegatefolderpermissionlevel%28v=exchg.80%29.aspx) 列挙値の 1 つを指定する) を使用して、フォルダーに対する代理アクセス権を設定します。 EWS を使用する場合は、[DelegatePermissions](http://msdn.microsoft.com/library/292badc7-bab3-4368-9d7c-9a8b7edb279b%28Office.15%29.aspx) 要素を使用して代理アクセス権を設定し、[PermissionLevel](http://msdn.microsoft.com/library/87978600-3523-451e-a725-ef092c543e2a%28Office.15%29.aspx) 要素を使用してアクセス許可レベルを定義します。 
  
**表 2. 代理アクセス権レベル**

|**アクセス許可レベル**|**説明**|
|:-----|:-----|
|なし  <br/> |これはすべてのフォルダーの既定値です。  <br/> |
|Author  <br/> |代理人は、アイテムの読み取りと作成、自分が作成したアイテムの変更と削除ができます。 たとえば、代理人はタスクの依頼や会議出席依頼をメールボックスの所有者のタスクのフォルダーまたは予定表のフォルダーに直接作成して、メールボックスの所有者の代わりにいずれかのアイテムを送信できます。  <br/> |
|Editor (編集者)  <br/> |代理人は、Author にできるすべてのことに加え、メールボックスの所有者が作成したアイテムの変更や削除もできます。  <br/> |
|Reviewer  <br/> |代理人はアイテムを読むことができます。たとえば、Reviewer のアクセス許可を持つ代理人は、別のユーザーの受信トレイのメッセージを読むことができます。  <br/> |
|Custom  <br/> |メールボックスの所有者が代理人にアクセス許可のカスタム セットを与えている場合です。  <br/> |
   
[DelegateUser.ViewPrivateItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.delegateuser.viewprivateitems%28v=exchg.80%29.aspx) EWS マネージ API プロパティと [ViewPrivateItems](http://msdn.microsoft.com/library/80b949ac-440c-4a01-b428-ebafb5b1b802%28Office.15%29.aspx) EWS 要素は、メール、連絡先、予定表、タスク、メモ、ジャーナルのすべてのフォルダーを含む、メールボックス所有者のすべてのフォルダーに影響を与えるグローバルな設定です。 1 つのフォルダーだけを選んで、その中の非公開アイテムへのアクセスを許可することはできません。 
  
## <a name="explicit-access"></a>明示的なアクセス
<a name="bk_explicit"> </a>

簡単に言えば、明示的なアクセスとは、代理人がメールボックス所有者のフォルダーまたはアイテムに対してアクションを実行するための通路のようなものです。代理人がサーバーへの要求にメールボックスの所有者のフォルダーの既知のフォルダー名とメールボックスの所有者の SMTP アドレスを含めると、代理人に明示的なアクセスが与えられます。このアクセスは明示的です。なぜなら、代理人の要求は、メソッドまたは操作のコンテキストがメールボックス所有者のメールボックスであって、代理人のメールボックスではないことを、明示的に示しているためです。
  
明示的なアクセスは、この先、フォルダーやアイテムで実行されるすべてのメソッドや操作のためにコンテキストを定義します。明示的なアクセスが設定されている場合に返されるすべてのアイテムとフォルダーの ID は、自らをメールボックスの所有者に属するものとして一意に識別します (ただし人間が読める形式ではありません)。こうして、アプリケーションはメールボックスの所有者の SMTP アドレスを繰り返し指定する必要がなくなります。コンテキストは識別子の中に隠されます。アイテムまたはフォルダーが識別された後、代理人はアイテムを変更するために、実際には[暗黙的なアクセス](#bk_implicit)を使用します。次の図に、明示的なアクセスと暗黙的なアクセスを行うプロセスを示します。 
  
**図 2. アイテムまたはフォルダーへの明示的および暗黙的なアクセスの要求**

![アプリケーションが明示的なアクセスの要求を送信し、サーバーからの応答を受け取り、暗黙的なアクセスの要求を送信し、サーバーからの応答を受け取る流れを示した図。](media/Ex15_Delegate_ExplictImplicit.png)
  
様々なシナリオで明示的なアクセスを設定できます。基本的に、フォルダー ID をメソッドまたは操作に入れて送信する場合は常に、明示的なアクセスを設定できます。これには、フォルダーの検索、予定の検索、アイテムの取得、会話の検索などがあります。
  
### <a name="explicit-access-and-the-ews-managed-api"></a>明示的なアクセスと EWS マネージ API
<a name="bk_explicitewsma"> </a>

[FolderId](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) 入力パラメーターでターゲット フォルダーを指定する次のオーバーロードされたメソッドのいずれかを使用すれば、明示的な代理人アクセスを開始できます。 
  
- [Folder.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx)
    
- [ExchangeService.FindItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [ExchangeService.FindAppointments](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx)
    
- [ExchangeService.FindFolders](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- その他多数。
    
これらの各メソッドで **FolderId** パラメーターを使用して、次のようにメールボックス所有者のターゲット フォルダーを指定できます。 
  
```cs
new FolderId(WellKnownFolderName.Calendar, "primary@contoso.com");
```

たとえば、予定表フォルダーにバインドするには、次の **Bind** メソッドの **FolderId** で既知のフォルダー名とメールボックス所有者の SMTP アドレスを指定します。 
  
```cs
CalendarFolder calendar = CalendarFolder.Bind(service, new FolderId(WellKnownFolderName.Calendar, "primary@contoso.com"), new PropertySet());
```

既知のフォルダー名と SMTP アドレスを指定すると、代理人はメールボックス所有者の予定表フォルダーにバインドできるため、フォルダーへの明示的なアクセスを取得できます。これ以降、フォルダー内のアイテムに対する[暗黙的なアクセス](#bk_implicit)のすべての要求では、アイテム ID とフォルダー ID で返されるコンテキストを利用します。基本的に、識別子には暗黙的な代理人アクセスの呼び出しのコンテキストが含まれています。または、特定の条件を満たすアイテムのアイテム ID を取得するには、以下を使用します。 
  
```cs
FindItemsResults<Item> results = service.FindItems(new FolderId(WellKnownFolderName.Calendar, "primary@contoso.com"), filter, view);
```

この場合、アイテム ID が返された後、このアイテム ID を使用すれば、代理人は暗黙的なアクセスでアイテムを変更できます。
  
既存の明示的なアクセスでアクセスしていないアイテム ID またはフォルダー ID が必要になるまで、明示的なアクセスをもう一度開始する必要はありません。 
  
### <a name="explicit-access-and-ews"></a>明示的なアクセスと EWS
<a name="bk_explicitewsma"> </a>

[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)、[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)、または [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) 操作を使用して、明示的なアクセスを開始できます。これらの操作は、[DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) 要素を使用して対象フォルダーを指定するオプションを提供します。**DistinguishedFolderId** 要素には省略可能な子要素が 1 つだけあります。すなわち、[Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素です。**Mailbox** 要素は、**DistinguishedFolderId** 要素の子として使用する場合、代理人がアクセスするメールボックスを指定します。呼び出し元のユーザーにメールボックス所有者のフォルダーにアクセスする権限がある場合、応答にはそのメールボックス内のアイテムまたはフォルダーの識別子のコレクションが含まれます。応答で返されるアイテムおよびフォルダーの識別子を暗黙的な代理人アクセスで使用できます。  
  
## <a name="implicit-access"></a>暗黙的なアクセス
<a name="bk_implicit"> </a>

代理人がメールボックスの所有者のメールボックス内のアイテムまたはフォルダーの ID を取得したら、アイテムの更新、削除、またはコピーを行うとき、後は暗黙的なアクセスが使用されます。代理人が要求でそのアイテム ID またはフォルダー ID を使用すると、メールボックス所有者のメールボックス内のアイテムに対して変更が加えられます。代理人はメールボックス所有者の SMTP アドレスを含める必要はありません。  
  
たとえば、代理人がメールボックス所有者のいずれかのフォルダーの ID を持っている場合、フォルダー ID を使用すれば、そのフォルダーに対して **FindItem** 操作を実行でき、メールボックス所有者のメールボックスを明示的に指定する必要はありません。その時点で、代理人は応答で返される ID を使用して、メールボックス所有者のフォルダーにアクションを実行できます。 
  
### <a name="implicit-access-and-the-ews-managed-api"></a>暗黙的なアクセスと EWS マネージ API

[FindItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) メソッドでアイテム ID を取得したら、後続の [Item.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) メソッドの呼び出しでそのアイテム ID を使用し、アイテムにバインドできます。 次いで、タスクを完了するために必要な [Item.Update](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx)、[Item.Delete](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)、[Item.Copy](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) メソッド (あるいは、アイテム ID を必要とする任意のメソッド呼び出し) を呼び出すことができます。 アイテムを含むフォルダー (および該当する場合は、アイテムの移動先のフォルダー) の適切なアクセス許可を持っているなら、代理人はアクセス許可レベルに応じて変更を実行できます。 
  
### <a name="implicit-access-and-ews"></a>暗黙的なアクセスと EWS

[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 操作でアイテム ID を取得したら、後続の [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) 操作でそのアイテム ID を使用して、アイテムにバインドできます。次いで、タスクを完了するために必要な [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)、[DeleteItem](../web-service-reference/deleteitem-operation.md)、[CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) 操作 (あるいはアイテム ID を必要とする任意の操作) を呼び出すことができます。アイテムを含むフォルダー (および該当する場合は、アイテムの移動先のフォルダー) の適切なアクセス許可を持っているなら、代理人はアクセス許可レベルに応じて変更を実行できます。 
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_implicit"> </a>

- [Exchange で EWS を使用して代理人を追加および削除する](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
    
- [Exchange で EWS を使用して予定表に代理人としてアクセスする](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Exchange で EWS を使用して、代理人として連絡先にアクセスする](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Exchange で EWS を使用して、代理人としてメールにアクセスする](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Exchange で EWS を使用して別のユーザーのフォルダーのアクセス許可を設定する](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)
    
- [Exchange の EWS での委任に関連するエラーの処理](handling-delegation-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>関連項目


- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    
- [自分のメールと予定表の管理を他のユーザーに許可する](http://office.microsoft.com/ja-JP/outlook-help/allow-someone-else-to-manage-your-mail-and-calendar-HA102749417.aspx)
    
- [Add- MailboxPermission](http://technet.microsoft.com/ja-JP/library/bb124097%28v=exchg.150%29.aspx)
    

