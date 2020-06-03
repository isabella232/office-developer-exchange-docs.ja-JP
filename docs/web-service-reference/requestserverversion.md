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
description: RequestServerVersion 要素には、要求に対してターゲットとするスキーマバージョンを識別するバージョン管理情報が含まれています。
ms.openlocfilehash: c4ae59a03c812d21153e4338734185d933d914ec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468321"
---
# <a name="requestserverversion"></a>RequestServerVersion

**RequestServerVersion**要素には、要求に対してターゲットとするスキーマバージョンを識別するバージョン管理情報が含まれています。 
  
```XML
<RequestServerVersion Version=""/>
```

 **ExchangeVersionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|Version  <br/> |要求の対象となるバージョンを示します。 この属性は、ターゲットサーバーのバージョンが Exchange Server 2010 以降の Exchange のバージョンである場合に必要です。  <br/> |
   
#### <a name="version-attribute-values"></a>バージョン属性の値

|**値**|**説明**|
|:-----|:-----|
|Exchange2007  <br/> |Exchange 2007 の最初のリリースバージョンのスキーマファイルをターゲットにします。  <br/> |
|Exchange2007_SP1  <br/> |Exchange 2007 Service Pack 1 (SP1)、Exchange 2007 Service Pack 2 (SP2)、および Exchange 2007 Service Pack 3 (SP3) のスキーマファイルを対象とします。  <br/> |
|Exchange2010  <br/> |Exchange 2010 のスキーマファイルをターゲットにします。  <br/> |
|Exchange2010_SP1  <br/> |Exchange 2010 Service Pack 1 (SP1) のスキーマファイルをターゲットにします。  <br/> |
|Exchange2010_SP2  <br/> |Exchange 2010 Service Pack 2 (SP2) および Exchange 2010 Service Pack 3 (SP3) のスキーマファイルを対象とします。  <br/> |
|Exchange2013  <br/> |Exchange 2013 のスキーマファイルをターゲットにします。  <br/> |
|Exchange2013_SP1  <br/> |Exchange 2013 Service Pack 1 (SP1) のスキーマファイルをターゲットにします。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

**RequestServerVersion**要素は、SOAP ヘッダーにあります。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


[バージョン管理要求](https://msdn.microsoft.com/library/76877b0a-d2e5-4c74-9295-7b445a41d46a%28Office.15%29.aspx)

