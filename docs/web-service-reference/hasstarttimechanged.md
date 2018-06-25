---
title: HasStartTimeChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 04a6968d-7fb5-47ee-b66e-dc99c35dbb63
description: HasStartTimeChanged 要素は、会議の開始時刻が変更されたかどうかを指定します。
ms.openlocfilehash: 2096084f4ec8848a63d10e0e80fdc7a37e473cd8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831809"
---
# <a name="hasstarttimechanged"></a>HasStartTimeChanged

**HasStartTimeChanged**要素は、会議の開始時刻が変更されたかどうかを指定します。 
  
```XML
<HasStartTimeChanged> true | false </HasStartTimeChanged>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ChangeHighlights](changehighlights.md) <br/> |会議の 2 つのバージョン間で変更内容を指定する要求メッセージ。  <br/> |
   
## <a name="text-value"></a>テキスト値

の**場合は true** 、 **HasStartTimeChanged**要素のテキスト値は、会議の開始時刻が変更されたことを示します。 **False**の値を開始時刻が変更されないことを示します。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型のスキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

