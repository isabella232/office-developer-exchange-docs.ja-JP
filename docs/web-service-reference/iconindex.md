---
title: IconIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 92020822-2a86-4dfc-aee1-3067af4d4edf
description: IconIndex 要素は、アイテムまたは会話のアイコンのインデックスを識別します。
ms.openlocfilehash: 8ada9da2df1cf128009c9b153736b434925f1a3f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831848"
---
# <a name="iconindex"></a>IconIndex

**IconIndex**要素は、アイテムまたは会話のアイコンのインデックスを識別します。 
  
```XML
<IconIndex>Default | PostItem | MailRead | MailUnread | MailReplied | MailForwarded | MailEncrypted | MailSmimeSigned | MailEncrytedReplied | MailSmimeSignedReplied | MailEncryptedForwarded | MailSmimeSignedForwarded | MailEncryptedRead | MailSmimeSignedRead | MailIrm | MailIrmForwarded | MailIrmReplied | SmsSubmitted | SmsRoutedToDeliveryPoint | SmsRoutedToExternalMessagingSystem | SmsDelivered | OutlookDefaultForContacts | AppointmentItem | AppointmentRecur | AppointmentMeet | AppointmentMeetRecur | AppointmentMeetNY | AppointmentMeetYes | AppointmentMeetNo | AppointmentMeetMaybe | AppointmentMeetCancel | AppointmentMeetInfo | TaskItem | TaskRecur | TaskOwned | TaskDelegated</IconIndex>
```

 **IconIndexType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[会話 (ConversationType)](conversation-conversationtype.md) | [アイテム](item.md) | [連絡先](contact.md) | [DistributionList](distributionlist.md) | [メッセージ](message-ex15websvcsotherref.md) | [カレンダー項目](calendaritem.md) | [PostItem](postitem.md) | [タスク](task.md)
  
## <a name="text-value"></a>テキスト値

次の表には、 **IconIndex**要素の可能なテキスト値が含まれています。 
  
|**値**|**説明**|
|:-----|:-----|
|||
|Default  <br/> |既定のアイコンを指定します。  <br/> |
|PostItem  <br/> |投稿アイテムのアイコンを指定します。  <br/> |
|MailRead  <br/> |開封済みのメールを指定します。  <br/> |
|MailUnread  <br/> |未読のメールのアイコンを指定します。  <br/> |
|MailReplied  <br/> |[メール] アイコンに、返信を指定します。  <br/> |
|MailForwarded  <br/> |転送されたメールのアイコンを指定します。  <br/> |
|MailEncrypted  <br/> |暗号化されたメール] アイコンを指定します。  <br/> |
|MailSmimeSigned  <br/> |/Multipurpose をセキュリティで保護されたインターネット メール拡張 (S/MIME) 署名されたメールのアイコンを指定します。  <br/> |
|MailEncryptedReplied  <br/> |[メール] アイコンを暗号化された応答を指定します。  <br/> |
|MailSmimeSignedReplied  <br/> |秒/MIME 署名返信メールのアイコンを指定します。  <br/> |
|MailEncryptedForwarded  <br/> |暗号化された転送されたメール] アイコンを指定します。  <br/> |
|MailSmimeSignedForwarded  <br/> |S/MIME 署名されたメール] アイコンを転送するかを指定します。  <br/> |
|MailEncryptedRead  <br/> |暗号化された読み取りメール] アイコンを指定します。  <br/> |
|MailSmimeSignedRead  <br/> |メール開封済みの S/MIME 署名を指定します。  <br/> |
|MailIrm  <br/> |情報権利管理の IRM で保護されたメール] アイコンを指定します。  <br/> |
|MailIrmForwarded  <br/> |[メール] アイコンを転送された IRM で保護されたを指定します。  <br/> |
|MailIrmReplied  <br/> |返信 IRM で保護されたメール] アイコンを指定します。  <br/> |
|SmsSubmitted  <br/> |ショート メッセージ サービス (SMS) のルーティングのために送信] アイコンのメールを指定します。  <br/> |
|SmsRoutedToDeliveryPoint  <br/> |SMS が外部の配信ポイントにルーティングするためのアイコンを指定します。  <br/> |
|SmsRoutedToExternalMessagingSystem  <br/> |SMS が外部のメッセージング システムにルーティングするためのアイコンを指定します。  <br/> |
|SmsDelivered  <br/> |SMS 配信されたメールのアイコンを指定します。  <br/> |
|OutlookDefaultForContacts  <br/> |連絡先の既定のアイコンを指定します。  <br/> |
|AppointmentItem  <br/> |予定項目のアイコンを指定します。  <br/> |
|AppointmentRecur  <br/> |定期的な予定のアイコンを指定します。  <br/> |
|AppointmentMeet  <br/> |会議アイコンを指定します。  <br/> |
|AppointmentMeetRecur  <br/> |定期的な会議のアイコンを指定します。  <br/> |
|AppointmentMeetNY  <br/> |会議への暫定的な応答のアイコンを指定します。  <br/> |
|AppointmentMeetYes  <br/> |会議の指定承認アイコンです。  <br/> |
|AppointmentMeetNo  <br/> |会議の辞退したアイコンを指定します。  <br/> |
|AppointmentMeetMaybe  <br/> |会議にも応答のアイコンを指定します。  <br/> |
|AppointmentMeetCancel  <br/> |会議キャンセルのアイコンを指定します。  <br/> |
|AppointmentMeetInfo  <br/> |会議を指定する情報のアイコンです。  <br/> |
|TaskItem  <br/> |作業項目のアイコンを指定します。  <br/> |
|TaskRecur  <br/> |定期的なタスクのアイコンを指定します。  <br/> |
|TaskOwned  <br/> |アイコンを所有するタスクを指定します。  <br/> |
|TaskDelegated  <br/> |委任されたタスクのアイコンを指定します。  <br/> |
   
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

