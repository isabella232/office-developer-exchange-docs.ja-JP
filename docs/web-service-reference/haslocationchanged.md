---
title: HasLocationChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 5fd465b4-6070-4cd0-9ac3-ed9d2bfd5951
description: HasLocationChanged 要素は、会議の場所プロパティが変更されたかどうかを指定します。
ms.openlocfilehash: f59bca138d0baee87afd12470d9c50704edc75bd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519549"
---
# <a name="haslocationchanged"></a>HasLocationChanged

**HasLocationChanged 要素** は、会議の場所プロパティが変更されたかどうかを指定します。 
  
```XML
<HasLocationChanged> true | false </HasLocationChanged>
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

**HasLocationChanged** **要素のテキスト** 値 true は、会議の location プロパティが変更されたかどうかを示します。 値 **false は** 、会議の場所プロパティが変更されていないかどうかを示します。 
  
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

