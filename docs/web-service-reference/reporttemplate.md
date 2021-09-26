---
title: ReportTemplate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ReportTemplate
api_type:
- schema
ms.assetid: f528eee6-d5af-4745-8b00-a9834bf34be6
description: ReportTemplate 要素は、取得するレポートの種類を表します。
ms.openlocfilehash: 18fc98a8d9aaa777a590561aedd4e86fdf91f9af
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542801"
---
# <a name="reporttemplate"></a>ReportTemplate

**ReportTemplate 要素** は、取得するレポートの種類を表します。 
  
```xml
<ReportTemplate>Summary or RecipientPath</ReportTemplate>
```

 **MessageTrackingReportTemplateType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetMessageTrackingReport](getmessagetrackingreport.md) <br/> |指定した ID の完全なメッセージ追跡レポートを取得する [GetMessageTrackingReport](getmessagetrackingreport-operation.md) 操作の要求を格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に **、ReportTemplate** 要素に使用できる値を示します。 
  
**ReportTemplate 要素の値**

|**値**|**説明**|
|:-----|:-----|
|概要  <br/> |レポートにメッセージのすべての受信者と、メッセージの配信状態を各受信者に表示します。  <br/> |
|RecipientPath  <br/> |1 人の受信者に対して、発生したイベントの完全な履歴をレポートに表示するを指定します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

