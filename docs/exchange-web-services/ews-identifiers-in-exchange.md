---
title: Exchange の EWS 識別子
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 39b6b20b-e081-4347-9e15-9b8cf829fdf0
description: Exchange での識別子、およびそれらを EWS マネージ API と EWS アプリケーションで使用する方法について説明します。
ms.openlocfilehash: c09b54c8ec4f443a64f8222094ccf0a5e1f750e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758911"
---
# <a name="ews-identifiers-in-exchange"></a>Exchange の EWS 識別子

Exchange での識別子、およびそれらを EWS マネージ API と EWS アプリケーションで使用する方法について説明します。
  
Exchange ストア内のすべてのオブジェクトには、一意の識別子があります。 オブジェクトを参照して、他のオブジェクトと区別するためには、オブジェクトの識別子を使用することができます。 使用可能な 2 つの最も一般的な識別子は、フォルダーと項目の識別子です。 
  
識別子、およびそれらのアプリケーションに重要な理解するために Exchange オブジェクト間の関係を理解しておくことをお勧めします。 EWS のマネージ API または EWS アプリケーションは、Exchange と通信すると、メールボックス、フォルダー、およびアイテム オブジェクトを含むオブジェクトの階層を操作します。 ストアは、これらのオブジェクト タイプのいずれかにできます。 ほとんどの場合、Exchange サーバー上のメールボックスが Exchange サーバー上のパブリック フォルダーにもできます。 (その Exchange Online を Office 365 の一部のバージョンの Exchange が Exchange 2013 を起動すると Exchange Online に注意してください、パブリック フォルダーは、メールボックスの 1 つの種類とさまざまな種類のストアされません)。ストアにフォルダーが含まれているフォルダーにアイテムが含まれているし、のこれらのフォルダーとアイテムは、識別子では、次の図に示すようにします。 
  
**図 1 です。メールボックス、フォルダー、およびアイテムの階層構造**

![メールボックス オブジェクトの階層を示す図。メールボックスが最上位レベルにあり、[受信トレイ] フォルダーが次のレベルにあります。図には、電子メールを格納したフォルダーが表示されています。識別子および変更キーが各オブジェクトに対してリストされており、短縮されています。](media/Ex15_Identifier_diagram.png)
  
## <a name="ews-identifiers"></a>EWS 識別子
<a name="bk_CommonIdentifiers"> </a>

EWS を使用して、フォルダーおよびアイテムの識別子は、EWS 識別子、または EwsIds と呼ばれます。 EwsIds は EWS、内の多数の異なるオブジェクトを参照していますと呼ばれる別の何か別のオブジェクトの。 アプリケーションでこれらのオブジェクトを使用する場合がありますので、EwsId にこれらのオブジェクトの識別子を関連付ける方法を理解します。 
  
さらに、EWS の識別子は、EWS マネージ API にも適用できます。EWS マネージ API では、識別子はオブジェクトのプロパティであり、EWS 要素にマッピングされるよう内部で管理されます。
  
**表 1 です。EWS でのオブジェクトの識別子**

|**オブジェクト**|**識別子**|**関係について EwsId でしょうか。**|
|:-----|:-----|:-----|
|[カレンダー項目](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |[ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx)の子要素には、予定表アイテムの一意の識別子が含まれています。  <br/> |[ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx)の子要素は、このアイテムの EwsId と同じです。  <br/> |
|[ConversationId](http://msdn.microsoft.com/library/d5f1ddb3-9af3-4677-a6ba-111b304a951e%28Office.15%29.aspx) <br/> |**Id**属性には、この項目が含まれるメッセージ交換の識別子が含まれています。  <br/> |**Id**属性は、この項目の EwsId と同じです。  <br/> |
|[AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) <br/> |添付ファイルの一意の識別子を提供します。 [RootItemId](http://msdn.microsoft.com/library/f613c705-17ce-48ce-aa64-4dc2cea25e31%28Office.15%29.aspx)属性には、添付ファイルが関連付けられているルート ストア アイテムの一意の識別子が含まれています。  <br/> |ケース[AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx)が、EwsId と同じには、Exchange ストア内の他のアイテムの添付ファイルを使用できます。 いずれの場合も、ストア内の項目を参照しているため、EwsId では[RootItemId です](http://msdn.microsoft.com/library/f613c705-17ce-48ce-aa64-4dc2cea25e31%28Office.15%29.aspx)。  <br/> |
|[PersonaId](http://msdn.microsoft.com/library/eec3a468-afd5-4d72-a61e-cd1964fb686c%28Office.15%29.aspx) <br/> |**Id**属性は、ペルソナの識別子を含む文字列を返します。  <br/> |**Id**属性は、ペルソナの EwsId と同じです。  <br/> |
|[ContactId](http://msdn.microsoft.com/library/86f66275-1e39-48ed-bd89-ac3bffc465a7%28Office.15%29.aspx) <br/> |**Id**属性では、取引先担当者の識別子を含む文字列を返します。  <br/> |**Id**属性は、連絡先の EwsId と同じです。  <br/> |
|[グループ Id](http://msdn.microsoft.com/library/656d9b9a-8a65-4a75-8466-5b0d96512dab%28Office.15%29.aspx) <br/> |**Id**属性は、グループの識別子を含む文字列を返します。  <br/> |**Id**属性は、グループの EwsId と同じです。  <br/> |
|[AssociatedCalendarItemId](http://msdn.microsoft.com/library/5b29898c-ea59-4e6a-914c-c011ec754032%28Office.15%29.aspx) <br/> |**Id**属性は、 [MeetingMessage](http://msdn.microsoft.com/library/c95956a8-7505-44b4-bea4-11d1f5182796%28Office.15%29.aspx)、 [MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx)、 [MeetingResponse](http://msdn.microsoft.com/library/9f798e79-dafd-4d4d-9967-95fd8e5c0502%28Office.15%29.aspx)、または[MeetingCancellation](http://msdn.microsoft.com/library/a9c61f7f-2ecd-4b21-9dce-24d9f61aeeea%28Office.15%29.aspx)に関連付けられている予定表アイテムを識別します。  <br/> |**Id**属性は、予定表アイテムの EwsId と同じです。  <br/> |
|[UserConfigurationProperties](http://msdn.microsoft.com/library/c143a6ec-62ad-4d48-b844-b1ad88054bc1%28Office.15%29.aspx) <br/> |この要素の**Id**値は、識別子のプロパティを指定します。  <br/> |この識別子は、プロパティの識別子であってアイテムではないため、直接には EwsId にマッピングされません。  <br/> |
|[OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) <br/> |**RecurringMasterId**属性では、定期的なアイテムのマスターを識別します。  <br/> |**OccurrenceItemId**値は、EwsId に直接マップされないが、 **RecurringMasterId**の定期的なアイテムの最上位レベルのオブジェクトを参照しているためです。  <br/> |
|[StoreEntryId](http://msdn.microsoft.com/library/f536e264-8c4d-4cc5-bab8-22a4fa38de39%28Office.15%29.aspx) <br/> |アイテムの Exchange ストア識別子が含まれています。   <br/> |**StoreEntryId**値は、EwsId にはマップされませんが、アイテムが保存されているストアの id を与えることは。  <br/> |
   
## <a name="working-with-identifiers"></a>識別子の処理
<a name="bk_WorkingWithIdentifiers"> </a>

Exchange サーバーは、さまざまな方法で識別子を処理します。EWS マネージ API または EWS アプリケーションを開発する場合、以下をご考慮ください。
  
- フォルダーおよびアイテムの**アイテム Id**要素の値は、大文字小文字を区別します。 場合は、フォルダーまたは[FindItem 操作](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)など、 [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) EWS のマネージ API のメソッドによって返される項目の項目 ID を見ると、別の項目 ID の重複していることと思われる場合があります。ただし、2 つの項目の項目 Id の 1 つまたは複数の文字は、さまざまな大文字と小文字があります。 
    
- 項目 ID を後で取得するためにデータベースに格納する場合は、お勧めフィールド サイズは、512 バイトである GUID を保持するのに十分な大きさになるようです。
    
- 限らないことに ID が常に有効では後で、項目を取得する必要がある場合。 場合は、ストア内のアイテムを移動すると、移動の処理方法があるため、ID を変更できます。 アイテムが実際にコピーされ、新しい ID を生成すると、後に[元のアイテムを削除](deleting-items-by-using-ews-in-exchange.md)します。
    
- Exchange の識別子は、符号化されています。たとえば、開発者にとっては重要ではないものの、Exchange にとって重要ないくつかの情報から EwsId が作成されます。
    
- アイテムを Exchange で使用するときに注意してくださいするのには別の値は、**変更キー**属性です。 項目の ID だけでなく、この値は、項目の状態を追跡するために使用されます。 アイテムが変更されると、いつでも新しいキーの変更が生成されます。 [UpdateItem 操作](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)を実行すると、たとえば、サーバーに項目の最新バージョンに更新プログラムが適用されているかを理解させる**変更キー**の属性を使用することができます。 場合は別のアプリケーションでは、更新する項目に変更を加えた、変更キーが一致しませんし、更新プログラムを実行することはできません。 
    
## <a name="distinguished-folder-ids"></a>識別フォルダー ID 
<a name="bk_DistinguishedFolderIds"> </a>

Exchange には、識別フォルダー ID と呼ばれる識別子を割り当てられているは、定義済みのメールボックス フォルダーの数が含まれます。 これらは、 [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx)の EWS のマネージ API の列挙体と[DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx)の EWS の要素によって定義されます。 簡単に参照する定義済みのフォルダーの場合は、これらの識別フォルダー Id を使用することができます。 たとえば、受信トレイ フォルダーでは、単に使用できます「受信トレイ」フォルダーの識別子を決定するのではなく、識別子。 
  
メール アイテムを整理するために作成する他のフォルダーにも、そのフォルダーに対して一意な ID が付けられます。その ID は、フォルダーの他のプロパティを変更しても、変更されることはありません。
  
識別フォルダー Id は、代理人アクセスのエントリ ポイントとして使用できます。 代理人アクセスを開始すると、アイテムやフォルダーを検索して識別フォルダー ID を検索する場所を指定するのには。 代理ユーザーにアクセスするサーバーが、メールボックスの代理人アクセスを明示的に指定するのには**DistinguishedFolderId**要素の子である[メールボックス](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx)の要素が使用されます。 
  
## <a name="handling-errors"></a>エラーの処理
<a name="bk_DealingWithErrors"> </a>

エラーを取得するすべてのプログラムがバインドされているし、EWS ベースのアプリケーション例外 (だじゃれ) ではありません。 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) EWS の要素で、またはの一部として、いくつかの識別子に関連するエラーが表示される可能性があります、[サービス エラー](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx)の EWS のマネージ API の列挙体の。 
  
EWS のマネージ API または EWS アプリケーションで、次のエラーが発生ことができます。 エラーは、プロパティの値に関する問題は、通常、EWS のマネージ API アプリケーションで使用している場合EWS アプリケーションは、エラーは、XML 要素の値または操作に関連付けられます。
  
**表 2 になります。識別子に関連するエラー**

|**Error**|**発生したとしています.**|**説明**|
|:-----|:-----|:-----|
|ErrorCalendarCannotUseIdForOccurrenceId  <br/> |**OccurenceID**の値は、有効な定期的な予定表アイテムには対応していません。  <br/> |要求で指定された**OccurenceId**の値は、構造体で有効である可能性がありますが、要求で可能性があります既存の定期的なマスターと一致しません。 定期的なアイテムは、予定表から削除する場合があります。 アイテムがまだ存在していると、正しい識別子を使用していることを確認します。  <br/> |
|ErrorCalendarCannotUseIdForRecurringMasterId  <br/> |**OccurrenceId**要素の有効なアイテムには、 **RecurringMasterId**属性は対応していません。  <br/> |要求で指定された**RecurringMasterId**の値は、構造体で有効である可能性がありますが、要求で可能性があります、アイテムの既存の出現に一致しません。 アイテムの出現は、予定表から削除する可能性があります。 アイテムがまだ存在していると、正しい識別子を使用していることを確認します。  <br/> |
|ErrorCannotUseFolderIdForItemId  <br/> |渡された**ID**はアイテムではなくフォルダーを表します。  <br/> |識別子の形式は正しい可能性がありますが、サーバーが操作しようとしていたものとは異なります。操作する正しい識別子を参照していることをご確認ください。  <br/> |
|ErrorCannotUseItemIdForFolderId  <br/> |渡された**ID**はフォルダーではなくアイテムを表します。  <br/> |識別子は、形式がどのようなサーバーが予期しない操作のために有効な可能性があります。 操作のための正しい**ID**を参照していることを確認します。  <br/> |
|ErrorChangeKeyRequiredForWriteOperations  <br/> |特定の更新操作を実行しているときは、正しい変更キーを指定する必要があります。  <br/> |、更新を要求すると、キーの変更が正しくないか、**変更キー**の値を省略するとします。 更新操作を実行すると、キーの適切な変更があることを確認します。  <br/> |
|ErrorInvalidAttachmentId  <br/> |添付物が、アイテムの添付ファイル コレクション内で見つかりませんでした。  <br/> |添付ファイル**ID**があると、添付ファイルを削除しようとして添付ファイル ID に対して[GetAttachment 操作](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx)を呼び出す場合、この応答コードが表示される場合があります。 添付ファイルが添付ファイル コレクション内に存在することを確認します。  <br/> |
|ErrorInvalidChangeKey  <br/> |使用できない変更キーが渡されました。   <br/> |変更キーを渡す必要がある操作とメソッドは多くないことにご注意ください。しかし、変更キーを指定する場合、それは必ずしも最新である必要はありませんが、正しくなければなりません。  <br/> |
|ErrorInvalidFolderId  <br/> |フォルダー **ID**が破損しています。  <br/> |適切な形式の、正しい識別子があることを確認します。  <br/> |
|ErrorInvalidId  <br/> |**ID**や変更キーの構造が内部的に矛盾ではありません。  <br/> |Exchange では、解析された後、 **ID**の問題が発生しました。 あった可能性がありますエラー変換にします。 これが発生することなど、Outlook のアイテムを**IdFormatType.HexEntryId**がある場合は、EwsId の考え方に変換するが、 **IdFormatType.EntryId**の形式です。 適切な変換の種類を使用することを確認します。  <br/> |
|ErrorInvalidIdEmpty  <br/> |アプリケーションでは、空では**ID**を指定します。  <br/> |アプリケーションは、識別子として空の文字列を渡しました。適切な形式の、正しい識別子があることを確認します。  <br/> |
|ErrorInvalidIdMalformed  <br/> |**ID**の構造が内部的に矛盾ではありません。  <br/> |Exchange では、解析された後、 **ID**の問題が発生しました。 ID が正しく変換されていない可能性があります。 適切な変換の種類を使用することを確認します。  <br/> |
|ErrorInvalidIdMalformedEwsLegacyIdFormat  <br/> |フォルダーや、Exchange 2007 形式を使用している項目の**ID**は、Exchange 2007 SP1 またはそれ以降のバージョンで要求に指定されました。  <br/> |Exchange 2007 SP1 またはそれ以降の要求での Exchange 2007 の Id を使用することはできません。 [ConvertId](http://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx) EWS 操作または[ConvertId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.convertid%28v=exchg.80%29.aspx)の EWS のマネージ API のメソッドを使用して、最初に変換する必要があります。  <br/> |
|ErrorInvalidIdNotAnItemAttachmentId  <br/> |**AttachmentId**プロパティは、アイテムの添付ファイルを参照していません。  <br/> |識別子の形式は正しい可能性がありますが、サーバーが操作しようとしていたものとは異なります。操作する正しい識別子を参照していることをご確認ください。  <br/> |
|ErrorInvalidIdReturnedByResolveNames  <br/> |メールボックス内の連絡先が破損しています。  <br/> |[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) EWS 操作または[ResolveName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) EWS のマネージ API のメソッドに 1 つまたは複数の識別子が返されますが、それらが有効ではありません。 連絡先を再作成する必要があります。  <br/> |
|ErrorInvalidIdStoreObjectIdTooLong  <br/> |**ID**の構造が内部的に矛盾ではありません。  <br/> |Exchange では、解析された後、 **ID**の問題が発生しました。 **ID**が正しく変換されていない可能性があります。 適切な変換の種類を使用することを確認します。  <br/> |
|ErrorInvalidIdTooManyAttachmentLevels  <br/> |添付物の階層が、深さの最大値の 255 レベルを超えています。  <br/> |要求で指定された**AttachmentId**プロパティの値は構造体で有効である可能性がありますが、添付されたファイルは、階層の深すぎます。 255 レベルの制限を超えるアイテムを添付するのには、コードをした可能性があります。  <br/> |
|ErrorInvalidImContactId  <br/> |連絡先で見つからない場合、IM グループで[RemoveImContactFromGroup 操作](http://msdn.microsoft.com/library/a190bbec-c71b-4e6a-880b-55854c724d8c%28Office.15%29.aspx)を使用するときにこのエラーが返されます。 このエラーは、Exchange Online とのバージョンの Exchange が Exchange 2013 で開始するクライアントに適用されます。  <br/> |要求で指定された **<** プロパティの値は構造体で有効である可能性がありますが、この構造に一致する、メールボックス内の連絡先はありません。 連絡先が既に削除されている可能性があります。  <br/> |
|ErrorInvalidImGroupId  <br/> |グループで見つからない場合、メールボックスで[RemoveImGroup 操作](http://msdn.microsoft.com/library/5e788016-68e0-4a3f-9243-03f6b6c6b389%28Office.15%29.aspx)を使用するときにこのエラーが返されます。 このエラーは、Exchange Online とのバージョンの Exchange が Exchange 2013 で開始するクライアントに適用されます。  <br/> |要求で指定された**グループ Id**のプロパティの値は構造体で有効である可能性がありますが、この構造に一致する、メールボックス内のグループはありません。 グループは既に削除されている可能性があります。  <br/> |
|ErrorInvalidReferenceItem  <br/> |参照されている項目の識別子は、**メッセージの種類**または**ExchangeWebServices.CalendarItemTypeType**、またはその子孫のいずれかではありません。 **CalendarItemType**オブジェクト用の参照項目の識別子であるし、開催者が返信] または [全員に返信ましょう。  <br/> |識別子の形式は正しい可能性がありますが、サーバーが操作しようとしていたものとは異なります。操作する正しい識別子を参照していることをご確認ください。  <br/> |
|ErrorMissingManagedFolderId  <br/> |フォルダーに対してポリシー ID プロパティ (プロパティ タグ 0x6732) が指定されていません。   <br/> |フォルダーが破損しています。再作成をご検討ください。  <br/> |
   
## <a name="converting-identifiers"></a>識別子の変換
<a name="bk_ConvertingIdentifiers"> </a>

識別子を別の 1 つの形式に変換する必要があります。 などの MAPI 接続の場合、アプリケーションが使用できる形式には、識別子など、外部の EWS から識別子に変換する必要があります。 これを行うには、 [ConvertId](http://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx)の EWS 操作、または[ConvertId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.convertid%28v=exchg.80%29.aspx)の EWS のマネージ API のメソッドを使用できます。 
  
たとえば、EntryID は、アイテムを保存するときに、ストアによって割り当てられる MAPI メッセージ ストアによって生成される一意の識別子です。EntryID をアプリケーションで使用するには、最初に EwsId に変換する必要があります。  
  
Outlook Web App は、フォルダーおよびアイテムにアクセスするための URL 内で、独自のバージョンの識別子 (OwaId と呼ばれる) を使用します。アプリケーションが Outlook Web App のアイテムにアクセスする必要がある場合、OwaId を EwsId に変換する必要があります。
  
**ConvertId**操作またはメソッドを使用するには、いくつかの異なる識別子の形式に変換します。 
  
**表 3。変換可能な識別子が Exchange 形式します。**

|**Format**|**説明**|
|:-----|:-----|
|EwsLegacyId  <br/> |この EwsId は、Exchange 2007 に適用されます。  <br/> |
|EwsId  <br/> |この EwsId は、Exchange Online、Exchange 2007 SP1 以降のバージョンの Exchange に適用されます。  <br/> |
|StoreId  <br/> |フォルダーとアイテムが格納されている Exchange ストアの識別子です。  <br/> |
|OwaId  <br/> |Exchange 2007 と Exchange 2010 の Outlook Web App で使用する Outlook Web App 識別子です。   <br/> > [!NOTE]> Exchange Online とのバージョンの Exchange が Exchange 2013 で始まるは、Outlook Web App で、EwsId を使用します。           |
|EntryId  <br/> |MAPI メッセージの**PR_ENTRYID**プロパティと呼ばれる MAPI 識別子です。  <br/> |
|HexEntryId  <br/> |可用性の予定表のイベント識別子を使用する**PR_ENTRYID**プロパティの 16 進数でエンコードされた表現。 Outlook を使用する識別子の形式です。  <br/> |
   
## <a name="see-also"></a>関連項目


- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    
- [ConvertId 操作](http://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx)
    
- [サービス エラーの列挙](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx)
    
- [Exchange の EWS を使用するアイテムの削除](deleting-items-by-using-ews-in-exchange.md)
    

