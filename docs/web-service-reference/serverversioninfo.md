---
title: ServerVersionInfo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ServerVersionInfo
api_type:
- schema
ms.assetid: c04a6872-ca27-432b-aac2-36b023d0afc6
description: ServerVersionInfo 要素は、バージョン番号Microsoft Exchange Server表します。
ms.openlocfilehash: 6907559e1ac98981028a017b64a38a343c36da70
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517715"
---
# <a name="serverversioninfo"></a>ServerVersionInfo

**ServerVersionInfo 要素** は、バージョン番号Microsoft Exchange Server表します。 
  
```xml
<ServerVersionInfo MajorVersion="" MinorVersion="" MajorBuildNumber="" MinorBuildNumber="" Version="" />
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|MajorVersion  <br/> |メジャー バージョン番号について説明します。  <br/> |
|MinorVersion  <br/> |マイナー バージョン番号について説明します。  <br/> |
|MajorBuildNumber  <br/> |メジャー ビルド番号を説明します。  <br/> |
|MinorBuildNumber  <br/> |マイナー ビルド番号について説明します。  <br/> |
|バージョン  <br/> |Web サービス (EWS) Exchangeバージョンについて説明します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素は、Web Services 応答メッセージの SOAP ヘッダー Exchange返されます。
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされているコンピューター Microsoft Exchange Server EWS 仮想ディレクトリにあります。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にできる  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

