---
title: アプリ
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f6f0a2ca-22dd-4789-9eed-f0c1ec9036c4
description: Apps 要素には、メールボックスにインストールされたアプリのすべての XML マニフェストファイルに関する情報が含まれています。
ms.openlocfilehash: b2d6f13241f68cbed449a9f9821f9a6ec6ff687a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527447"
---
# <a name="apps"></a>アプリ

**Apps**要素には、メールボックスにインストールされたアプリのすべての XML マニフェストファイルに関する情報が含まれています。 
  
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

[App](app.md)
  
### <a name="parent-elements"></a>親要素

[GetAppManifestsResponse](getappmanifestsresponse.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |該当なし  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [App](app.md)
- [GetAppManifestsResponse](getappmanifestsresponse.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

