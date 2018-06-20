---
title: 発表者
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 01057872-4f1a-4246-86ba-73d10ef854a0
description: プレゼンター要素は、オンライン会議の発表者を指定します。
ms.openlocfilehash: f62b458759e0d8199c98827602d6c3fe16aebeea
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832875"
---
# <a name="presenters"></a>発表者

**プレゼンター**要素は、オンライン会議の発表者を指定します。 
  
```XML
<Presenters> Disabled | Internal | Everyone </Presenters>
```

 **PresentersType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[OnlineMeetingSettings](onlinemeetingsettings.md)
  
## <a name="text-value"></a>テキスト値

**発表者**の要素のテキスト値は、オンライン会議の発表者ことができるユーザーの種類です。 **発表者**の要素のテキスト値は、次の表で説明します。 
  
**要素のテキスト値を発表**

|**値**|**説明**|
|:-----|:-----|
|無効  <br/> |発表者が無効になります。  <br/> |
|内部  <br/> |内部のみの参加者は、発表者を指定できます。  <br/> |
|全員  <br/> |任意の参加者、発表者ができます。  <br/> |
   
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> ||
   

