---
title: AccessLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 09475586-00fa-4e82-a915-5ca263ab4d1c
description: AccessLevel 要素は、オンライン会議のアクセスレベルを指定します。
ms.openlocfilehash: 3c1375ef37ea666c6c4fafce7daa46ae0d0a2696
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462340"
---
# <a name="accesslevel"></a>AccessLevel

**Accesslevel**要素は、オンライン会議のアクセスレベルを指定します。 
  
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

次の表に、 **Accesslevel**要素のテキスト値を示します。 
  
**AccessLevel 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|すべてのユーザー  <br/> |アクセスレベルが [すべて] になっています。  <br/> |
|内部  <br/> |アクセスレベルは内部のみです。  <br/> |
|あなた  <br/> |アクセスレベルは、招待された参加者のみになります。  <br/> |
|ロックされています  <br/> |アクセスレベルがロックされています。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
この要素は Exchange Server 2013 で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

