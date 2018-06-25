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
ms.openlocfilehash: 05e92a3fea10a84518b0680c425011a91bc43d93
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759422"
---
# <a name="appointmentstate"></a>AppointmentState

**AppointmentState**要素は、予定の状態を指定します。 
  
```XML
<AppointmentState/>
```

 **int**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[カレンダー項目](calendaritem.md) <br/> |Exchange 予定表アイテムを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を表しますが、ビットを設定するテキスト値が含まれています。 これは整数です。 この要素は、読み取り専用です。 応答でのみ返されます。
  
## <a name="remarks"></a>備考

返される整数値では、予定の状態ビットマスクを表します。 次の表では、各ビットについて説明します。
  
|**名前**|**ビット**|**説明**|
|:-----|:-----|:-----|
|なし  <br/> |0x0000  <br/> |フラグが設定されていません。 出席者が含まれていない予定の場合にだけ使用します。  <br/> |
|会議  <br/> |0x0001  <br/> |この予定は会議です。  <br/> |
|Received  <br/> |0x0002  <br/> |この予定を受信しました。  <br/> |
|キャンセル済み  <br/> |0x0004  <br/> |この予定は取り消されました。  <br/> |
   
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

