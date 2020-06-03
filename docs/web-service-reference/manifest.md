---
title: マニフェスト
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: af0d7435-fef6-4f0d-bd22-00e3fa576315
description: Manifest 要素には、base64 でエンコードされたアプリマニフェストファイルが含まれています。
ms.openlocfilehash: faac517bf8a8f03c6ae8abffddaf10421eed1699
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530538"
---
# <a name="manifest"></a>マニフェスト

**Manifest**要素には、base64 でエンコードされたアプリマニフェストファイルが含まれています。 
  
```XML
<Manifest></Manifest>
```

 **base64Binary**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[マニフェスト](manifests.md)  | [Installapp](installapp.md)  | [Clientextension](clientextension.md)
  
## <a name="text-value"></a>テキスト値

Manifest 要素のテキスト値は、クライアントアプリケーションマニフェストファイルの base64 バイナリエンコード形式を ASCII で表現したものです。
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  

