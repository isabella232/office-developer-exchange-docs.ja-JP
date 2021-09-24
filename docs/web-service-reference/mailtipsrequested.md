---
title: MailTipsRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MailTipsRequested
api_type:
- schema
ms.assetid: 8037bbe5-a37f-4f77-8209-27a94f9095ef
description: MailTipsRequested 要素には、サービスから要求されたメール ヒントの種類が含まれる。
ms.openlocfilehash: 14a463d3b00a9f8b3e2aa2e822209ff87a221f9b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524855"
---
# <a name="mailtipsrequested"></a>MailTipsRequested

**MailTipsRequested 要素** には、サービスから要求されたメール ヒントの種類が含まれる。 
  
```XML
<MailTipsRequested/>
```

 **MailTipTypes**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetMailTips](getmailtips.md) <br/> |取得する受信者とメール ヒントの種類が含まれる。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に **、MailTipsRequested 要素に使用できる値を示** します。 
  
|**値**|**説明**|
|:-----|:-----|
|すべて  <br/> |使用可能なすべてのメール ヒントを表します。  <br/> |
|OutOfOfficeMessage  <br/> |[アウト オブ Office ( OOF) メッセージを表します。  <br/> |
|MailboxFullStatus  <br/> |完全なメールボックスの状態を表します。  <br/> |
|CustomMailTip  <br/> |カスタム メール ヒントを表します。  <br/> |
|ExternalMemberCount  <br/> |外部メンバーの数を表します。  <br/> |
|TotalMemberCount  <br/> |すべてのメンバーの数を表します。  <br/> |
|MaxMessageSize  <br/> |受信者が受け入れ可能な最大メッセージ サイズを表します。  <br/> |
|DeliveryRestriction  <br/> |配信の制限によって、送信者のメッセージが受信者に届かないかどうかを示します。  <br/> |
|ModerationStatus  <br/> |送信者のメッセージをモデレーターが確認するかどうかを示します。  <br/> |
|InvalidRecipient  <br/> |受信者が無効かどうかを示します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

