---
title: PendingMailTips ヒント
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PendingMailTips
api_type:
- schema
ms.assetid: 0cd70eea-8d36-4b1b-bf80-5edf359e7ba7
description: PendingMailTips ヒント要素は、サーバーの処理タイムアウトが経過する前に、この要素のメールヒントを評価できなかったことを示します。
ms.openlocfilehash: 715d68b367c3b7251c7406c10c1ec52dcd992a59
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529967"
---
# <a name="pendingmailtips"></a>PendingMailTips ヒント

**Pendingmailtips**ヒント要素は、サーバーの処理タイムアウトが経過する前に、この要素のメールヒントを評価できなかったことを示します。 
  
```XML
<PendingMailTips>All | OutOfOfficeMessage | MailboxFullStatus | CustomMailTip | ExternalMemberCount | TotalMemberCount | MaxMessageSize | DeliveryRestriction | ModerateStatus | InvalidRecipient</PendingMailTips>
```

 **Mailヒントの種類**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[メールヒント](mailtips.md) <br/> |さまざまな種類のメールヒントの値を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に、 **Pendingmailtips ヒント**要素に指定できる値を示します。 
  
|**値**|**説明**|
|:-----|:-----|
|すべて  <br/> |利用可能なすべてのメールヒントを表します。  <br/> |
|OutOfOfficeMessage  <br/> |不在 (OOF) メッセージを表します。  <br/> |
|MailboxFullStatus  <br/> |メールボックスがいっぱいになったときの状態を表します。  <br/> |
|CustomMailTip  <br/> |ユーザー設定のメールヒントを表します。  <br/> |
|ExternalMemberCount  <br/> |外部メンバーの数を表します。  <br/> |
|TotalMemberCount  <br/> |すべてのメンバーの数を表します。  <br/> |
|MaxMessageSize  <br/> |受信者が受け付けることができる最大メッセージサイズを表します。  <br/> |
|DeliveryRestriction  <br/> |配信の制限によって、送信者のメッセージが受信者に届かないようにするかどうかを示します。  <br/> |
|ModerationStatus  <br/> |送信者のメッセージがモデレーターによって確認されるかどうかを示します。  <br/> |
|InvalidRecipient  <br/> |受信者が無効かどうかを示します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

