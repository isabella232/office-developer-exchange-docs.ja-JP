---
title: StartDate (Recurrence)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- StartDate
api_type:
- schema
ms.assetid: bd65ac06-b3ac-4c9b-9568-3e4dc94378e7
description: StartDate 要素は、定期的なタスクまたは予定表アイテムの開始日を表します。
ms.openlocfilehash: 50f83e5c97d346cc3f7dfced1ee71aa3f9f38ed5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545868"
---
# <a name="startdate-recurrence"></a>StartDate (Recurrence)

**StartDate 要素** は、定期的なタスクまたは予定表アイテムの開始日を表します。 
  
```xml
<StartDate/>
```

**日付**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[EndDateRecurrence](enddaterecurrence.md) <br/> |アイテムの定期的なパターンの開始日と終了日を説明します。  <br/> |
|[NoEndRecurrence](noendrecurrence.md) <br/> |定義された終了日を持つアイテムの定期的なパターンの開始日を説明します。  <br/> |
|[NumberedRecurrence](numberedrecurrence.md) <br/> |定期的なアイテムの開始日と出現回数を示します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、日付を表すテキスト値が必要です。 値は、4 月 1 日 1601 00:00:00 未満にすることはできません。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

