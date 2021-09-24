---
title: DiagnosticsLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DiagnosticsLevel
api_type:
- schema
ms.assetid: 66794226-f5e0-44f0-8a0e-1f194bb0ba0f
description: DiagnosticsLevel 要素は、レポートの派生に使用されるタイミングとパフォーマンスの情報を表します。
ms.openlocfilehash: c7e74f324385ca76a58872e2e735ea2c5d926a53
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519801"
---
# <a name="diagnosticslevel"></a>DiagnosticsLevel

**DiagnosticsLevel** 要素は、レポートの派生に使用されるタイミングとパフォーマンスの情報を表します。 
  
```XML
<DiagnosticsLevel/>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindMessageTrackingReport](findmessagetrackingreport.md) <br/> |検索するメッセージの種類の条件が含まれます。  <br/> |
|[GetMessageTrackingReport](getmessagetrackingreport.md) <br/> |指定した ID の完全なメッセージ追跡レポートを取得する [GetMessageTrackingReport](getmessagetrackingreport-operation.md) 操作の要求を格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、文字列を表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

