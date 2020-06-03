---
title: GetItem 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- GetItem
api_type:
- schema
ms.assetid: e3590b8b-c2a7-4dad-a014-6360197b68e4
description: GetItem EWS 操作に関する情報を検索します。
localization_priority: Priority
ms.openlocfilehash: 8871dde183974454fc27dbddda489e6b0a70f3aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463329"
---
# <a name="getitem-operation"></a>GetItem 操作

**GetItem** EWS 操作に関する情報を検索します。 
  
**GetItem**操作は、Exchange ストアからアイテムを取得します。 
  
## <a name="using-the-getitem-operation"></a>GetItem 操作の使用

**GetItem**操作は、多くのアイテムプロパティを返します。 **GetItem**応答で返されるプロパティは、要求された図形、要求された追加プロパティ、および返されるアイテムの種類によって異なります。 
  
[Message](message-ex15websvcsotherref.md)要素は、電子メールメッセージと、Exchange Web サービス (EWS) スキーマで厳密に型指定されていないその他すべてのアイテムを表します。 IPM などのアイテム。共有と IPM. InfoPath は、[メッセージ](message-ex15websvcsotherref.md)要素として返されます。 Exchange は、応答で基本[Item](item.md)要素を返しません。 
  
**GetItem**操作では、添付ファイルは返されません。 添付されているアイテムまたはファイルに関するメタデータを返します。 添付ファイルを取得するには、 [getattachment 操作](getattachment-operation.md)を使用します。
  
## <a name="getitem-operation-soap-headers"></a>GetItem 操作 SOAP ヘッダー

**GetItem**操作では、次の表に示す SOAP ヘッダーを使用できます。 
  
|ヘッダー * * * *|****Element****|****説明****|
|:-----|:-----|:-----|
|**DateTimePrecision** <br/> |[DateTimePrecision](datetimeprecision.md) <br/> |サーバーからの応答におけるデータ/時刻値の解決方法を秒単位で指定します。またはミリ秒単位で指定します。  <br/> |
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアントアプリケーションが偽装しているユーザーを識別します。  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマバージョンを識別します。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。  <br/> |
|**TimeZoneContext** <br/> |[TimeZoneContext](timezonecontext.md) <br/> |サーバーからのすべての応答に使用するタイムゾーンを指定します。  <br/> |
   
## <a name="in-this-section"></a>このセクションの内容

[GetItem 操作 (電子メールメッセージ)](getitem-operation-email-message.md)
  
[GetItem 操作 (予定表アイテム)](getitem-operation-calendar-item.md)
  
[GetItem 操作 (タスク)](getitem-operation-task.md)
  
[GetItem 操作 (連絡先)](getitem-operation-contact.md)
  
## <a name="see-also"></a>関連項目



[Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)

