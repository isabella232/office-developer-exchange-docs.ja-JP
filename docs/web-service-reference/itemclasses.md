---
title: ItemClasses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ItemClasses
api_type:
- schema
ms.assetid: f95430cc-2860-47c1-af2d-8c4156c9b281
description: ItemClasses 要素は、条件または例外を適用するために受信メッセージにスタンプする必要があるアイテム クラスを表します。
ms.openlocfilehash: a04c773d40d199902de7a7963e02444ed1def4fa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511428"
---
# <a name="itemclasses"></a>ItemClasses

**ItemClasses 要素** は、条件または例外を適用するために受信メッセージにスタンプする必要があるアイテム クラスを表します。 
  
```XML
<ItemClasses>
    <String/>
</ItemClasses>
```

 **ArrayOfStringsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[String](string.md) <br/> |1 つのアイテム クラスを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[条件](conditions.md) <br/> |満たされると、ルールのルール アクションをトリガーする条件を表します。  <br/> |
|[例外](exceptions.md) <br/> |受信トレイ ルールで使用可能なすべてのルール例外条件を表す例外を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

