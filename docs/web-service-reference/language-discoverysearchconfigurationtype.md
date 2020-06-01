---
title: 言語 (DiscoverySearchConfigurationType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 34eab81c-d832-4925-9f76-d69f24b36931
description: Language (DiscoverySearchConfigurationType) 要素は、カルチャ固有の日付範囲の形式に使用されるカルチャを指定します。 検索クエリで使用される言語も指定します。
ms.openlocfilehash: 3cf85525147bec5d6dfc6fe2b2af5916d42c44be
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463287"
---
# <a name="language-discoverysearchconfigurationtype"></a>言語 (DiscoverySearchConfigurationType)

**Language (DiscoverySearchConfigurationType)** 要素は、カルチャ固有の日付範囲の形式に使用されるカルチャを指定します。 検索クエリで使用される言語も指定します。 
  
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

この要素は、 [Searchmailboxes ボックス操作](searchmailboxes-operation.md)または[SetHoldOnMailboxes 操作](setholdonmailboxes-operation.md)で指定された日付範囲の形式を指定します。
  
この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[DiscoverySearchConfiguration](discoverysearchconfiguration.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

