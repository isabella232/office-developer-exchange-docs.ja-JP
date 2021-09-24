---
title: IsInline
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsInline
api_type:
- schema
ms.assetid: 5e7712c8-372a-4a16-be64-360c5ff3961a
description: IsInline 要素は、添付ファイルがアイテム内にインラインで表示されるかどうかを表します。
ms.openlocfilehash: 0bf51c981f3c9d2a4e38939d349fe662a57b29ac
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518275"
---
# <a name="isinline"></a>IsInline

**IsInline 要素** は、添付ファイルがアイテム内にインラインで表示されるかどうかを表します。 
  
```xml
<IsInline>true or false</IsInline>
```

 **boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FileAttachment](fileattachment.md) <br/> |アイテム ストア内のアイテムに添付されているファイルをExchangeします。  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |別のアイテムExchange付けられたアイテムを表Exchangeします。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素には **、true** または false を **指定できます**。 既定値は **false** です。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされているコンピューター Microsoft Exchange Server EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

