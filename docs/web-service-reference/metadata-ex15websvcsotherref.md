---
title: メタデータ
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c1cc609b-65ff-4998-8d2b-545f0fdcb54c
description: メタデータ要素には、メール ・ アプリケーションについてのメタデータが含まれています。
ms.openlocfilehash: 8dd3a3db5a5e0afc1a23dad44d70fa3353c796f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832459"
---
# <a name="metadata"></a>メタデータ

**メタデータ**要素には、メール ・ アプリケーションについてのメタデータが含まれています。 
  
```XML
<Metadata>
    <EndNodeUrl/>
    <AppStatus/>
    <ActionUrl/>
</Metadata>
```

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[EndNodeUrl](endnodeurl.md) | [AppStatus](appstatus-ex15websvcsotherref.md) | [ActionUrl](actionurl.md)
  
### <a name="parent-elements"></a>親要素

[App](app.md)
  
## <a name="remarks"></a>Remarks

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> | http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |該当しない  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[App](app.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

