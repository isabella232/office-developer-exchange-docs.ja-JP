---
title: IconIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 92020822-2a86-4dfc-aee1-3067af4d4edf
description: IconIndex 要素は、アイテムまたはスレッドのアイコンインデックスを識別します。
ms.openlocfilehash: 0f932f5632422a8786e74500bf83cb1337f780c3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460786"
---
# <a name="iconindex"></a>IconIndex

**IconIndex**要素は、アイテムまたはスレッドのアイコンインデックスを識別します。 
  
```XML
<IconIndex>Default | PostItem | MailRead | MailUnread | MailReplied | MailForwarded | MailEncrypted | MailSmimeSigned | MailEncrytedReplied | MailSmimeSignedReplied | MailEncryptedForwarded | MailSmimeSignedForwarded | MailEncryptedRead | MailSmimeSignedRead | MailIrm | MailIrmForwarded | MailIrmReplied | SmsSubmitted | SmsRoutedToDeliveryPoint | SmsRoutedToExternalMessagingSystem | SmsDelivered | OutlookDefaultForContacts | AppointmentItem | AppointmentRecur | AppointmentMeet | AppointmentMeetRecur | AppointmentMeetNY | AppointmentMeetYes | AppointmentMeetNo | AppointmentMeetMaybe | AppointmentMeetCancel | AppointmentMeetInfo | TaskItem | TaskRecur | TaskOwned | TaskDelegated</IconIndex>
```

 **IconIndexType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[会話 (ConversationType)](conversation-conversationtype.md)  | [アイテム](item.md)  | [連絡先](contact.md)  | [DistributionList](distributionlist.md)  | [メッセージ](message-ex15websvcsotherref.md)  | [Calendaritem](calendaritem.md)  | [Postitem](postitem.md)  | [タスク](task.md)
  
## <a name="text-value"></a>テキスト値

次の表に、 **IconIndex**要素に使用できるテキスト値を示します。 
  
|**値**|**説明**|
|:-----|:-----|
|||
|既定  <br/> |既定のアイコンを指定します。  <br/> |
|PostItem  <br/> |投稿アイテムのアイコンを指定します。  <br/> |
|MailRead  <br/> |[メールの閲覧] アイコンを指定します。  <br/> |
|メール未開封  <br/> |[未読のメール] アイコンを指定します。  <br/> |
|メール返信  <br/> |[返信済みメール] アイコンを指定します。  <br/> |
|メール転送  <br/> |[転送されたメール] アイコンを指定します。  <br/> |
|MailEncrypted  <br/> |暗号化されたメールのアイコンを指定します。  <br/> |
|MailSmimeSigned  <br/> |[セキュリティで保護されたマルチパーパスインターネットメール内線 (S/MIME) 署名済みメール] アイコンを指定します。  <br/> |
|MailEncryptedReplied  <br/> |[暗号化された返信メール] アイコンを指定します。  <br/> |
|MailSmimeSignedReplied  <br/> |S/MIME で署名された返信メールアイコンを指定します。  <br/> |
|MailEncryptedForwarded  <br/> |[暗号化された転送メール] アイコンを指定します。  <br/> |
|MailSmimeSignedForwarded  <br/> |S/MIME で署名された転送メールアイコンを指定します。  <br/> |
|MailEncryptedRead  <br/> |[暗号化されたメールの開封] アイコンを指定します。  <br/> |
|MailSmimeSignedRead  <br/> |S/MIME で署名されたメールの開封アイコンを指定します。  <br/> |
|MailIrm  <br/> |Information Rights Management (IRM) で保護されたメールのアイコンを指定します。  <br/> |
|MailIrmForwarded  <br/> |IRM で保護された転送されたメールのアイコンを指定します。  <br/> |
|MailIrmReplied  <br/> |[IRM で保護された返信メール] アイコンを指定します。  <br/> |
|SmsSubmitted  <br/> |ショートメッセージサービス (SMS) ルーティングに送信されるメールのアイコンを指定します。  <br/> |
|Smsルーブル Tedtodeliverypoint  <br/> |外部配信ポイントへの SMS ルーティングのアイコンを指定します。  <br/> |
|Smsルーブル Tedtoexternalmessagingsystem  <br/> |外部メッセージングシステムへの SMS ルーティングのアイコンを指定します。  <br/> |
|SmsDelivered  <br/> |[SMS 配信メール] アイコンを指定します。  <br/> |
|OutlookDefaultForContacts  <br/> |連絡先の既定のアイコンを指定します。  <br/> |
|AppointmentItem  <br/> |予定アイテムアイコンを指定します。  <br/> |
|AppointmentRecur  <br/> |定期的な予定のアイコンを指定します。  <br/> |
|AppointmentMeet  <br/> |会議アイコンを指定します。  <br/> |
|AppointmentMeetRecur  <br/> |[定期的な会議] アイコンを指定します。  <br/> |
|AppointmentMeetNY  <br/> |会議への仮承諾応答のアイコンを指定します。  <br/> |
|AppointmentMeetYes  <br/> |[会議の承諾] アイコンを指定します。  <br/> |
|AppointmentMeetNo  <br/> |会議の辞退アイコンを指定します。  <br/> |
|AppointmentMeetMaybe  <br/> |会議への応答の可能性があるアイコンを指定します。  <br/> |
|AppointmentMeetCancel  <br/> |会議のキャンセルアイコンを指定します。  <br/> |
|AppointmentMeetInfo  <br/> |[ミーティング情報] アイコンを指定します。  <br/> |
|TaskItem  <br/> |タスクアイテムアイコンを指定します。  <br/> |
|TaskRecur  <br/> |[定期タスク] アイコンを指定します。  <br/> |
|TaskOwned 者  <br/> |タスクの所有者アイコンを指定します。  <br/> |
|TaskDelegated  <br/> |タスクの委任アイコンを指定します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

