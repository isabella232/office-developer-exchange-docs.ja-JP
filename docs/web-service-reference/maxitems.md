---
title: MaxItems
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4ddba6b8-0f38-42cd-96a1-0d4283f6375b
description: MaxItems 要素は、要求で取得するアイテムの最大数を指定します。
ms.openlocfilehash: dffb9ba4e29915a65fe2a57b6e7a7b4468028fa1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832384"
---
# <a name="maxitems"></a>MaxItems

**MaxItems**要素は、要求で取得するアイテムの最大数を指定します。 
  
```XML
<MaxItems/>
```

 **int**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[GetReminders](getreminders.md)
  
## <a name="text-value"></a>テキスト値

**MaxItems**要素のテキスト値は、要求で取得するアイテムの最大数です。 この数には、0 以上 200 より大きい値を指定できません。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetReminders](getreminders.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

