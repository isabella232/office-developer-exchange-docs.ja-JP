---
title: NormalizedBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfb813e4-642d-4f1b-9e91-1fee89dbd083
description: NormalizedBody 要素は、別の HTML 本文に挿入できるフラグメントとして、アイテムの Body プロパティの HTML 表記を指定します。
ms.openlocfilehash: fb249794bccfeed198e7a3230ab53c66893dcf96
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462669"
---
# <a name="normalizedbody"></a>NormalizedBody

**Normalizedbody**要素は、別の html 本文に挿入できるフラグメントとして、アイテムの**BODY**プロパティの HTML 表記を指定します。 
  
```XML
<NormalizedBody BodyType="Text | HTML" IsTruncated="true | false"></NormalizedBody>
```

 **BodyType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|BodyType  <br/> |本文の種類を示します。 **Bodytype**属性の**テキスト**の値は、本文がプレーンテキスト形式であることを示します。 **Bodytype**属性の**html**の値は、本文が HTML 形式であることを示します。 **Bodytype**属性は必須です。  <br/> |
|Istrがありません  <br/> |本文の内容が切り捨てられていることを示します。 **Istruncated** attribute のテキスト値が**false**の場合は、本文のコンテンツが切り捨てられていないことを示します。 正規化された本文の長さが、 [Maximumbodysize](maximumbodysize.md)要素で設定された値よりも長い場合は、正規化された本文は切り捨てられます。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[アイテム](item.md)  | [メッセージ](message-ex15websvcsotherref.md)  | [会議メッセージ](meetingmessage.md)  | [会議の要求](meetingrequest.md)  | [会議の応答](meetingresponse.md)  | [会議のキャンセル](meetingcancellation.md)  | [タスク](task.md)  | [Postitem](postitem.md)  | [Calendaritem](calendaritem.md)  | [連絡先](contact.md)  | [DistributionList](distributionlist.md)
  
## <a name="text-value"></a>テキスト値

**Normalizedbody**要素のテキスト値は、アイテムの正規化された本文です。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   

