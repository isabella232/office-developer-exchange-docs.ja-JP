---
title: GetItem 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: e3590b8b-c2a7-4dad-a014-6360197b68e4
description: 操作 GetItem EWS についての情報を検索します。
ms.openlocfilehash: 9b63032b2eaa3bf26027a42e38bfa06bedcbac86
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760776"
---
# <a name="getitem-operation"></a>GetItem 操作

**GetItem** EWS の操作に関する情報を検索します。 
  
**GetItem**操作は、Exchange ストアから項目を取得します。 
  
## <a name="using-the-getitem-operation"></a>GetItem 操作を使用します。

**GetItem**操作は、多くのアイテムのプロパティを返します。 **GetItem**応答で返されるプロパティによって要求された図形を要求された追加のプロパティと項目の型が返されます。 
  
[メッセージ](message-ex15websvcsotherref.md)要素は、電子メール メッセージ、Exchange Web サービス (EWS) スキーマが厳密に型指定されない他のすべての項目を表します。 IPM などの項目です。共有し、IPM.InfoPath は、[メッセージ](message-ex15websvcsotherref.md)の要素として返されます。 Exchange では、応答の基本要素の[項目](item.md)が返されません。 
  
**GetItem**操作では、添付ファイルは返されません。 添付されたアイテムやファイルについてのメタデータを返すには。 添付ファイルを取得するには、 [GetAttachment 操作](getattachment-operation.md)を使用します。
  
## <a name="getitem-operation-soap-headers"></a>GetItem 操作の SOAP ヘッダー

**GetItem**操作は、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|ヘッダー。|****Element****|****説明****|
|:-----|:-----|:-----|
|**DateTimePrecision** <br/> |[DateTimePrecision](datetimeprecision.md) <br/> |秒またはミリ秒単位のいずれか、サーバーからの応答では、日付/時刻値の解像度を指定します。  <br/> |
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装するユーザーを識別します。  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマのバージョンを識別します。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。  <br/> |
|**TimeZoneContext** <br/> |[TimeZoneContext](timezonecontext.md) <br/> |サーバーからのすべての応答に使用するタイム ゾーンを識別します。  <br/> |
   
## <a name="in-this-section"></a>���̃Z�N�V�����̓�e

[GetItem 操作 (電子メール)](getitem-operation-email-message.md)
  
[GetItem 操作 (予定表アイテム)](getitem-operation-calendar-item.md)
  
[GetItem 操作 (タスク)](getitem-operation-task.md)
  
[GetItem 操作 (連絡先)](getitem-operation-contact.md)
  
## <a name="see-also"></a>関連項目




  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)

