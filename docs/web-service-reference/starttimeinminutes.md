---
title: StartTimeInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartTimeInMinutes
api_type:
- schema
ms.assetid: 0fb60a78-6e79-4601-8e2f-5bd245c46d69
description: StartTimeInMinutes 要素は、メールボックスユーザーの稼働日の開始を表します。
ms.openlocfilehash: b33cb12299a146b577dd17939a0585a15d50fb07
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458531"
---
# <a name="starttimeinminutes"></a>StartTimeInMinutes

**StartTimeInMinutes**要素は、メールボックスユーザーの稼働日の開始を表します。 
  
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
- [FreeBusyResponseArray](freebusyresponsearray.md)
  
- [FreeBusyResponse](freebusyresponse.md)
  
- [FreeBusyView](freebusyview.md)
  
- [WorkingHours](workinghours-ex15websvcsotherref.md)
  
- [WorkingPeriodArray](workingperiodarray.md)
  
- [WorkingPeriod](workingperiod.md)
  
- [StartTimeInMinutes](starttimeinminutes.md)
  
```xml
<StartTimeInMinutes>...</StartTimeInMinutes>
```

**int**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[WorkingPeriod](workingperiod.md) <br/> |メールボックスユーザーの勤務週の曜日と時間を含みます。  <br/> この要素の XPath 式を次に示します。  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値は、1日から開始してからの経過時間 (分単位) による稼働日の開始を表します。 たとえば、開始時刻の午前8時 は480分で表されます。
  
この要素で使用できる値の範囲は 0 ~ 1440 です。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserAvailability 操作](getuseravailability-operation.md)
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
- [ユーザーの空き時間情報の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

