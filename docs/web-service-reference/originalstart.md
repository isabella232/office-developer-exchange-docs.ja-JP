---
title: OriginalStart
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OriginalStart
api_type:
- schema
ms.assetid: 4599dd34-15ee-4d57-b886-732081b50784
description: OriginalStart 要素は、予定表アイテムの元の開始時刻を表します。
ms.openlocfilehash: 9e5facb3df87ab08e05f23258abdf1767fae64e4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832668"
---
# <a name="originalstart"></a>OriginalStart

**OriginalStart**要素は、予定表アイテムの元の開始時刻を表します。 
  
```xml
<OriginalStart/>
```

 **DateTime**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[カレンダー項目](calendaritem.md) <br/> |Exchange ストア内の予定表アイテムを表します。  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |定期的な予定表アイテムが最初に見つかった位置を表します。  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |定期的な予定表アイテムが最後に見つかった位置を表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[出現](occurrence.md) <br/> |定期的な予定表アイテムの 1 つの変更されたアイテムを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

日付と時刻を表すテキスト値は、この要素を使用する場合に必要です。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

