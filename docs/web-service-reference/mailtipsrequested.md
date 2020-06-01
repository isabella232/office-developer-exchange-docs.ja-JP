---
title: Mailヒント要求
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
description: Mailヒント要求要素には、サービスから要求されたメールヒントの種類が含まれています。
ms.openlocfilehash: bcb2ebf15e628a04e8507f938d385cf113f2f2a3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465899"
---
# <a name="mailtipsrequested"></a>Mailヒント要求

**Mailヒント要求**要素には、サービスから要求されたメールヒントの種類が含まれています。 
  
```XML
<MailTipsRequested/>
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
|[GetMailTips](getmailtips.md) <br/> |取得するメールヒントの受信者と種類が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に、 **Mailヒントの要求さ**れた要素に使用できる値を示します。 
  
|**値**|**説明**|
|:-----|:-----|
|すべて  <br/> |利用可能なすべてのメールヒントを表します。  <br/> |
|OutOfOfficeMessage  <br/> |不在 (OOF) メッセージを表します。  <br/> |
|MailboxFullStatus  <br/> |フルのメールボックスの状態を表します。  <br/> |
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
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

