---
title: 言語 (DiscoverySearchConfigurationType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 34eab81c-d832-4925-9f76-d69f24b36931
description: (DiscoverySearchConfigurationType) の言語要素は、カルチャに固有の形式の日付の範囲に使用するカルチャを識別します。 また、検索クエリで使用する言語を指定します。
ms.openlocfilehash: 1e904ac4d7f525b2d12cfe83f0da33b9ed474066
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832197"
---
# <a name="language-discoverysearchconfigurationtype"></a>言語 (DiscoverySearchConfigurationType)

**(DiscoverySearchConfigurationType) の言語**要素は、カルチャに固有の形式の日付の範囲に使用するカルチャを識別します。 また、検索クエリで使用する言語を指定します。 
  
```XML
<Language />
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[DiscoverySearchConfiguration](discoverysearchconfiguration.md)
  
## <a name="text-value"></a>テキスト値

**言語 (DiscoverySearchConfigurationType)** の要素のテキスト値は、カルチャまたは言語です。 
  
## <a name="remarks"></a>備考

この要素は、 [SearchMailboxes 操作](searchmailboxes-operation.md)または[SetHoldOnMailboxes 操作](setholdonmailboxes-operation.md)で指定された日付範囲の書式を指定します。
  
この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[DiscoverySearchConfiguration](discoverysearchconfiguration.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

