---
title: ProposedStart (MeetingRegistrationResponseObjectType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8c58cef7-bc43-493a-a323-ba4dc6a33704
description: ProposedStart (MeetingRegistrationResponseObjectType) の要素では、出席者の提案された新しい開始会議の時間を指定します。
ms.openlocfilehash: db03d1b5e79ed53313cff9677687647f24e90756
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832905"
---
# <a name="proposedstart-meetingregistrationresponseobjecttype"></a>ProposedStart (MeetingRegistrationResponseObjectType)

**ProposedStart (MeetingRegistrationResponseObjectType)** の要素では、出席者の提案された新しい開始会議の時間を指定します。 
  
```XML
<ProposedStart />
```

 **dateTime**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[AcceptItem](acceptitem.md) | [TentativelyAcceptItem](tentativelyacceptitem.md) | [DeclineItem](declineitem.md)
  
## <a name="text-value"></a>テキスト値

**ProposedStart (MeetingRegistrationResponseObjectType)** の要素のテキスト値とは、提案された開始日と会議の時刻です。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[AcceptItem](acceptitem.md)
  
[DeclineItem](declineitem.md)
  
[TentativelyAcceptItem](tentativelyacceptitem.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

