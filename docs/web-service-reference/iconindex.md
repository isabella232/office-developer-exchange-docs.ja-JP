---
title: IconIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 92020822-2a86-4dfc-aee1-3067af4d4edf
description: IconIndex 要素は、アイテムまたは会話のアイコン インデックスを識別します。
ms.openlocfilehash: f0c024eeedcbda9aa5ad8afdea09a68f2499798e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541162"
---
# <a name="iconindex"></a>IconIndex

**IconIndex 要素** は、アイテムまたは会話のアイコン インデックスを識別します。 
  
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

[Conversation (ConversationType)](conversation-conversationtype.md)  | [アイテム](item.md)  | [連絡先](contact.md)  | [DistributionList](distributionlist.md)  | [メッセージ](message-ex15websvcsotherref.md)  | [CalendarItem](calendaritem.md)  | [PostItem](postitem.md)  | [タスク](task.md)
  
## <a name="text-value"></a>テキスト値

次の表に、IconIndex 要素に使用できるテキスト **値を示** します。 
  
|**値**|**説明**|
|:-----|:-----|
|||
|既定値  <br/> |既定のアイコンを指定します。  <br/> |
|PostItem  <br/> |投稿アイテムのアイコンを指定します。  <br/> |
|MailRead  <br/> |メール読み取りアイコンを指定します。  <br/> |
|MailUnread  <br/> |未読メール アイコンを指定します。  <br/> |
|MailReplied  <br/> |メール に返信するアイコンを指定します。  <br/> |
|MailForwarded  <br/> |転送されるメール アイコンを指定します。  <br/> |
|MailEncrypted  <br/> |暗号化されたメール アイコンを指定します。  <br/> |
|MailSmimeSigned  <br/> |Secure/Multipurpose インターネット メール拡張機能 (S/MIME) 署名付きメール アイコンを指定します。  <br/> |
|MailEncryptedReplied  <br/> |メール に返信される暗号化されたアイコンを指定します。  <br/> |
|MailSmimeSignedReplied  <br/> |メール に返信される S/MIME 署名済みアイコンを指定します。  <br/> |
|MailEncryptedForwarded  <br/> |暗号化された転送メール アイコンを指定します。  <br/> |
|MailSmimeSignedForwarded  <br/> |S/MIME 署名済み転送メール アイコンを指定します。  <br/> |
|MailEncryptedRead  <br/> |暗号化された読み取りメール アイコンを指定します。  <br/> |
|MailSmimeSignedRead  <br/> |S/MIME 署名済み読み取りメール アイコンを指定します。  <br/> |
|MailIrm  <br/> |Information Rights Management (IRM)で保護されたメール アイコンを指定します。  <br/> |
|MailIrmForwarded  <br/> |IRM で保護された転送メール アイコンを指定します。  <br/> |
|MailIrmReplied  <br/> |メール に返信する IRM で保護されたアイコンを指定します。  <br/> |
|SmsSubmitted  <br/> |ショート メッセージ サービス (SMS) ルーティング用に送信されるアイコン メールを指定します。  <br/> |
|SmsRoutedToDeliveryPoint  <br/> |外部配信ポイントへの SMS ルーティングのアイコンを指定します。  <br/> |
|SmsRoutedToExternalMessagingSystem  <br/> |外部メッセージング システムへの SMS ルーティングのアイコンを指定します。  <br/> |
|SmsDelivered  <br/> |SMS 配信メール アイコンを指定します。  <br/> |
|OutlookDefaultForContacts  <br/> |連絡先の既定のアイコンを指定します。  <br/> |
|AppointmentItem  <br/> |予定アイテムのアイコンを指定します。  <br/> |
|AppointmentRecur  <br/> |定期的な予定アイコンを指定します。  <br/> |
|AppointmentMeet  <br/> |会議アイコンを指定します。  <br/> |
|AppointmentMeetRecur  <br/> |定期的な会議アイコンを指定します。  <br/> |
|AppointmentMeetNY  <br/> |会議への暫定的な応答のアイコンを指定します。  <br/> |
|AppointmentMeetYes  <br/> |会議の承諾アイコンを指定します。  <br/> |
|AppointmentMeetNo  <br/> |会議が拒否されたアイコンを指定します。  <br/> |
|AppointmentMeetMaybe  <br/> |会議への応答のアイコンを指定します。  <br/> |
|AppointmentMeetCancel  <br/> |会議のキャンセル アイコンを指定します。  <br/> |
|AppointmentMeetInfo  <br/> |会議情報アイコンを指定します。  <br/> |
|TaskItem  <br/> |タスク アイテム アイコンを指定します。  <br/> |
|TaskRecur  <br/> |定期的なタスク アイコンを指定します。  <br/> |
|TaskOwned  <br/> |タスクが所有するアイコンを指定します。  <br/> |
|TaskDelegated  <br/> |タスク委任アイコンを指定します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |false  <br/> |
   

