---
title: アプリ
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f6f0a2ca-22dd-4789-9eed-f0c1ec9036c4
description: アプリケーション要素には、メールボックスにインストールされているアプリケーションのすべての XML マニフェスト ファイルに関する情報が含まれています。
ms.openlocfilehash: 81b0cb76b02fcc9145f6d70eff12a0a0ac0ad51f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759426"
---
# <a name="apps"></a>アプリ

**アプリケーション**要素には、メールボックスにインストールされているアプリケーションのすべての XML マニフェスト ファイルに関する情報が含まれています。 
  
```XML
<Apps>
    <App/>
</Apps>
```

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[App](app.md)
  
### <a name="parent-elements"></a>親要素

[GetAppManifestsResponse](getappmanifestsresponse.md)
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |該当しない  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [App](app.md)
- [GetAppManifestsResponse](getappmanifestsresponse.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

