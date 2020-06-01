---
title: ProposedStart (会議 Registrationresponseobjecttype)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8c58cef7-bc43-493a-a323-ba4dc6a33704
description: ProposedStart (meeting Registrationresponseobjecttype) 要素は、会議の出席者が提案した新しい開始時刻を指定します。
ms.openlocfilehash: 6f105556c39fa6549b3bec2f7a6fee50d4049358
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465591"
---
# <a name="proposedstart-meetingregistrationresponseobjecttype"></a>ProposedStart (会議 Registrationresponseobjecttype)

**ProposedStart (Meeting Registrationresponseobjecttype)** 要素は、会議の出席者が提案した新しい開始時刻を指定します。 
  
```XML
<ProposedStart />
```

 **dateTime**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[Acceptitem](acceptitem.md)  | [TentativelyAcceptItem](tentativelyacceptitem.md)  | [Declineitem](declineitem.md)
  
## <a name="text-value"></a>テキスト値

**ProposedStart (Meeting Registrationresponseobjecttype)** 要素のテキスト値は、提案された開始日時 (会議の開始日時) です。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[AcceptItem](acceptitem.md)
  
[DeclineItem](declineitem.md)
  
[TentativelyAcceptItem](tentativelyacceptitem.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

