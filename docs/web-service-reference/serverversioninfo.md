---
title: ServerVersionInfo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ServerVersionInfo
api_type:
- schema
ms.assetid: c04a6872-ca27-432b-aac2-36b023d0afc6
description: ServerVersionInfo 要素は、Microsoft Exchange Server のバージョン番号を表します。
ms.openlocfilehash: 5bd1fbd8fdee584a9d272fa8ab82f2a31c1357fe
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466830"
---
# <a name="serverversioninfo"></a>ServerVersionInfo

**ServerVersionInfo**要素は、Microsoft Exchange Server のバージョン番号を表します。 
  
```xml
<ServerVersionInfo MajorVersion="" MinorVersion="" MajorBuildNumber="" MinorBuildNumber="" Version="" />
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|MajorVersion  <br/> |メジャーバージョン番号について説明します。  <br/> |
|MinorVersion  <br/> |マイナーバージョン番号を記述します。  <br/> |
|MajorBuildNumber  <br/> |主要なビルド番号を記述します。  <br/> |
|MinorBuildNumber または  <br/> |マイナービルド番号を記述します。  <br/> |
|バージョン  <br/> |Exchange Web サービス (EWS) スキーマのバージョンについて説明します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素は、Exchange Web サービス応答メッセージの SOAP ヘッダーで返されます。
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

