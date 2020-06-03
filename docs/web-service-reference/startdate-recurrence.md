---
title: StartDate (定期的な予定)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartDate
api_type:
- schema
ms.assetid: bd65ac06-b3ac-4c9b-9568-3e4dc94378e7
description: StartDate 要素は、定期的な仕事または予定表アイテムの開始日を表します。
ms.openlocfilehash: 4514f126b1de31c64a2650b9e7cb6b7412a726c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457208"
---
# <a name="startdate-recurrence"></a>StartDate (定期的な予定)

**StartDate**要素は、定期的な仕事または予定表アイテムの開始日を表します。 
  
```xml
<StartDate/>
```

**Date**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[EndDateRecurrence](enddaterecurrence.md) <br/> |アイテムの定期的なパターンの開始日と終了日を示します。  <br/> |
|[NoEndRecurrence](noendrecurrence.md) <br/> |定義済みの終了日を持たないアイテムの定期的なパターンの開始日を示します。  <br/> |
|[NumberedRecurrence](numberedrecurrence.md) <br/> |定期的なアイテムの開始日と発生回数を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、日付を表すテキスト値が必要です。 この値は、Apr、1、1601 00:00:00 より小さくすることはできません。
  
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

