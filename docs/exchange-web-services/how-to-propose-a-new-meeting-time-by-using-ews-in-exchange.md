---
title: Exchange で EWS を使用して会議の新しい日時を提案する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d5ac8e5b-3876-4f20-b4d3-44505e066042
description: Exchange で EWS を使用して Exchange クライアント アプリケーションから新しい会議日時を提案する方法について説明します。
ms.openlocfilehash: 4f001bb82d2325624b567412620283619b51f25b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456813"
---
# <a name="propose-a-new-meeting-time-by-using-ews-in-exchange"></a>Exchange で EWS を使用して会議の新しい日時を提案する

Exchange で EWS を使用して Exchange クライアント アプリケーションから新しい会議日時を提案する方法について説明します。
  
出席者は、新しい日時を提案する機能を使用して、新しい会議日時を Exchange 予定表ワークフローの一部として会議開催者に提案できます。出席者が新しい会議を提案すると、開催者は提案された新しい会議日時を使用して会議を更新し、最新情報をすべての出席者に送信できます。新しい会議日時を出席者が提案できるようにするためには、新しい日時の提案を開催者が許可しているかどうかを確認しておく必要があります。この記事では、新しい日時を提案できるかどうかを確認する方法、および EWS を使用して新しい日時を提案する方法について説明します。
  
> [!NOTE]
> EWS マネージ API はこの機能を実装していません。 
  
## <a name="determine-whether-you-can-propose-a-new-time-for-a-meeting-by-using-ews"></a>EWS を使用して会議の新しい日時を提案できるかどうかを確認する
<a name="bk_Determine"> </a>

会議の新しい日時を提案するためには、その会議への参照を見つけ、新しい日時の提案をサポートするように会議開催者が会議を構成しているかどうかを確認しておく必要があります。会議への参照は、次のいずれかの方法で取得できます。  
  
- 受信トレイで会議出席依頼を見つける
    
- 予定表で予定を見つける
    
会議の参照を見つけるには、次の手順を使用します。
  
1. [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS 操作 (または [Folder.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=EXCHG.80%29.aspx) EWS マネージ API メソッド) を使用して、対象の会議出席依頼アイテムまたは予定表アイテムを見つけます。 あるいは、[SyncFolderItems](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) EWS 操作を使用して、対象の会議出席依頼アイテムまたは予定表アイテムの識別子を取得することもできます。 
    
2. **FindItem** 操作 (または **Folder.FindItems** メソッド) の結果を解析して、会議アイテムのアイテム識別子を取得します。 
    
3. [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS 操作を使用して、会議の応答オブジェクトを取得します。 
    
次の XML は、アイテムの応答オブジェクトを要求するために何が送られるかを示しています。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:MailboxCulture>en-US</t:MailboxCulture>
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:ResponseObjects"/>
          <t:FieldURI FieldURI="item:Subject"/>
          <t:FieldURI FieldURI="calendar:Start"/>
          <t:FieldURI FieldURI="calendar:End"/>
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkADEzOTExYjJkL1AAA=" ChangeKey="CwAAAB/G6X"/>
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

アイテム識別子、会議の開始時刻と終了時刻、応答オブジェクト コレクション、および会議日時変更提案を開催者が許可しているかどうかを要求した場合、**GetItem** 操作の応答は次の XML のようになります。 [ResponseObjects](https://msdn.microsoft.com/library/ad29e064-3f3d-4b7b-aa4c-9ec27326381d%28Office.15%29.aspx) 要素で表される応答オブジェクト コレクションには、予定表アイテムに有効な応答のセットが含まれます。 **ProposeNewTime** 要素は、新しい会議日時をユーザーが提案できることを示す応答オブジェクトです。 [AcceptItem](https://msdn.microsoft.com/library/05a15431-77e1-411a-a16b-5481d364d3cc%28Office.15%29.aspx)、[TentativelyAcceptItem](https://msdn.microsoft.com/library/ce6f50ef-ad8a-47e4-915a-487b2ef7a2e0%28Office.15%29.aspx)、および [DeclineItem](https://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) 要素は、新しい会議日時を会議開催者に提案するために使用できる応答オブジェクトを表します。 
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:MeetingRequest>
              <t:ItemId Id="AAMkADEzOTExYjJkL1AAA=" ChangeKey="CwAAAB/G6X"/>
              <t:Subject>Competitive analysis: kick off meeting</t:Subject>
              <t:ResponseObjects>
                <t:AcceptItem/>
                <t:TentativelyAcceptItem/>
                <t:DeclineItem/>
                <t:ProposeNewTime/>
                <t:ReplyToItem/>
                <t:ReplyAllToItem/>
                <t:ForwardItem/>
              </t:ResponseObjects>
              <t:Start>2013-11-09T17:00:00Z</t:Start>
              <t:End>2013-11-09T17:30:00Z</t:End>
            </t:MeetingRequest>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="propose-a-new-meeting-time-by-using-ews"></a>EWS を使用して新しい会議日時を提案する
<a name="bk_Propose"> </a>

**GetItem** 操作を使用して予定表アイテムまたは会議出席依頼を取得した際に **ProposeNewTime** 応答オブジェクトを受け取ったら、新しい会議日時の提案で応答できます。 **ProposeNewTime** 応答オブジェクトを受け取らなかった場合、新しい会議日時を予定表ワークフローの一部として提案することはできません。 ただし、開催者に返信して、新しい会議日時を要求することができます。 **ProposeNewTime** 応答オブジェクトを受け取った場合は、会議に対してその識別子を参照して応答し、新しい会議日時を開催者に提案できます。 ここが、**ProposeNewTime** 応答オブジェクトを使用して応答しない通常の応答オブジェクト パターンと **ProposeNewTime** 応答オブジェクトが異なる点です。 **AcceptItem**、**TentativelyAcceptItem**、または **DeclineItem** などの他の会議応答オブジェクトのいずれかを使用して、新しい会議を提案します。 この例では、**AcceptItem** 応答オブジェクトを使用しています。 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013"/>
  </soap:Header>
  <soap:Body>
    <m:CreateItem>
      <m:Items>
        <t:AcceptItem>
          <t:Body BodyType="Text">This time works better for the HiPPO.</t:Body>
          <t:ReferenceItemId Id="AAMkADEzOTExYjJkL1AAA=" ChangeKey="CwAAAB/G6X"/>
          <t:ProposedStart>2013-11-28T04:00:00Z</t:ProposedStart>
          <t:ProposedEnd>2013-11-28T04:30:00Z</t:ProposedEnd>
        </t:AcceptItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

この要求への応答には、出席者の予定表に追加された予定表アイテムの識別子、および出席者の [削除済みアイテム] フォルダーに置かれた会議出席依頼のコピーが含まれます。 新しい日時の提案を含む応答メッセージは、出席者の [送信済みアイテム] フォルダーにも保存されます (会議応答メッセージのハンドルを取得するには、その会議応答メッセージを見つける必要があります)。
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkAGRmOWE2OWAAA=" ChangeKey="DwAAJsmU"/>
            </t:CalendarItem>
            <t:MeetingRequest>
              <t:ItemId Id="AAMkAGRmOWE2AAABB=" ChangeKey="AAAGJu1A"/>
            </t:MeetingRequest>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>
```

出席者が新しい会議日時の提案で応答すると、開催者は [MeetingResponse](https://msdn.microsoft.com/library/9f798e79-dafd-4d4d-9967-95fd8e5c0502%28Office.15%29.aspx) メッセージを受け取ります。 **MeetingResponse** メッセージには、会議の新しい開始時刻と終了時刻の提案、開催者の予定表の中の関連予定表アイテムの識別子が含まれます。 開催者はその情報を使用して、会議を表す既存の予定表アイテムを更新できます。 新しい会議日時を提案する **MeetingResponse** メッセージに開催者が応答するワークフローを次に示します。 
  
1. **ProposedStart** 要素、または **ProposedEnd** 要素が **MeetingResponse** で設定されているかどうかを判断します。 設定されている場合は、手順 2 に進みます。 設定されていない場合、**MeetingResponse** メッセージは、出席者が会議を承諾した、仮承諾した、または辞退したことのみを示します。 
    
2. **AssociatedCalendarItemId** 要素で返される EWS 識別子を使用して、会議を表す開催者の既存予定表アイテムを取得します。  
    
3. 元の開始時刻と終了時刻を、提案された新しい会議日時と比較します。提案された新しい会議日時を開催者が受け入れることができる場合は、手順 4 に進みます。それ以外の場合、会議開催者は、提案された会議日時を無視するか、新しい会議日時を提案した出席者にメール応答を送信できます。
    
4. (省略可能) [GetUserAvailability](https://msdn.microsoft.com/library/8da17226-5d3a-4525-9ffa-d83730f47bb1%28Office.15%29.aspx) EWS 操作呼び出しを実行して、提案された日時がすべての出席者 (部屋およびリソース メールボックスを含む) にとって都合がよいかどうかを調べます。 (これを行うには、[ExchangeService.GetUserAvailability](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getuseravailability%28v=exchg.80%29.aspx) EWS マネージ API メソッドを使用することもできます。) 
    
5. その後開催者は、[UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) EWS 操作 (または [Appointment.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) EWS マネージ API メソッド) を使用して、提案された新しい会議日時に基づいて会議を更新し、最新情報をすべての出席者に送信できます。 
    
次の図は、会議開催者、出席者、および EWS 呼び出しを処理する Exchange サーバーの間で行われるプロセスを示しています。
  
**図 1. 新しい会議日時の提案プロセス**

![図は、新しい会議時間が提案された際の、開催者、Exchange、出席者間のワークフローを示しています。開催者が新しい会議の提案を許可する場合、出席者は応答オブジェクトを使用して新しい会議時間を提案できます。](media/Ex_ProposeNewMeetingTime.png)
  
## <a name="version-differences"></a>バージョンの相違点
<a name="bk_Behavior"> </a>

新しい日時を提案する機能は、Exchange ビルド バージョン 15.00.0800.007 で導入されました。以前のバージョンの Exchange では、EWS アプリケーション ユーザーは、異なる会議日時を要求するためには、別個のメールを会議開催者に送信する必要があります。  
  
## <a name="see-also"></a>関連項目


- [Exchange の予定表と EWS](calendars-and-ews-in-exchange.md)
    
- [Exchange 2013 で EWS を使用して予定と会議を作成する](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Exchange の EWS を使用して予定と会議を取得する](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Exchange で EWS を使用して予定と会議を更新する](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Exchange の EWS を使用して、予定を削除し、会議をキャンセルする](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

