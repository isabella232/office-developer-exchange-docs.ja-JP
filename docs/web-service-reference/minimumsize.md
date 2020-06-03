---
title: MinimumSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 841d229c-140c-48bd-b3a7-21478fcea2fb
description: MinimumSize 要素は、条件または例外を適用するためにメッセージが必要とされる最小サイズを表します。
ms.openlocfilehash: b43a8b5916747c4e3e4ca9b66cf8b9d73f5f8942
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464204"
---
# <a name="minimumsize"></a>MinimumSize

**Minimumsize**要素は、条件または例外を適用するためにメッセージが必要とされる最小サイズを表します。 
  
```XML
<MinimumSize/>
```

 **int**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[WithinSizeRange](withinsizerange.md) <br/> |条件または例外を適用するために、受信メッセージが必要とする最小サイズと最大サイズを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、メッセージの最小サイズをバイト単位で示す整数です。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[MaximumSize](maximumsize.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

