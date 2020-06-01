---
title: Is自動応答
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAutomaticReply
api_type:
- schema
ms.assetid: 280e9baf-199d-422c-8fdf-1d0751a3e77d
description: Isautomatic Reply 要素は、条件または例外を適用するために、受信メッセージが自動応答である必要があるかどうかを示します。
ms.openlocfilehash: 7521dbbb458cf7683b52b2fe4fddacd276b40256
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455563"
---
# <a name="isautomaticreply"></a>Is自動応答

**Isautomatic reply**要素は、条件または例外を適用するために、受信メッセージが自動応答である必要があるかどうかを示します。 
  
```XML
<IsAutomaticReply> true | false</IsAutomaticReply>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[条件](conditions.md) <br/> |ルールのルールの処理を開始するときに実行される条件を表します。  <br/> |
|[例外](exceptions.md) <br/> |受信トレイルールに対して使用可能なすべてのルールの例外条件を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**True**のテキスト値は、条件または例外を適用するために、メッセージが自動応答である必要があることを示します。 値が**false**の場合、条件または例外を適用するために、メッセージは自動応答でなくてもよいことを示します。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

