---
title: スコープ (NonEmptyStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Scope
api_type:
- schema
ms.assetid: 7efb6fd9-1615-469e-96f6-0f7846ad9b44
description: スコープ要素は、メッセージ追跡レポートの範囲を指定します。
ms.openlocfilehash: 534ed23916a60b246c7cb5be4a59d086980a7c37
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833280"
---
# <a name="scope-nonemptystringtype"></a>スコープ (NonEmptyStringType)

**スコープ**要素は、メッセージ追跡レポートの範囲を指定します。 
  
```XML
<Scope>Organization | Forest | Site</Scope>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[FindMessageTrackingReport](findmessagetrackingreport.md) | [GetMessageTrackingReport](getmessagetrackingreport.md)
  
## <a name="text-value"></a>テキスト値

**スコープ**要素の有効な値を次の表に一覧します。 
  
|**値**|**説明**|
|:-----|:-----|
|組織  <br/> |組織全体にわたってメッセージ追跡用のスコープにまたがっています。  <br/> |
|フォレスト  <br/> |フォレストにまたがるメッセージのスコープを追跡できます。  <br/> |
|サイト  <br/> |サイトにまたがるメッセージのスコープを追跡できます。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

