---
title: Exchange のユニファイドメッセージング web サービスの操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Unified
api_type:
- schema
ms.assetid: d92455bd-24e8-4255-9f93-2bdeff00d42d
description: Exchange でのユニファイドメッセージング web サービスの操作に関する参照情報を検索します。
ms.openlocfilehash: b13ca2fbc44846db0bc98b3961916ba5d0872310
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529715"
---
# <a name="unified-messaging-web-service-operations-for-exchange"></a>Exchange のユニファイドメッセージング web サービスの操作

Exchange でのユニファイドメッセージング web サービスの操作に関する参照情報を検索します。
  
ユニファイドメッセージング web サービスは、クライアントアプリケーションが、ユニファイドメッセージングのプロパティの読み取りおよび変更、ボイスメールメッセージの再生、案内応答の再生、およびテレフォニーデバイスを介したメールボックスアイテムのディクテーションを行えるようにする多くの操作を提供します。 このセクションの記事では、要求の全体的な構造と、操作に対する応答メッセージについて説明します。 これらの記事には、一般的なメッセージ構造を示す例が用意されています。 これらの例を使用して、ユニファイドメッセージング web サービス要求に対して実行できる操作について理解することができます。
  
> [!NOTE]
> Exchange 2010 以降のバージョンの Exchange では、次の理由から、ユニファイドメッセージング Web サービスの代わりに[Exchange Web サービス (EWS)](https://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx)で使用できるユニファイドメッセージング操作を使用することをお勧めします。 
> - Ews ベースのユニファイドメッセージング機能には、EWS マネージ API でのファーストクラスのサポートが含まれています。 
> - Exchange 2010 以降のバージョンの Exchange では、新しいユニファイドメッセージング機能は EWS に追加されますが、ユニファイドメッセージング web サービスには追加されません。 
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_InThisSection"> </a>

- [Disconnect 操作 (UM web サービス)](disconnect-operation-um-web-service.md)    
- [GetCallInfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)   
- [GetUMProperties 操作 (UM web サービス)](getumproperties-operation-um-web-service.md)   
- [IsUMEnabled 操作 (UM web サービス)](isumenabled-operation-um-web-service.md)   
- [PlayOnPhone 操作 (UM web サービス)](playonphone-operation-um-web-service.md)   
- [Playon電話案内応答操作 (UM web サービス)](playonphonegreeting-operation-um-web-service.md)   
- [ResetPIN 操作 (UM web サービス)](resetpin-operation-um-web-service.md)   
- [SetMissedCallNotificationEnabled 操作 (UM web サービス)](setmissedcallnotificationenabled-operation-um-web-service.md)  
- [SetOofStatus 操作 (UM web サービス)](setoofstatus-operation-um-web-service.md)    
- [SetPlayOnPhoneDialString 操作 (UM web サービス)](setplayonphonedialstring-operation-um-web-service.md)   
- [SetTelephoneAccessFolderEmail 操作 (UM web サービス)](settelephoneaccessfolderemail-operation-um-web-service.md)
    
## <a name="see-also"></a>関連項目

- [Exchange 用ユニファイドメッセージング web サービスのリファレンス](unified-messaging-web-service-reference-for-exchange.md)
- [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)
- [Exchange で Web サービスの使用を開始する](../exchange-web-services/start-using-web-services-in-exchange.md)
    

