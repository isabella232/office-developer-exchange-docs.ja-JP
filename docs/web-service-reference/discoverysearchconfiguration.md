---
title: DiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 085384f9-dca4-4534-82e2-dd782471d0da
description: DiscoverySearchConfiguration 要素は、電子情報開示検索の構成を指定します。
ms.openlocfilehash: 4f5f0a5b8e78521302fd136f0a0280aa3ff4e4c3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523098"
---
# <a name="discoverysearchconfiguration"></a>DiscoverySearchConfiguration

**DiscoverySearchConfiguration 要素は**、電子情報開示検索の構成を指定します。 
  
```XML
<DiscoverySearchConfiguration>
    <SearchId></SearchId>
    <SearchQuery></SearchQuery>
    <SearchableMailboxes></SearchableMailboxes>
</DiscoverySearchConfiguration>
```

 **DiscoverySearchConfigurationType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[SearchId](searchid.md) <br/> |検索の識別子を指定します。  <br/> |
|[SearchQuery](searchquery.md) <br/> |電子情報開示検索クエリの名前を指定します。  <br/> |
|[SearchableMailboxes](searchablemailboxes.md) <br/> |**GetSearchableMailboxes** 要求から返されるメールボックスの一覧を格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DiscoverySearchConfigurations](discoverysearchconfigurations.md) <br/> |**DiscoverySearchConfiguration 要素の配列を指定** します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

