---
title: AccessLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 09475586-00fa-4e82-a915-5ca263ab4d1c
description: AccessLevel 要素は、オンライン会議のアクセス レベルを指定します。
ms.openlocfilehash: f1c85579affe7d1142b22a890808bceeb8f82d38
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544417"
---
# <a name="accesslevel"></a>AccessLevel

**AccessLevel 要素** は、オンライン会議のアクセス レベルを指定します。 
  
```XML
<AccessLevel/>
```

 **OnlineMeetingSettingsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[OnlineMeetingSettings](onlinemeetingsettings.md) <br/> |オンライン会議の設定を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に **、AccessLevel 要素のテキスト値を示** します。 
  
**AccessLevel 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|すべてのユーザー  <br/> |アクセス レベルは、すべて開きます。  <br/> |
|内部  <br/> |アクセス レベルは内部のみです。  <br/> |
|招待  <br/> |アクセス レベルは招待された参加者のみです。  <br/> |
|ロックされています  <br/> |アクセス レベルはロックされています。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
この要素は Exchange Server 2013 で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> ||
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

