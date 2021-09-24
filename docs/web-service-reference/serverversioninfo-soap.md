---
title: ServerVersionInfo (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 8662647b-e50a-4774-9ba3-a951ae6df781
description: ServerVersionInfo 要素には、要求を処理したサーバーのバージョンが含まれる。
ms.openlocfilehash: ac52b3eda429e65cb1ec046167a63fe4029d423a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521456"
---
# <a name="serverversioninfo-soap"></a>ServerVersionInfo (SOAP)

**ServerVersionInfo** 要素には、要求を処理したサーバーのバージョンが含まれる。 
  
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
|[MajorVersion (SOAP)](majorversion-soap.md) <br/> |サーバーのメジャー バージョン番号。  <br/> |
|[MinorVersion (SOAP)](minorversion-soap.md) <br/> |サーバーのマイナー バージョン番号。  <br/> |
|[MajorBuildNumber (SOAP)](majorbuildnumber-soap.md) <br/> |サーバーの主要なビルド番号。  <br/> |
|[MinorBuildNumber (SOAP)](minorbuildnumber-soap.md) <br/> |サーバーのマイナー ビルド番号。  <br/> |
|[Version (SOAP)](version-soap.md) <br/> |サーバー製品のバージョンの説明。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素は SOAP ヘッダーで返されます。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |はい  <br/> |
   

