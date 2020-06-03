---
title: ActionUrl
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9697f2e5-a5f7-471a-a052-ae79e06eb09d
description: ActionUrl 要素は、AppStatus 要素によって示された問題を修正するために、ユーザーが移動する必要のある URL を識別します。
ms.openlocfilehash: 2335595b4be6452f41c25f15d359e6939609c9b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529673"
---
# <a name="actionurl"></a>ActionUrl

**Actionurl**要素は、 [appstatus](appstatus-ex15websvcsotherref.md)要素によって示された問題を修正するために、ユーザーが移動する必要のある url を識別します。 
  
```XML
<ActionUrl/>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[メタデータ](metadata-ex15websvcsotherref.md)
  
## <a name="text-value"></a>テキスト値

**Actionurl**要素のテキスト値は、 **appstatus**要素によって示された問題を修正するために、ユーザーが移動する必要のある url を示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> | https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |該当なし  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [メタデータ](metadata-ex15websvcsotherref.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

