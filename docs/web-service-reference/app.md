---
title: アプリ
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 92b776b5-fec6-4443-a606-51ccb06f7afd
description: App 要素には、メールボックスにインストールされているメール アプリの XML マニフェスト ファイルに関する情報が含まれています。
ms.openlocfilehash: 548df0f5547c4d7bf3ffacd32308be6824fadaf2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520123"
---
# <a name="app"></a>アプリ

App **要素** には、メールボックスにインストールされているメール アプリの XML マニフェスト ファイルに関する情報が含まれています。 
  
```XML
<App>
    <Metadata/>
    <Manifest/>
</App>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[メタデータ](metadata-ex15websvcsotherref.md)  | [マニフェスト](manifest.md)
  
### <a name="parent-elements"></a>親要素

[アプリ](apps.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |該当なし  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [アプリ](apps.md)
- [メタデータ](metadata-ex15websvcsotherref.md)
- [マニフェスト](manifest.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

