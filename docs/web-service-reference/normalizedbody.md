---
title: NormalizedBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfb813e4-642d-4f1b-9e91-1fee89dbd083
description: NormalizedBody 要素は、別の HTML 本文に挿入できるフラグメントとしてアイテムの Body プロパティの HTML 表記を指定します。
ms.openlocfilehash: 07c2176d2c8a7473c06b7e42f8bcbbe6670581ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832548"
---
# <a name="normalizedbody"></a>NormalizedBody

**NormalizedBody**要素は、別の HTML 本文に挿入できるフラグメントとしてアイテムの**Body**プロパティの HTML 表記を指定します。 
  
```XML
<NormalizedBody BodyType="Text | HTML" IsTruncated="true | false"></NormalizedBody>
```

 **BodyType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|BodyType  <br/> |本文の種類を示します。 **BodyType**属性の**テキスト**の値は、プレーン テキスト形式の本文であることを示します。 **BodyType**属性の**HTML**の値は、本文が HTML 形式でことを示します。 **BodyType**属性は、必要があります。  <br/> |
|IsTruncated  <br/> |本文の内容が切り詰められたことを示します。 テキスト値が**false**の**IsTruncated**属性のでは、本文の内容は切り捨てられましたしないことを示します。 正規化された本文は[MaximumBodySize](maximumbodysize.md)要素で設定した値よりも長い場合は、正規化された本文の長さに切り詰められます。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[項目](item.md) | [メッセージ](message-ex15websvcsotherref.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [作業](task.md) | [PostItem](postitem.md)  | [カレンダー項目](calendaritem.md) | [連絡先](contact.md) | [DistributionList](distributionlist.md)
  
## <a name="text-value"></a>テキスト値

**NormalizedBody**要素のテキスト値は、項目の正規化の本体です。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> ||
   

