---
title: MaxItems
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 4ddba6b8-0f38-42cd-96a1-0d4283f6375b
description: MaxItems 要素は、要求で返されるアイテムの最大数を指定します。
ms.openlocfilehash: 23a78db874ef3678be8c6703fb7004fc5f8a1425
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511117"
---
# <a name="maxitems"></a>MaxItems

**MaxItems 要素** は、要求で返されるアイテムの最大数を指定します。 
  
```XML
<MaxItems/>
```

 **int**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[GetReminders](getreminders.md)
  
## <a name="text-value"></a>テキスト値

**MaxItems** 要素のテキスト値は、要求で返されるアイテムの最大数です。 この数値は、0 未満または 200 より大きくすることはできません。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetReminders](getreminders.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

