---
title: NormalizedBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: bfb813e4-642d-4f1b-9e91-1fee89dbd083
description: NormalizedBody 要素は、アイテムの Body プロパティの HTML 表現を、別の HTML 本文に挿入できるフラグメントとして指定します。
ms.openlocfilehash: 9ce7a745cfbe2e08afbe4c83873cb670b6afa571
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515433"
---
# <a name="normalizedbody"></a>NormalizedBody

**NormalizedBody** 要素は、アイテムの **Body** プロパティの HTML 表現を、別の HTML 本文に挿入できるフラグメントとして指定します。 
  
```XML
<NormalizedBody BodyType="Text | HTML" IsTruncated="true | false"></NormalizedBody>
```

 **BodyType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|BodyType  <br/> |本文の種類を示します。 **BodyType** 属性 **の Text** の値は、本文がテキスト形式で表されます。 **BodyType** 属性 **の HTML** の値は、本文が HTML 形式を表します。 **BodyType 属性** が必要です。  <br/> |
|IsTruncated  <br/> |本文の内容が切り詰められることを示します。 **IsTruncated** 属性のテキスト値 **false** は、本文の内容が切り詰められていない状態を示します。 正規化された本文の長さが MaximumBodySize 要素で設定された値よりも長い場合、正規化された本文 [は切り捨](maximumbodysize.md) てされます。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[アイテム](item.md)  | [メッセージ](message-ex15websvcsotherref.md)  | [MeetingMessage](meetingmessage.md)  | [MeetingRequest](meetingrequest.md)  | [MeetingResponse](meetingresponse.md)  | [MeetingCancellation](meetingcancellation.md)  | [タスク](task.md)  | [PostItem](postitem.md)  | [CalendarItem](calendaritem.md)  | [連絡先](contact.md)  | [DistributionList](distributionlist.md)
  
## <a name="text-value"></a>テキスト値

**NormalizedBody 要素のテキスト値** は、アイテムの正規化された本文です。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> ||
   

