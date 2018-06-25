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
ms.openlocfilehash: b02071e4997aba91fb538d52df2612fe6fd32800
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833385"
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[MajorVersion (SOAP)](majorversion-soap.md) <br/> |サーバーのメジャー バージョン番号です。  <br/> |
|[マイナー バージョン (SOAP)](minorversion-soap.md) <br/> |サーバーのマイナー バージョン番号です。  <br/> |
|[MajorBuildNumber (SOAP)](majorbuildnumber-soap.md) <br/> |サーバーのメジャー ビルド番号。  <br/> |
|[MinorBuildNumber (SOAP)](minorbuildnumber-soap.md) <br/> |サーバーのマイナー ビルド番号。  <br/> |
|[バージョン (SOAP)](version-soap.md) <br/> |サーバー製品のバージョンの説明です。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

この要素は、SOAP ヘッダーで返されます。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   

