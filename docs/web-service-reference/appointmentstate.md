---
title: AppointmentState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AppointmentState
api_type:
- schema
ms.assetid: ab3f5d04-ace1-4a15-9107-cefa6c41abc7
description: AppointmentState 要素は、予定の状態を指定します。
ms.openlocfilehash: 8b0e827d02e9051f31d43199503dc286c50e2125
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463476"
---
# <a name="appointmentstate"></a>AppointmentState

**AppointmentState**要素は、予定の状態を指定します。 
  
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
|[CalendarItem](calendaritem.md) <br/> |Exchange の予定表アイテムを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素には、セットビットを表すテキスト値が含まれています。 これは整数形式です。 この要素は値の取得のみ可能です。 応答でのみ返されます。
  
## <a name="remarks"></a>注釈

返される整数値は、予定の状態ビットマスクを表します。 次の表で、各ビットについて説明します。
  
|**名前**|**若干**|**説明**|
|:-----|:-----|:-----|
|なし  <br/> |0x0000  <br/> |フラグが設定されていません。 これは、出席者が含まれていない予定に対してのみ使用されます。  <br/> |
|会議  <br/> |0x0001  <br/> |この予定は会議です。  <br/> |
|受信済み  <br/> |0x0002  <br/> |この予定を受信しました。  <br/> |
|キャンセル済み  <br/> |0x0004  <br/> |この予定はキャンセルされました。  <br/> |
   
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

