---
title: AppointmentState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AppointmentState
api_type:
- schema
ms.assetid: ab3f5d04-ace1-4a15-9107-cefa6c41abc7
description: AppointmentState 要素は、予定の状態を指定します。
ms.openlocfilehash: f984bbd5a1319a6051a3394ed04d56deabbb2c5a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544283"
---
# <a name="appointmentstate"></a>AppointmentState

**AppointmentState 要素** は、予定の状態を指定します。 
  
```XML
<AppointmentState/>
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
|[CalendarItem](calendaritem.md) <br/> |予定表アイテムのExchangeを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |ユーザー ストア内の会議Exchangeします。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素には、セット ビットを表すテキスト値が含まれる。 これは整数形式です。 この要素は読み取り専用です。 応答でのみ返されます。
  
## <a name="remarks"></a>注釈

返される整数値は、予定状態ビットマスクを表します。 次の表に、各ビットについて説明します。
  
|**名前**|**ビット**|**説明**|
|:-----|:-----|:-----|
|なし  <br/> |0x0000  <br/> |フラグが設定されていない。 これは、出席者を含めない予定にのみ使用されます。  <br/> |
|会議  <br/> |0x0001  <br/> |この予定は会議です。  <br/> |
|受信済み  <br/> |0x0002  <br/> |この予定は受信しました。  <br/> |
|キャンセルされました  <br/> |0x0004  <br/> |この予定は取り消されました。  <br/> |
   
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

