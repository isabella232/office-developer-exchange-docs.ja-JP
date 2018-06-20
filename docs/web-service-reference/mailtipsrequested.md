---
title: MailTipsRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsRequested
api_type:
- schema
ms.assetid: 8037bbe5-a37f-4f77-8209-27a94f9095ef
description: MailTipsRequested 要素には、サービスから要求されたメール ヒントの種類が含まれています。
ms.openlocfilehash: fa2bef394ea8473aa65bdc2f1d39c0794186fdc6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832348"
---
# <a name="mailtipsrequested"></a>MailTipsRequested

**MailTipsRequested**要素には、サービスから要求されたメール ヒントの種類が含まれています。 
  
```XML
<MailTipsRequested/>
```

 **MailTipTypes**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetMailTips](getmailtips.md) <br/> |受信者とメール ヒントの種類を取得するのにが含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表は、 **MailTipsRequested**要素の値を一覧します。 
  
|**値**|**説明**|
|:-----|:-----|
|All  <br/> |すべての利用可能なメール ヒントを表します。  <br/> |
|OutOfOfficeMessage  <br/> |Office (OOF) メッセージを表します。  <br/> |
|MailboxFullStatus  <br/> |メールボックスがいっぱいの状態を表します。  <br/> |
|CustomMailTip  <br/> |カスタム メール ヒントを表します。  <br/> |
|ExternalMemberCount  <br/> |外部のメンバーの数を表します。  <br/> |
|TotalMemberCount  <br/> |すべてのメンバーの数を表します。  <br/> |
|MaxMessageSize  <br/> |受信者が受け入れることができるメッセージの最大サイズを表します。  <br/> |
|DeliveryRestriction  <br/> |配信の制限が、送信者のメッセージを防ぐため、受信者に到達できないかどうかを示します。  <br/> |
|ModerationStatus  <br/> |送信者のメッセージはモデレーターによって確認するかどうかを示します。  <br/> |
|InvalidRecipient  <br/> |受信者が有効かどうかを示します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

