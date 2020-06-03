---
title: Exchange の EWS 識別子
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 39b6b20b-e081-4347-9e15-9b8cf829fdf0
description: Exchange での識別子、およびそれらを EWS マネージ API と EWS アプリケーションで使用する方法について説明します。
localization_priority: Priority
ms.openlocfilehash: 9fa2e31a3c67b0b4291b1e3f32a775655e2bf80a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528427"
---
# <a name="ews-identifiers-in-exchange"></a>Exchange の EWS 識別子

Exchange での識別子、およびそれらを EWS マネージ API と EWS アプリケーションで使用する方法について説明します。
  
Exchange ストア内のすべてのオブジェクトには、一意の識別子があります。 オブジェクトの識別子を使用して、そのオブジェクトを参照し、他のオブジェクトと区別できます。 使用頻度の最も高い 2 つの識別子は、フォルダーとアイテムの識別子です。 
  
識別子と、識別子がアプリケーションにとってどのように重要なのかを理解するために、Exchange のオブジェクト間の関係を理解しておくようお勧めします。 EWS マネージ API または EWS アプリケーションが Exchange と通信するときには、メールボックス、フォルダー、アイテムのオブジェクトを含むオブジェクトの階層を操作します。 ストアは、これらのオブジェクトの種類のいずれにでもすることができます。 通常、ストアは Exchange サーバー上のメールボックスです。しかし、ストアを Exchange サーバーのパブリック フォルダーとすることもできます。 (Exchange Online、Office 365 に含まれる Exchange Online、および Exchange 2013 以降のバージョンの Exchange では、パブリック フォルダーはメールボックスの一種にすぎず、異なる種類のストアではないことに注意してください。) 次の図に示されるように、フォルダーはストアに格納され、アイテムはフォルダーに格納されます。それぞれのフォルダーやアイテムには識別子があります。 
  
**図 1. メールボックス、フォルダー、アイテムの階層構造**

![メールボックス オブジェクトの階層を示す図。メールボックスが最上位レベルにあり、[受信トレイ] フォルダーが次のレベルにあります。図には、電子メールを格納したフォルダーが表示されています。識別子および変更キーが各オブジェクトに対してリストされており、短縮されています。](media/Ex15_Identifier_diagram.png)
  
## <a name="ews-identifiers"></a>EWS 識別子
<a name="bk_CommonIdentifiers"> </a>

EWS がフォルダーおよびアイテム用に使用する識別子を EWS 識別子、または EwsId と呼びます。 EwsId は、EWS 内部の多くの異なるオブジェクト内にありますが、オブジェクトが異なると呼び方も異なります。 アプリケーションでこれらのオブジェクトを使用する可能性があるため、EwsId とオブジェクトの識別子の関係がどのようなものか理解する必要があります。 
  
さらに、EWS の識別子は、EWS マネージ API にも適用できます。EWS マネージ API では、識別子はオブジェクトのプロパティであり、EWS 要素にマッピングされるよう内部で管理されます。
  
**表 1. EWS のオブジェクト識別子**

|**オブジェクト**|**識別子**|**EwsId との関係**|
|:-----|:-----|:-----|
|[CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |子要素 [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) に予定表アイテムの一意の識別子が含まれています。  <br/> |子要素 [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) は、このアイテムの EwsId と同じです。  <br/> |
|[ConversationId](https://msdn.microsoft.com/library/d5f1ddb3-9af3-4677-a6ba-111b304a951e%28Office.15%29.aspx) <br/> |**Id** 属性に、このアイテムが含まれるスレッドの識別子が含まれています。  <br/> |**Id** 属性は、このアイテムの EwsId と同じです。  <br/> |
|[AttachmentId](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) <br/> |添付物の一意の識別子を提供します。[RootItemId](https://msdn.microsoft.com/library/f613c705-17ce-48ce-aa64-4dc2cea25e31%28Office.15%29.aspx) 属性には、添付物の添付先ルート ストア アイテムの一意の識別子が含まれています。  <br/> |添付物は、Exchange ストア内の他のアイテムにもできます。その場合、[AttachmentId](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) は EwsId と同じです。どの場合も、[RootItemId](https://msdn.microsoft.com/library/f613c705-17ce-48ce-aa64-4dc2cea25e31%28Office.15%29.aspx) は、ストアのアイテムを参照しているため、EwsId です。<br/> |
|[PersonaId](https://msdn.microsoft.com/library/eec3a468-afd5-4d72-a61e-cd1964fb686c%28Office.15%29.aspx) <br/> |**Id** 属性は、ペルソナの識別子を含む文字列を返します。  <br/> |**Id** 属性は、ペルソナの EwsId と同じです。  <br/> |
|[ContactId](https://msdn.microsoft.com/library/86f66275-1e39-48ed-bd89-ac3bffc465a7%28Office.15%29.aspx) <br/> |**Id** 属性は、連絡先の識別子を含む文字列を返します。  <br/> |**Id** 属性は、連絡先の EwsId と同じです。  <br/> |
|[GroupId](https://msdn.microsoft.com/library/656d9b9a-8a65-4a75-8466-5b0d96512dab%28Office.15%29.aspx) <br/> |**Id** 属性は、グループの識別子を含む文字列を返します。  <br/> |**Id** 属性は、グループの EwsId と同じです。  <br/> |
|[AssociatedCalendarItemId](https://msdn.microsoft.com/library/5b29898c-ea59-4e6a-914c-c011ec754032%28Office.15%29.aspx) <br/> |**Id** 属性は、[MeetingMessage](https://msdn.microsoft.com/library/c95956a8-7505-44b4-bea4-11d1f5182796%28Office.15%29.aspx)、[MeetingRequest](https://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx)、[MeetingResponse](https://msdn.microsoft.com/library/9f798e79-dafd-4d4d-9967-95fd8e5c0502%28Office.15%29.aspx)、または [MeetingCancellation](https://msdn.microsoft.com/library/a9c61f7f-2ecd-4b21-9dce-24d9f61aeeea%28Office.15%29.aspx) に関連付けられている予定表アイテムを識別します。  <br/> |**Id** 属性は、予定表アイテムの EwsId と同じです。  <br/> |
|[UserConfigurationProperties](https://msdn.microsoft.com/library/c143a6ec-62ad-4d48-b844-b1ad88054bc1%28Office.15%29.aspx) <br/> |この要素の **Id** 値は、識別子プロパティを指定します。  <br/> |この識別子は、プロパティの識別子であってアイテムではないため、直接には EwsId にマッピングされません。  <br/> |
|[OccurrenceItemId](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) <br/> |**RecurringMasterId** 属性は、定期的なアイテムのマスターを識別します。  <br/> |**OccurrenceItemId** 値は、直接には EwsId にマッピングされません。しかし、**RecurringMasterId** は、定期的なアイテムの最上位レベルのオブジェクトを参照しているため、直接に EwsId にマッピングされます。  <br/> |
|[StoreEntryId](https://msdn.microsoft.com/library/f536e264-8c4d-4cc5-bab8-22a4fa38de39%28Office.15%29.aspx) <br/> |アイテムの Exchange ストア識別子が含まれています。  <br/> |**StoreEntryId** 値は EwsId にはマッピングされませんが、アイテムが保存されているストアの識別子を指定します。  <br/> |
   
## <a name="working-with-identifiers"></a>識別子の処理
<a name="bk_WorkingWithIdentifiers"> </a>

Exchange サーバーは、さまざまな方法で識別子を処理します。EWS マネージ API または EWS アプリケーションを開発する場合、以下をご考慮ください。
  
- フォルダーとアイテムの **ItemID** 要素の値は、大文字小文字を区別します。 [FindItem 操作](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) (または EWS マネージ API の[FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) メソッド) によって返されるフォルダーまたはアイテムのアイテム IDは、別のアイテム ID と重複しているように見えるかもしれませんが、2 つのアイテムのアイテム ID を比べると、大文字と小文字の違いがある文字があるあずです。 
    
- 後で取得するためにアイテム ID をデータベースに格納する場合、GUID を保持するのに十分な大きさを確保するために、フィールド サイズを 512 バイトにすることをお勧めします。
    
- 後でアイテムを取得する必要がある場合は、アイテム ID が常に有効であるとは限りません。 ストア内でアイテムが移動されると、移動の処理方法によっては、ID が変更される可能性があります。 アイテムの複製が実行され、新たな ID が生成されると、[元のアイテムは削除されます](deleting-items-by-using-ews-in-exchange.md)。 フォルダー Id は変更できないため、ストアに移動しても変更されないことに注意してください。
    
- Exchange の識別子は、符号化されています。たとえば、開発者にとっては重要ではないものの、Exchange にとって重要ないくつかの情報から EwsId が作成されます。
    
- Exchange のアイテムを操作する時に留意して操作する必要がある値の 中に、**ChangeKey** 属性があります。 この値は、アイテム ID としてだけではなく、アイテムの状態を追跡するためにも使用されます。 アイテムが変更されるたびに、新しい変更キーが生成されます。 たとえば、[UpdateItem 操作](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)を実行するときに、**ChangeKey** 属性を使用して、アイテムの最新バージョンに更新を適用することをサーバーに認識させることができます。 更新中のアイテムを別のアプリケーションが変更していた場合、変更キーが一致しな くなるため、更新を実行できなくなります。 
    
## <a name="distinguished-folder-ids"></a>識別フォルダー ID
<a name="bk_DistinguishedFolderIds"> </a>

Exchange には、定義済みのメールボックス フォルダーが多数含まれています。各フォルダーには、識別フォルダー ID と呼ばれる識別子が割り当てられています。 これらは EWS マネージ API の [WellKnownFolderName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) 列挙体と EWS の [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) 要素によって定義されます。 これらの識別フォルダー ID を使用すれば、特定の定義済みフォルダーを参照するのが簡単になります。 たとえば、受信トレイ フォルダーでは、識別子にフォルダー識別子を判別しないで、単に "受信トレイ" を使用できます。 
  
メール アイテムを整理するために作成する他のフォルダーにも、そのフォルダーに対して一意な ID が付けられます。その ID は、フォルダーの他のプロパティを変更しても、変更されることはありません。
  
識別フォルダー ID は、代理人アクセスのエントリ ポイントとして使用できます。代理人アクセスを開始すると、アイテムやフォルダーを検索し、識別フォルダー ID を使用して、検索する場所を指定します。代理人ユーザーがサーバーにアクセスすると、**DistinguishedFolderId** 要素の子である [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素が、代理人がアクセスするメールボックスを明示的に指定するために使用されます。 
  
## <a name="handling-errors"></a>エラーの処理
<a name="bk_DealingWithErrors"> </a>

どのプログラムにもときおりエラーが発生しますが、EWS ベースのアプリケーションも例外ではありません。 EWS の [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素で、または EWS マネージ API の [ServiceError](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) 列挙体の一部分として、識別子に関連するエラーが発生することがあります。 
  
以下は、EWS マネージ API または EWS アプリケーションで発生する可能性のあるエラーです。 EWS マネージ API アプリケーションを操作している際に発生するエラーは、通常はプロパティ値の問題です。EWS アプリケーションでは、エラーは XML 要素値または操作と関連しています。
  
**表 2. 識別子に関連するエラー**

|**エラー**|**発生条件**|**説明**|
|:-----|:-----|:-----|
|ErrorCalendarCannotUseIdForOccurrenceId  <br/> |**OccurenceID** の値が、有効な定期的な予定表アイテムと一致しないとき。  <br/> |要求で指定された **OccurenceId** の値は、正しい構造である可能性がありますが、その値は既存の定期的なマスターと一致しませんでした。定期的なアイテムが予定表から削除された可能性があります。アイテムがまだ存在していることと、正しい識別子を使用していることを確認します。  <br/> |
|ErrorCalendarCannotUseIdForRecurringMasterId  <br/> |**RecurringMasterId** 属性が、**OccurrenceId** 要素の有効な発生と一致しないとき。  <br/> |要求で指定された **RecurringMasterId** の値は、正しい構造である可能性がありますが、その値は既存のアイテムと一致しませんでした。アイテムが予定表から削除された可能性があります。アイテムがまだ存在していることと、正しい識別子を使用していることを確認します。  <br/> |
|ErrorCannotUseFolderIdForItemId  <br/> |渡された **ID** が、アイテムではなくフォルダーを表しているとき。  <br/> |識別子の形式は正しい可能性がありますが、サーバーが操作しようとしていたものとは異なります。操作する正しい識別子を参照していることをご確認ください。  <br/> |
|ErrorCannotUseItemIdForFolderId  <br/> |渡された **ID** が、フォルダーではなくアイテムを表しているとき。  <br/> |識別子の形式は正しい可能性がありますが、サーバーが操作しようとしていたものとは異なります。操作する正しい **ID** を参照していることを確認します。<br/> |
|ErrorChangeKeyRequiredForWriteOperations  <br/> |特定の更新操作を実行する際に、有効な変更キーを指定する必要があります。  <br/> |更新を要求したときに **ChangeKey** 値を省略したか、変更キーが正しくなかったかのいずれかです。更新操作を実行する場合には、変更キーが正しいことを確認します。  <br/> |
|ErrorInvalidAttachmentId  <br/> |添付物が、アイテムの添付ファイル コレクション内で見つからないとき。  <br/> |削除された添付物の添付ファイル **ID** に対して [GetAttachment 操作](https://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx)を呼び出すと、この応答コードが返される可能性があります。 添付ファイルが添付ファイル コレクションにあることをご確認ください。  <br/> |
|ErrorInvalidChangeKey  <br/> |使用できない変更キーが渡されました。  <br/> |変更キーを渡す必要がある操作とメソッドは多くないことにご注意ください。しかし、変更キーを指定する場合、それは必ずしも最新である必要はありませんが、正しくなければなりません。  <br/> |
|ErrorInvalidFolderId  <br/> |フォルダー **ID** が破損しているとき。  <br/> |適切な形式の、正しい識別子があることを確認します。  <br/> |
|ErrorInvalidId  <br/> |**ID** の構造または変更キーで、内部の整合性に問題があるとき。  <br/> |Exchange は解析後の **ID** で問題を検出しました。変換中にエラーが発生した可能性があります。たとえば、Outlook のアイテムの **IdFormatType.HexEntryId** があり、それを **IdFormatType.EntryId** 形式と判断して、EwsId に変換した場合に、これが発生する可能性があります。適切な種類の変換をご使用ください。<br/> |
|ErrorInvalidIdEmpty  <br/> |アプリケーションで空の **ID** が指定されているとき。  <br/> |アプリケーションで、空の文字列が識別子に渡されました。正しい形式の有効な識別子があることを確認します。  <br/> |
|ErrorInvalidIdMalformed  <br/> |**ID** の構造で、内部の整合性に問題があるとき。  <br/> |Exchange は解析後の **ID** で問題を検出しました。ID が正しく変換されていない可能性があります。適切な種類の変換をご使用ください。<br/> |
|ErrorInvalidIdMalformedEwsLegacyIdFormat  <br/> |Exchange 2007 形式を使用しているフォルダーまたはアイテム **ID** が、Exchange 2007 SP1 以降のバージョンでの要求に指定されました。   <br/> |Exchange 2007 の ID を Exchange 2007 SP1 以降の要求で使用することはできません。 先に、[ConvertId](https://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx) EWS 操作または EWS マネージ API の [ConvertId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.convertid%28v=exchg.80%29.aspx) メソッドを使用して、それらを変換する必要があります。  <br/> |
|ErrorInvalidIdNotAnItemAttachmentId  <br/> |**AttachmentId** プロパティがアイテムの添付ファイルを参照していないとき。  <br/> |識別子の形式は正しい可能性がありますが、サーバーが操作しようとしていたものとは異なります。操作する正しい識別子を参照していることをご確認ください。  <br/> |
|ErrorInvalidIdReturnedByResolveNames  <br/> |メールボックス内の連絡先が破損しているとき。  <br/> |EWS の [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) 操作または EWS マネージ API の[ResolveName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) メソッドが返す識別子が無効のとき。 連絡先を再作成する必要がある場合があります。  <br/> |
|ErrorInvalidIdStoreObjectIdTooLong  <br/> |**ID** の構造で、内部の整合性に問題があるとき。  <br/> |Exchange は解析後の **ID** で問題を検出しました。**ID** が正しく変換されていない可能性があります。適切な種類の変換をご使用ください。<br/> |
|ErrorInvalidIdTooManyAttachmentLevels  <br/> |添付物の階層が、深さの最大値の 255 レベルを超えているとき。  <br/> |要求で指定された **AttachmentId** プロパティの値は、正しい構造である可能性がありますが、要求された添付物の階層が深すぎます。255 レベルの限度を超えるアイテムをコードが添付しようとしている可能性があります。  <br/> |
|ErrorInvalidImContactId  <br/> |[RemoveImContactFromGroup 操作](https://msdn.microsoft.com/library/a190bbec-c71b-4e6a-880b-55854c724d8c%28Office.15%29.aspx)を使用していて、連絡先が IM グループで見つからない場合、このエラーが返される可能性があります。このエラーは、Exchange Online と Exchange 2013 以降のバージョンの Exchange を対象とするクライアントに適用されます。<br/> |要求で指定された **ContactId** プロパティの値は、正しい構造である可能性がありますが、メールボックス内の連絡先に、この構造と一致するものはありません。連絡先が既に削除されている可能性があります。  <br/> |
|ErrorInvalidImGroupId  <br/> |[RemoveImGroup 操作](https://msdn.microsoft.com/library/5e788016-68e0-4a3f-9243-03f6b6c6b389%28Office.15%29.aspx)を行う際にメールボックスでグループが見つからない場合、このエラーが返される場合があります。 このエラーは、Exchange Online と Exchange 2013 以降のバージョンの Exchange を対象とするクライアントに適用されます。  <br/> |要求で指定された **GroupId** プロパティの値は、正しい構造である可能性がありますが、メールボックス内のグループに、この構造と一致するものはありません。グループが既に削除されている可能性があります。  <br/> |
|ErrorInvalidReferenceItem  <br/> |参照されているアイテムの識別子は、**MessageType**、**ExchangeWebServices.CalendarItemTypeType**、その子孫の 1 つのいずれでもありません。参照アイテムの識別子は、**CalendarItemType** オブジェクト用であり、開催者は返信、または全員に返信しようとしています。<br/> |識別子の形式は正しい可能性がありますが、サーバーが操作しようとしていたものとは異なります。操作する正しい識別子を参照していることをご確認ください。  <br/> |
|ErrorMissingManagedFolderId  <br/> |フォルダーに対してポリシー ID プロパティ (プロパティ タグ 0x6732) が指定されていません。  <br/> |フォルダーが破損しています。再作成をご検討ください。  <br/> |
   
## <a name="converting-identifiers"></a>識別子の変換
<a name="bk_ConvertingIdentifiers"> </a>

識別子を、ある形式から別の形式に変換することが必要になる場合があります。 たとえば、EWS の外部からの識別子 (MAPI 接続からの識別子など) を、アプリケーションが使用できる形式に変換することが必要になる場合があります。 これを行うには、EWS の [ConvertId](https://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx) 操作または EWS マネージ API の [ConvertId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.convertid%28v=exchg.80%29.aspx) メソッドを使用できます。 
  
たとえば、EntryID は、アイテムを保存するときに、ストアによって割り当てられる MAPI メッセージ ストアによって生成される一意の識別子です。EntryID をアプリケーションで使用するには、最初に EwsId に変換する必要があります。  
  
Outlook Web App は、フォルダーおよびアイテムにアクセスするための URL 内で、独自のバージョンの識別子 (OwaId と呼ばれる) を使用します。アプリケーションが Outlook Web App のアイテムにアクセスする必要がある場合、OwaId を EwsId に変換する必要があります。
  
**ConvertId** 操作またはメソッドを使用して、いくつかの異なる識別子の形式を変換できます。 
  
**表 3. Exchange で変換可能な識別子の形式**

|**形式**|**説明**|
|:-----|:-----|
|EwsLegacyId  <br/> |この EwsId は、Exchange 2007 に適用されます。  <br/> |
|EwsId  <br/> |この EwsId は、Exchange Online、Exchange 2007 SP1 以降のバージョンの Exchange に適用されます。  <br/> |
|StoreId  <br/> |フォルダーとアイテムが格納されている Exchange ストアの識別子です。  <br/> |
|OwaId  <br/> |Exchange 2007 と Exchange 2010 の Outlook Web App で使用する Outlook Web App 識別子です。 <br/><br/>**注意**: Exchange Online と Exchange 2013 以降のバージョンの Exchange は、Outlook Web App で EwsId を使用します。           |
|EntryId  <br/> |MAPI メッセージの **PR_ENTRYID** プロパティとして一般的に知られる、MAPI 識別子です。  <br/> |
|HexEntryId  <br/> |**PR_ENTRYID** プロパティを 16 進数でエンコードした表現で、空き時間の予定表のイベント識別子のために使用されます。これは、Outlook が使用する識別子の形式でもあります。  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange 用の Web サービス クライアントの開発](develop-web-service-clients-for-exchange.md)  
- [ConvertId 操作](https://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx)  
- [ServiceError 列挙体](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) 
- [Exchange で、EWS を使ってのアイテムの削除](deleting-items-by-using-ews-in-exchange.md)
    

