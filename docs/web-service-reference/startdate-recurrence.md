---
title: 開始日 (繰り返し)
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
description: 開始要素では、定期的な仕事または予定表アイテムの開始日を表します。
ms.openlocfilehash: 6a38e63bbcf010ab6dca8f66440a2b0a559cf88d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833551"
---
# <a name="startdate-recurrence"></a>開始日 (繰り返し)

**開始**要素では、定期的な仕事または予定表アイテムの開始日を表します。 
  
```xml
<StartDate/>
```

**日付**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[EndDateRecurrence](enddaterecurrence.md) <br/> |開始日と終了日の項目の定期的なパターンについて説明します。  <br/> |
|[NoEndRecurrence](noendrecurrence.md) <br/> |定義された終了日がない項目の定期的なパターンの開始日について説明します。  <br/> |
|[NumberedRecurrence](numberedrecurrence.md) <br/> |開始日と定期的なアイテムの出現回数を説明します。  <br/> |
   
## <a name="text-value"></a>テキスト値

日付を表すテキスト値は、この要素を使用する場合に必要です。 1601、4 月、1 より小さい値を指定できません 00時 00分: 00 です。
  
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

