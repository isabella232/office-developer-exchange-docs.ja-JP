---
title: ServerVersionInfo (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 8662647b-e50a-4774-9ba3-a951ae6df781
description: ServerVersionInfo 要素には、要求を処理したサーバーのバージョンが含まれています。
ms.openlocfilehash: b54b4833361ec78c7f8213473af4638965c7ddae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467649"
---
# <a name="serverversioninfo-soap"></a>ServerVersionInfo (SOAP)

**ServerVersionInfo**要素には、要求を処理したサーバーのバージョンが含まれています。 
  
```XML
<ServerVersionInfo>
   <MajorVersion/>
   <MinorVersion/>
   <MajorBuildNumber/>
   <MinorBuildNumber/>
   <Version/>
</ServerVersionInfo>
```

 **ServerVersionInfo**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MajorVersion (SOAP)](majorversion-soap.md) <br/> |サーバーのメジャーバージョン番号。  <br/> |
|[MinorVersion (SOAP)](minorversion-soap.md) <br/> |サーバーのマイナーバージョン番号。  <br/> |
|[MajorBuildNumber (SOAP)](majorbuildnumber-soap.md) <br/> |サーバーのメジャービルド番号。  <br/> |
|[MinorBuildNumber/(SOAP)](minorbuildnumber-soap.md) <br/> |サーバーのマイナービルド番号。  <br/> |
|[バージョン (SOAP)](version-soap.md) <br/> |サーバー製品バージョンの説明。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素は、SOAP ヘッダーで返されます。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |はい  <br/> |
   

