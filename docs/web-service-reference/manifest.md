---
title: マニフェスト
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: af0d7435-fef6-4f0d-bd22-00e3fa576315
description: Manifest 要素には、base64 エンコードされたアプリ マニフェスト ファイルが含まれます。
ms.openlocfilehash: 418191c47af0422c2d555b577dd804e02f0e38ce
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524764"
---
# <a name="manifest"></a>マニフェスト

**Manifest 要素** には、base64 エンコードされたアプリ マニフェスト ファイルが含まれます。 
  
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

[マニフェスト](manifests.md)  | [InstallApp](installapp.md)  | [ClientExtension](clientextension.md)
  
## <a name="text-value"></a>テキスト値

Manifest 要素のテキスト値は、クライアント アプリ マニフェスト ファイルの base64 バイナリ エンコード形式の ASCII 表記です。
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  

