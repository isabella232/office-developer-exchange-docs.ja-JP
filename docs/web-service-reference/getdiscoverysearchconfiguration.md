---
title: GetDiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: e15dbfca-3b9d-463e-94ec-4f1b6115bee3
description: GetDiscoverySearchConfiguration 要素は、電子情報開示検索構成を取得する要求を指定します。
ms.openlocfilehash: ff84e648e14b79f64cf2a769c83aae28791790ef
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519689"
---
# <a name="getdiscoverysearchconfiguration"></a>GetDiscoverySearchConfiguration

**GetDiscoverySearchConfiguration 要素** は、電子情報開示検索構成を取得する要求を指定します。 
  
```XML
<GetDiscoverySearchConfiguration>
    <SearchId/>
    <ExpandGroupMembership/>
</GetDiscoverySearchConfiguration>
```

 **GetDiscoverySearchConfigurationType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[SearchId](searchid.md) <br/> |検索の識別子を指定します。  <br/> |
|[ExpandGroupMembership](expandgroupmembership.md) <br/> |**GetSearchableMailboxes** 要求から返されるグループのメンバーシップを展開するかどうかを示すブール型 (Boolean) の値を含む。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
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

