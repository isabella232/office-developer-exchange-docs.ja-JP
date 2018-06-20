---
title: MaximumSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fb7c3ab3-ef97-44c7-83e0-93cfe8c48e84
description: 作成要素は、メッセージ内に含まれる条件や例外条件を適用する順序の最大サイズを表します。
ms.openlocfilehash: 37e3d377b105534fe34b54e262bd47bc450706da
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832387"
---
# <a name="maximumsize"></a>MaximumSize

**作成**要素は、メッセージ内に含まれる条件や例外条件を適用する順序の最大サイズを表します。 
  
```XML
<Maximum/>
```

 **int**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[WithinSizeRange](withinsizerange.md) <br/> |適用する場合の条件または例外の順序で受信メッセージをする必要のある最小値と最大サイズを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、バイト単位でのメッセージの最大サイズを識別する整数です。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[MinimumSize](minimumsize.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

