---
title: HasEndTimeChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: a0eb444d-8e2e-478b-b785-2b9787ffb226
description: HasEndTimeChanged 要素は、会議の終了時刻が変更されたかどうかを指定します。
ms.openlocfilehash: f5f0c54e210219566786980ca02f33d72307dcff
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516777"
---
# <a name="hasendtimechanged"></a>HasEndTimeChanged

**HasEndTimeChanged** 要素は、会議の終了時刻が変更されたかどうかを指定します。 
  
```XML
<HasEndTimeChanged>true | false</HasEndTimeChanged>
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
|[ChangeHighlights](changehighlights.md) <br/> |2 つのバージョンの会議出席依頼メッセージの間で何が変更されたかを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**HasEndTimeChanged** 要素のテキスト値 **true** は、会議の終了時刻が変更されたかどうかを示します。 false の **値は** 、会議の終了時刻が変更されていないかどうかを示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

