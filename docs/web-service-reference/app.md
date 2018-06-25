---
title: アプリ
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 92b776b5-fec6-4443-a606-51ccb06f7afd
description: アプリケーション要素には、メールボックスにインストールされているメール アプリの XML マニフェスト ファイルに関する情報が含まれています。
ms.openlocfilehash: c63bbbf6eb3bf718b2cf81e67d9ec978b3bc5f8d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759330"
---
# <a name="app"></a>アプリ

**アプリケーション**要素には、メールボックスにインストールされているメール アプリの XML マニフェスト ファイルに関する情報が含まれています。 
  
```XML
<App>
    <Metadata/>
    <Manifest/>
</App>
```

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[メタデータ](metadata-ex15websvcsotherref.md) | [マニフェスト](manifest.md)
  
### <a name="parent-elements"></a>親要素

[アプリ](apps.md)
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |該当しない  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [アプリ](apps.md)
- [メタデータ](metadata-ex15websvcsotherref.md)
- [Manifest](manifest.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

