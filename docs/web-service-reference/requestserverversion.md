---
title: RequestServerVersion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequestServerVersion
api_type:
- schema
ms.assetid: af4032d5-42b3-463e-9d0a-8236d78e5b75
description: RequestServerVersion 要素には、要求の対象とするスキーマのバージョンを識別するバージョン情報が含まれています。
ms.openlocfilehash: 0092d90a5fc479363f6d774b793c7148ad29f21c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833143"
---
# <a name="requestserverversion"></a>RequestServerVersion

**RequestServerVersion**要素には、要求の対象とするスキーマのバージョンを識別するバージョン情報が含まれています。 
  
```XML
<RequestServerVersion Version=""/>
```

 **ExchangeVersionType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|バージョン  <br/> |要求の対象とするバージョンをについて説明します。 対象サーバーのバージョンのバージョンの Exchange が Exchange Server 2010 で始まる場合、この属性が必要です。  <br/> |
   
#### <a name="version-attribute-values"></a>バージョン属性の値

|**値**|**説明**|
|:-----|:-----|
|Exchange2007  <br/> |初期リリース版の Exchange 2007 用のスキーマ ファイルを対象とします。  <br/> |
|Exchange2007_SP1  <br/> |Exchange 2007 Service Pack 1 (SP1)、Exchange 2007 Service Pack 2 (SP2)、および Exchange 2007 Service Pack 3 (SP3) 用のスキーマ ファイルを対象とします。  <br/> |
|Exchange2010  <br/> |Exchange 2010 用のスキーマ ファイルを対象とします。  <br/> |
|Exchange2010_SP1  <br/> |Exchange 2010 Service Pack 1 (SP1) 用のスキーマ ファイルを対象とします。  <br/> |
|Exchange2010_SP2  <br/> |Exchange 2010 Service Pack 2 (SP2) および Exchange 2010 Service Pack 3 (SP3) 用のスキーマ ファイルを対象とします。  <br/> |
|Exchange2013  <br/> |Exchange 2013 のスキーマ ファイルを対象とします。  <br/> |
|Exchange2013_SP1  <br/> |Exchange 2013 の Service Pack 1 (SP1) 用のスキーマ ファイルを対象とします。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

**RequestServerVersion**要素は、SOAP ヘッダーに配置されます。 
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


[バージョン管理の要求](http://msdn.microsoft.com/library/76877b0a-d2e5-4c74-9295-7b445a41d46a%28Office.15%29.aspx)

