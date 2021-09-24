---
title: GetMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetMessageTrackingReport
api_type:
- schema
ms.assetid: b6ffa8ef-90f6-402d-afac-c3f5ee55cf49
description: GetMessageTrackingReport 要素には、指定した ID の完全なメッセージ追跡レポートを取得する GetMessageTrackingReport 操作の要求が含まれる。
ms.openlocfilehash: cdf4e2c0f17c7d723dc56f30c445bfd527f891a3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516980"
---
# <a name="getmessagetrackingreport"></a>GetMessageTrackingReport

**GetMessageTrackingReport** 要素には、指定した ID の完全なメッセージ追跡レポートを取得する [GetMessageTrackingReport](getmessagetrackingreport-operation.md)操作の要求が含まれる。 
  
```XML
<GetMessageTrackingReport>
   <Scope/>
   <ReportTemplate/>
   <RecipientFilter/>
   <MessageTrackingReportId/>
   <ReturnQueueEvents/>
   <DiagnosticsLevel/>
   <Properties/>
</GetMessageTrackingReport>
```

 **GetMessageTrackingReportRequestType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Scope (NonEmptyStringType)](scope-nonemptystringtype.md) <br/> |検索を実行する場所を指定します。 この要素は必須です。  <br/> |
|[ReportTemplate](reporttemplate.md) <br/> |取得する追跡レポートの種類を指定します。 この要素は必須です。  <br/> |
|[RecipientFilter](recipientfilter.md) <br/> |指定した追跡レポートで使用する受信者アドレスを指定します。 この要素は省略できます。  <br/> |
|[MessageTrackingReportId](messagetrackingreportid.md) <br/> |**FindMessageTrackingReport** 操作から取得した ID 文字列を指定します。 この要素は必須です。  <br/> |
|[ReturnQueueEvents](returnqueueevents.md) <br/> |タスクを実行しているユーザーに特権ロールが割り当てられています。 この要素は省略できます。  <br/> |
|[DiagnosticsLevel](diagnosticslevel.md) <br/> |追跡レポートの派生に使用するタイミングとパフォーマンスの情報を指定します。 この要素は省略できます。  <br/> |
|[Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |1 つ以上の追跡プロパティの一覧を指定します。 この要素は省略できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
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



[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

