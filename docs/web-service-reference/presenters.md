---
title: プレゼン
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 01057872-4f1a-4246-86ba-73d10ef854a0
description: プレゼンター要素は、オンライン会議のプレゼンターを指定します。
ms.openlocfilehash: 0236457020dfc4684569e84d3d54e357af00d102
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529911"
---
# <a name="presenters"></a>プレゼン

**プレゼンター**要素は、オンライン会議のプレゼンターを指定します。 
  
```XML
<Presenters> Disabled | Internal | Everyone </Presenters>
```

 **PresentersType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[OnlineMeetingSettings](onlinemeetingsettings.md)
  
## <a name="text-value"></a>テキスト値

**プレゼンター**要素のテキスト値は、オンライン会議の発表者になることができるユーザーの種類です。 次の表では、**プレゼンター**要素のテキスト値について説明します。 
  
**プレゼンター要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|無効  <br/> |プレゼンターは無効になっています。  <br/> |
|内部  <br/> |内部参加者のみがプレゼンターになることができます。  <br/> |
|すべてのユーザー  <br/> |参加者はすべて発表者になることができます。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   

