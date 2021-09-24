---
title: UmEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UmEnabled
api_type:
- schema
ms.assetid: 87382d9b-0c02-49ec-85dc-3f5918df3195
description: UmEnabled 要素は、アカウントでユニファイド メッセージングが有効になっているかどうかを示します。
ms.openlocfilehash: 9ff6432324e3a15b9ae805a7d6d836c9c895059c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527154"
---
# <a name="umenabled"></a>UmEnabled

**UmEnabled 要素** は、アカウントでユニファイド メッセージングが有効になっているかどうかを示します。 
  
```XML
<UmEnabled>true | false</UmEnabled>
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
|[UnifiedMessagingConfiguration](unifiedmessagingconfiguration.md) <br/> |ユニファイド メッセージング サービスのサービス構成情報が含まれる。  <br/> |
   
## <a name="text-value"></a>テキスト値

アカウントでユニファイド メッセージングが有効になっている場合 **、UmEnabled** 要素のテキスト値は true です。 それ以外の場合、値は false **です**。
  
## <a name="remarks"></a>注釈

この要素は必須です。
  
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

