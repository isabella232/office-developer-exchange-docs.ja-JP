---
title: マニフェスト
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: af0d7435-fef6-4f0d-bd22-00e3fa576315
description: マニフェストの要素には、base64 でエンコードされたアプリケーション マニフェスト ファイルが含まれています。
ms.openlocfilehash: 7388e40a96a082666519d1c67af5b218b2b9ab01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832343"
---
# <a name="manifest"></a>マニフェスト

**マニフェスト**の要素には、base64 でエンコードされたアプリケーション マニフェスト ファイルが含まれています。 
  
```XML
<Manifest></Manifest>
```

 **base64Binary**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[マニフェスト](manifests.md) | [InstallApp](installapp.md) | [ClientExtension](clientextension.md)
  
## <a name="text-value"></a>テキスト値

マニフェストの要素のテキスト値は、クライアント アプリケーションのマニフェスト ファイルの ASCII エンコードされた base64 をバイナリの表現形式です。
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  

