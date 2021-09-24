---
title: アプリ
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f6f0a2ca-22dd-4789-9eed-f0c1ec9036c4
description: Apps 要素には、メールボックスにインストールされているアプリのすべての XML マニフェスト ファイルに関する情報が含まれています。
ms.openlocfilehash: 8a8b6c459a014517936d1c2753c4ce125892dacb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525308"
---
# <a name="apps"></a>アプリ

**Apps 要素** には、メールボックスにインストールされているアプリのすべての XML マニフェスト ファイルに関する情報が含まれています。 
  
```XML
<Apps>
    <App/>
</Apps>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[アプリ](app.md)
  
### <a name="parent-elements"></a>親要素

[GetAppManifestsResponse](getappmanifestsresponse.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |該当なし  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [アプリ](app.md)
- [GetAppManifestsResponse](getappmanifestsresponse.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

