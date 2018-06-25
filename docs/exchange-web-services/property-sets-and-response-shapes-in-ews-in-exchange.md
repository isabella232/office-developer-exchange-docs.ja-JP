---
title: Exchange の EWS でのプロパティ セットと応答の図形
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 04a29804-6067-48e7-9f5c-534e253a230e
description: EWS マネージ API および Exchange の EWS から返される応答の図形とプロパティ セットを管理する方法について説明します。
ms.openlocfilehash: d9fd6c155438dfd03cfc9536397316cf3faa2287
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759199"
---
# <a name="property-sets-and-response-shapes-in-ews-in-exchange"></a>Exchange の EWS でのプロパティ セットと応答の図形

EWS マネージ API および Exchange の EWS から返される応答の図形とプロパティ セットを管理する方法について説明します。
  
Exchange のデータ保存には、連絡先や予定表のエントリなど、さまざまなアイテムを同じフォルダーに格納できる柔軟なストレージ ソリューションが採用されています。しかしそのために、EWS 操作や EWS マネージ API メソッドへの呼び出しから返されるデータを管理するのが困難になることがあります。
  
によって返される Exchange オンラインになって、Office 365 の一部または Excahange のバージョンと Exchange のオンライン Exchange 2013 年から始まる EWS のマネージ API を使用して、プロパティ セット、および EWS 避難用図形を使用してデータを管理するために容易にできるようにします。 これらは、ストアの項目の最も一般的なプロパティを提供する定義済みのコレクションです。 返されるプロパティのセットは、アイテムの種類によって決定されます。 Exchange マネージ API の[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx)メソッドを使用してアイテムをバインドする場合、バインドする項目の種類によってプロパティの異なるセットを入手することを意味します。 予定表アイテムへのバインドは、連絡先アイテムに異なるバインディングよりもプロパティのセットを返します。 同様に、EWS を使用する場合は、 [GetItem 操作](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx)は、返される項目の種類に基づいてプロパティの別のセットを返します。 
  
[Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx)メソッドを使用してフォルダーにバインドまたは[GetFolder の操作](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)を使用しても要求するフォルダーのプロパティのセットを返します。 
  
**表 1 です。図形の定義済みの応答**

|**応答の図形**|**EWS のマネージ API と同じ**|**説明**|
|:-----|:-----|:-----|
|ID のみ  <br/> |[BasePropertySet.IdOnly](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) <br/> |アイテムまたはフォルダーの ID のみを返します。ほとんどのアプリケーションは、この応答の図形を使用し、さらに必要なプロパティを指定します。  <br/> |
|既定値  <br/> |該当なし  <br/> |アイテムまたはフォルダー (EWS のみ) の既定である事前定義プロパティ セットを返します。  <br/> |
|すべてのプロパティ  <br/> |[BasePropertySet.FirstClassProperties](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) <br/> |クライアント アプリケーションで最も頻繁に使用されるプロパティを返します。プロパティ パスを使用して追加のプロパティを返すことができます。  <br/> |
   
## <a name="default-response-shapes"></a>既定の応答の図形

EWS には、フォルダーまたはフォルダー アイテムの既定の応答の図形セットが含まれています。  
  
次の表は、各フォルダーに[FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) 、 [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) EWS の操作によって返される既定のプロパティを一覧します。 
  
**表 2 になります。既定のフォルダーのプロパティ**

|**プロパティ**|**[受信トレイ]**|**予定表**|**連絡先**|**削除済みアイテム**|**[下書き]**|**メモ**|**他のフォルダー**|**[送信トレイ] します。**|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|表示名  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|フォルダー ID  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|サブフォルダーの数  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|総件数  <br/> |X  <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|未読件数  <br/> |X  <br/> |||X  <br/> |X  <br/> ||X  <br/> |X  <br/> |
   
[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)および[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS の操作によって項目の種類ごとに返される既定のプロパティを次の表に一覧します。 
  
**表 3。項目の既定のプロパティ**

|**プロパティ**|**予定表アイテム**|**連絡先アイテム**|**メッセージ アイテム**|**タスク アイテム**|
|:-----|:-----|:-----|:-----|:-----|
|Body  <br/> |||X(1)  <br/> ||
|CalendarItemType  <br/> ||x  <br/> |||
|CompanyName  <br/> ||x  <br/> |||
|CompleteName  <br/> ||x  <br/> |||
|DateTimeCreated  <br/> |||x  <br/> ||
|DateTimeSent  <br/> |||x  <br/> ||
|DueDate  <br/> ||||x(2)  <br/> |
|EmailAddresses  <br/> ||x  <br/> |||
|End  <br/> |x  <br/> ||||
|FileAs  <br/> ||x  <br/> |||
|接続元  <br/> |||x  <br/> ||
|HasAttachments  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ImAddresses  <br/> ||x  <br/> |||
|IsAssociated  <br/> |x  <br/> ||x  <br/> ||
|IsDeliveryReceiptRequested  <br/> |||x  <br/> ||
|ItemId  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|JobTitle  <br/> ||x  <br/> |||
|LegacyFreeBusyStatus  <br/> |x  <br/> ||||
|Location  <br/> |x  <br/> ||||
|開催者  <br/> |x  <br/> ||||
|PercentComplete  <br/> ||||x  <br/> |
|PhoneNumbers  <br/> ||x  <br/> |||
|PhysicalAddresses  <br/> ||x  <br/> |||
|ResponseObjects  <br/> |x(1)  <br/> ||x(1)  <br/> ||
|Sensitity  <br/> |||x  <br/> ||
|サイズ  <br/> |||x  <br/> ||
|StartDate  <br/> ||||x(2)  <br/> |
|Status  <br/> ||||x  <br/> |
|対象  <br/> |x  <br/> ||x  <br/> |x  <br/> |
   
メモ:
  
1. **GetItem**操作からの応答に含まれます。 **FindItem**操作からの応答に含まれません。 
    
2. フィールドにデータがある場合のみ応答に含まれます。フィールドが空白の場合は応答に含まれません。
    
### <a name="all-properties-set-and-response-shape"></a>すべてのプロパティ セットと応答の図形

次の表では、EWS のマネージ API の[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx)と[Item.FindItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) EWS のマネージ API のメソッド、および[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)と[によって返される [すべてのプロパティ] の応答の図形を呼び出すことによって返される最上位のプロパティGetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS 運用します。 
  
プロパティに追加のプロパティを設定または拡張プロパティを含めるを追加することができます。 詳細については、[プロパティ、および Exchange 内の拡張プロパティ](properties-and-extended-properties-in-ews-in-exchange.md)を参照してください。
  
**表 4 です。ファースト クラスのプロパティ**

|||||||
|:-----|:-----|:-----|:-----|:-----|:-----|
|プロパティ  <br/> |予定表アイテム  <br/> |連絡先アイテム  <br/> |メッセージ アイテム  <br/> |投稿アイテム  <br/> |作業アイテム  <br/> |
|ActualWork  <br/> |||||x  <br/> |
|AdjacentMeetingCount  <br/> |x  <br/> |||||
|AdjacentMeetings  <br/> |x  <br/> |||||
|エイリアス  <br/> ||x  <br/> ||||
|AllowNewTimeProposal  <br/> |x  <br/> |||||
|AppointmentReplyTime  <br/> |x  <br/> |||||
|AppointmentSequenceNumber  <br/> |x  <br/> |||||
|AppointmentState  <br/> |x  <br/> |||||
|AssignedTime  <br/> |||||x  <br/> |
|AssistantName  <br/> ||x  <br/> ||||
|BccRecipients  <br/> |||x  <br/> |||
|BillingInformation  <br/> |||||x  <br/> |
|Body  <br/> |x(1)  <br/> |x(1)  <br/> |x(1)  <br/> ||x(1)  <br/> |
|BusinessHomePage  <br/> ||x  <br/> |x  <br/> |||
|CalendarItemType  <br/> |x  <br/> |||||
|カテゴリ  <br/> |x  <br/> ||x  <br/> |x  <br/> |x  <br/> |
|CcRecipients  <br/> |||x  <br/> |||
|ChangeCount  <br/> |||||x  <br/> |
|子供  <br/> ||x  <br/> ||||
|Companies  <br/> |||||x  <br/> |
|CompleteDate  <br/> |||||x  <br/> |
|CompleteName  <br/> ||x  <br/> ||||
|ConferenceType  <br/> |x  <br/> |||||
|ConflictingMeetingCount  <br/> |x  <br/> |||||
|ConflictingMeetings  <br/> |x  <br/> |||||
|連絡先  <br/> |||||x  <br/> |
|ContactSource  <br/> ||x  <br/> ||||
|ConversationId  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ConversationIndex  <br/> |||x  <br/> |x  <br/> ||
|ConversationTopic  <br/> |||x  <br/> |x  <br/> ||
|カルチャ  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DateTimeCreated  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DateTimeReceived  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DateTimeSent  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DateTimeStamp  <br/> |x  <br/> |||||
|DelegationState  <br/> |||||x  <br/> |
|Delegator  <br/> |||||x  <br/> |
|DeletedOccurances  <br/> |x  <br/> |||||
|Department  <br/> ||x  <br/> ||||
|DirectoryId  <br/> ||x  <br/> ||||
|DirectReports  <br/> ||x  <br/> ||||
|DisplayCc  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DisplayName  <br/> ||x  <br/> ||||
|DisplayTo  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DueDate  <br/> |||||x  <br/> |
|Duration  <br/> |x  <br/> |||||
|EffectiveRights  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|EmailAddresses  <br/> ||x  <br/> ||||
|End  <br/> |x  <br/> |||||
|EndTimeZone  <br/> |x  <br/> |||||
|FileAs  <br/> ||x  <br/> ||||
|FileAsMapping  <br/> ||x  <br/> ||||
|FirstOccurance  <br/> |x  <br/> |||||
|接続元  <br/> |||x  <br/> |x  <br/> ||
|Generation  <br/> ||x  <br/> ||||
|GivenName  <br/> ||x  <br/> ||||
|HasAttachments  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|HasPicture  <br/> ||x  <br/> ||||
|ImAddresses  <br/> ||x  <br/> ||||
|Importance  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Initials  <br/> ||x  <br/> ||||
|InReplyTo  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|InternetMessageId  <br/> |||x  <br/> |x  <br/> ||
|InternetMessageHeaders  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsAllDayEvent  <br/> |x  <br/> |||||
|IsAssociated  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsCancelled  <br/> |x  <br/> |||||
|IsComplete  <br/> |||||x  <br/> |
|IsDeliveryReceiptRequested  <br/> |||x  <br/> |||
|IsDraft  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsFromMe  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsMeeting  <br/> |x  <br/> |||||
|IsOnlineMeeting  <br/> |x  <br/> |||||
|IsRead  <br/> |||x  <br/> |||
|IsReadReceiptRequested  <br/> |||x  <br/> |||
|IsRecurring  <br/> |x  <br/> ||||x  <br/> |
|IsResend  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsResponseRequested  <br/> |x  <br/> ||x  <br/> |||
|IsSubmitted  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsUnmodified  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ItemClass  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ItemId  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|JobTitle  <br/> ||x  <br/> ||||
|LastModifiedName  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|LastModifiedTime  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|LastOccurrance  <br/> |x  <br/> |||||
|LegacyFreeBusyStatus  <br/> |x  <br/> |||||
|Location  <br/> |x  <br/> |||||
|Manager  <br/> ||x  <br/> ||||
|MeetingRequestWasSent  <br/> |x  <br/> |||||
|MeetingTimeZone  <br/> |x  <br/> |||||
|MeetingWorkspaceUrl  <br/> |x  <br/> |||||
|MiddleName  <br/> ||x  <br/> ||||
|Mileage  <br/> ||x  <br/> |||x  <br/> |
|ModifiedOccurrances  <br/> |x  <br/> |||||
|MyResponseType  <br/> |x  <br/> |||||
|NetShowUrl  <br/> |x  <br/> |||||
|NickName  <br/> ||x  <br/> ||||
|メモ  <br/> ||x  <br/> ||||
|OfficeLocation  <br/> ||x  <br/> ||||
|OptionalAttendees  <br/> |x  <br/> |||||
|開催者  <br/> |x  <br/> |||||
|OriginalStart  <br/> |x  <br/> |||||
|Owner  <br/> |||||x  <br/> |
|ParentFolderId  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|PercentComplete  <br/> |||||x  <br/> |
|PhoneNumbers  <br/> ||x  <br/> ||||
|PhoneticFirstName  <br/> ||x  <br/> ||||
|PhoneticFullName  <br/> ||x  <br/> ||||
|PhoneticLastName  <br/> ||x  <br/> ||||
|Photo  <br/> ||x  <br/> ||||
|PhysicalAddresses  <br/> ||x  <br/> ||||
|PostalAddressIndex  <br/> ||x  <br/> ||||
|PostedTime  <br/> ||||x  <br/> ||
|Profession  <br/> ||x  <br/> ||||
|ReceivedBy  <br/> |||x  <br/> |||
|ReceivedRepresenting  <br/> |||x  <br/> |||
|Reccurrence  <br/> |x  <br/> ||||x  <br/> |
|参照  <br/> |||x  <br/> |x  <br/> ||
|ReminderDueBy  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ReminderIsSet  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ReminderMinutesBeforeStart  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ReplyTo  <br/> |||x  <br/> |||
|RequiredAttendees  <br/> |x  <br/> |||||
|リソース  <br/> |x  <br/> |||||
|ResponseObjects  <br/> |x(1)  <br/> |x(1)  <br/> |x(1)  <br/> |x(1)  <br/> |x(1)  <br/> |
|Sender  <br/> |||x  <br/> |x  <br/> ||
|Sensitivity  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|サイズ  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|SpouseName  <br/> ||x  <br/> ||||
|開始  <br/> |x  <br/> |||||
|StartDate  <br/> |||||x  <br/> |
|StartTimeZone  <br/> |x  <br/> |||||
|Status  <br/> |||||x  <br/> |
|StatusDescription  <br/> |||||x  <br/> |
|対象  <br/> |x  <br/> |x  <br/> |x  <br/> ||x  <br/> |
|Surname  <br/> ||x  <br/> ||||
|タイム ゾーン  <br/> |x  <br/> |||||
|ToRecipients  <br/> |||x  <br/> |||
|TotalWork  <br/> |||||x  <br/> |
|WebClientEditFormQueryString  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|WebClientReadFormQueryString  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
   
メモ:
  
1. とき含まれている[アイテムへのバインド](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx)および[GetItem 操作](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx)からの応答します。 [Item.FindItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)メソッドまたは[FindItem 操作](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)からの応答の結果に含まれません。
    
## <a name="see-also"></a>関連項目

- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    
- 
  [FindItem 操作](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- 
  [GetItem 操作](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx)
    
- 
  [FindFolder 操作](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- 
  [GetFolder 操作](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)
    

