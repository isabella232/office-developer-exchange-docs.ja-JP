---
title: 発表者
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 01057872-4f1a-4246-86ba-73d10ef854a0
description: Presenters 要素は、オンライン会議の発表者を指定します。
ms.openlocfilehash: 1c9bf9093450e675245b647c98d7b1d00101ce9e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519143"
---
# <a name="presenters"></a>発表者

Presenters **要素** は、オンライン会議の発表者を指定します。 
  
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

Presenters 要素の **テキスト値** は、オンライン会議の発表者になるユーザーの種類です。 Presenters 要素の **テキスト値を** 次の表に示します。 
  
**発表者要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|無効  <br/> |発表者は無効です。  <br/> |
|内部  <br/> |発表者は内部参加者のみ可能です。  <br/> |
|すべてのユーザー  <br/> |参加者は誰でも発表者にできます。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> ||
   

