---
title: CalendarItemType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarItemType
api_type:
- schema
ms.assetid: 1feb0788-adf7-4a7c-830c-005214ad930f
description: CalendarItemType 要素は、予定表アイテムの種類を表します。
ms.openlocfilehash: 3fe95c86ea24e6dfeb4740ead5e787bd63b5190d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759589"
---
# <a name="calendaritemtype"></a>CalendarItemType

**CalendarItemType**要素は、予定表アイテムの種類を表します。 
  
```xml
<CalendarItemType/>
```

 **CalendarItemTypeType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[カレンダー項目](calendaritem.md) <br/> |Exchange 予定表アイテムを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、この要素が使用される場合に必要です。 以下は、この要素の有効な値です。
  
- **1 つ**アイテムが定期的な予定表アイテムに関連付けられているではありません。 
    
- **出現**アイテムは、定期的な予定表アイテムの発生です。 
    
- **例外**アイテムは、定期的な予定表アイテムの例外です。 
    
- **RecurringMaster**アイテムは、一連の定期的な予定表アイテムのマスターです。 
    
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

