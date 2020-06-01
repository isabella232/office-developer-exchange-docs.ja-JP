---
title: IsCancelled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsCancelled
api_type:
- schema
ms.assetid: 50c1e97f-2913-47a1-8457-60428a3c5b92
description: IsCancelled 要素は、予定または会議がキャンセルされたかどうかを示します。
ms.openlocfilehash: 946c9d956da9cf31e9fa08d4ab6f4950b11214b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455570"
---
# <a name="iscancelled"></a>IsCancelled

**Iscancelled**要素は、予定または会議がキャンセルされたかどうかを示します。 
  
```xml
<IsCancelled/>
```

 **Boolean**
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
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素が含まれている場合は、ブール値を表すテキスト値が必要です。 **True**の値は、予定表アイテムが取り消されたことを示します。 値が**false**の場合、予定表アイテムが取り消されていないことを示します。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

