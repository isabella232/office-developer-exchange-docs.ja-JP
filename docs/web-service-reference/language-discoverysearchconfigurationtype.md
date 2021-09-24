---
title: Language (DiscoverySearchConfigurationType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 34eab81c-d832-4925-9f76-d69f24b36931
description: Language (DiscoverySearchConfigurationType) 要素は、日付範囲のカルチャ固有の形式に使用するカルチャを識別します。 また、検索クエリで使用される言語も指定します。
ms.openlocfilehash: 5d51960aa00b2c47d96972abc05e4d6027eeecb3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540896"
---
# <a name="language-discoverysearchconfigurationtype"></a>Language (DiscoverySearchConfigurationType)

Language **(DiscoverySearchConfigurationType)** 要素は、日付範囲のカルチャ固有の形式に使用するカルチャを識別します。 また、検索クエリで使用される言語も指定します。 
  
```XML
<Language />
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[DiscoverySearchConfiguration](discoverysearchconfiguration.md)
  
## <a name="text-value"></a>テキスト値

**Language (DiscoverySearchConfigurationType)** 要素のテキスト値は、カルチャまたは言語です。 
  
## <a name="remarks"></a>注釈

この要素は [、SearchMailboxes](searchmailboxes-operation.md) 操作または [SetHoldOnMailboxes](setholdonmailboxes-operation.md)操作で指定された日付範囲の形式を指定します。
  
この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[DiscoverySearchConfiguration](discoverysearchconfiguration.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

