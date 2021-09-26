---
title: RequestServerVersion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RequestServerVersion
api_type:
- schema
ms.assetid: af4032d5-42b3-463e-9d0a-8236d78e5b75
description: RequestServerVersion 要素には、要求の対象となるスキーマ バージョンを識別するバージョン管理情報が含まれる。
ms.openlocfilehash: 4f01d5fcc2a2e08d426efc8d1f0a193d6139a038
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541876"
---
# <a name="requestserverversion"></a>RequestServerVersion

**RequestServerVersion** 要素には、要求の対象となるスキーマ バージョンを識別するバージョン管理情報が含まれる。 
  
```XML
<RequestServerVersion Version=""/>
```

 **ExchangeVersionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|Version  <br/> |要求の対象となるバージョンについて説明します。 この属性は、ターゲット サーバーのバージョンが 2010 年ExchangeバージョンExchange Serverです。  <br/> |
   
#### <a name="version-attribute-values"></a>Version 属性値

|**値**|**説明**|
|:-----|:-----|
|Exchange2007  <br/> |2007 年の初期リリース バージョンのスキーマ ファイルExchangeします。  <br/> |
|Exchange2007_SP1  <br/> |Exchange 2007 Service Pack 1 (SP1)、Exchange 2007 Service Pack 2 (SP2)、および Exchange 2007 Service Pack 3 (SP3) のスキーマ ファイルをターゲットに設定します。  <br/> |
|Exchange2010  <br/> |2010 年のスキーマ ファイルExchangeします。  <br/> |
|Exchange2010_SP1  <br/> |2010 Service Pack 1 (SP1) Exchangeスキーマ ファイルをターゲットに設定します。  <br/> |
|Exchange2010_SP2  <br/> |2010 Service Pack 2 (SP2 Exchange) および Exchange 2010 Service Pack 3 (SP3) のスキーマ ファイルをターゲットに設定します。  <br/> |
|Exchange2013  <br/> |2013 年のスキーマ ファイルExchangeします。  <br/> |
|Exchange2013_SP1  <br/> |2013 Service Pack 1 (SP1) Exchangeスキーマ ファイルをターゲットに設定します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

**RequestServerVersion** 要素は SOAP ヘッダー内に存在します。 
  
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


[バージョン管理要求](https://msdn.microsoft.com/library/76877b0a-d2e5-4c74-9295-7b445a41d46a%28Office.15%29.aspx)

