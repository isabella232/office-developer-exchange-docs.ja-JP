---
title: マニフェスト
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 650d9fc0-1504-4db4-95d6-d3ba86df66ca
description: Manifests 要素には、電子メール アカウント用にインストールされている base64 エンコードアプリ マニフェストのコレクションが含まれています。
ms.openlocfilehash: e29a892fa69f33e9b7bb81f8abc9cc13b4649c51
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522671"
---
# <a name="manifests"></a>マニフェスト

**Manifests 要素** には、電子メール アカウント用にインストールされている base64 エンコードアプリ マニフェストのコレクションが含まれています。 
  
```XML
<Manifests>
   <Manifest/>
</Manifests>
```

 **ArrayOfAppManifestsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[マニフェスト](manifest.md)
  
### <a name="parent-elements"></a>親要素

[GetAppManifestsResponse](getappmanifestsresponse.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空の場合  <br/> ||
   

