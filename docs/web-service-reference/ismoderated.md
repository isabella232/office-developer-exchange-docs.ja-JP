---
title: IsModerated
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsModerated
api_type:
- schema
ms.assetid: a7562256-feb9-41a1-857e-b5d41cbed680
description: IsModerated 要素は、受信者のメールボックスがモデ管理されているかどうかを示します。
ms.openlocfilehash: e06e7e01e08cb8418adafaae09cae94ceb5c3b2c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522902"
---
# <a name="ismoderated"></a>IsModerated

**IsModerated 要素** は、受信者のメールボックスがモデ管理されているかどうかを示します。 
  
```XML
<IsModerated>true | false</IsModerated>
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
|[メールヒント](mailtips.md) <br/> |さまざまな種類のメール ヒントの値を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素のテキスト値は、 **受信者** のメールボックスがモデレドされている場合は true です。 受信者の **メールボックスがモ** デ管理されていない場合、値は false です。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

