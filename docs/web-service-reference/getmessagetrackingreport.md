---
title: GetMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMessageTrackingReport
api_type:
- schema
ms.assetid: b6ffa8ef-90f6-402d-afac-c3f5ee55cf49
description: GetMessageTrackingReport 要素には、指定した ID のレポートを追跡する、完全なメッセージを取得するために GetMessageTrackingReport 操作の要求が含まれています。
ms.openlocfilehash: cb16f6e9d322cefb0d59c962af8e2f60ebae0e90
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760796"
---
# <a name="getmessagetrackingreport"></a>GetMessageTrackingReport

**GetMessageTrackingReport**要素には、指定した ID のレポートを追跡する、完全なメッセージを取得するために[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)の要求が含まれています。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[スコープ (NonEmptyStringType)](scope-nonemptystringtype.md) <br/> |検索を実行する場所を指定します。 この要素は必須です。  <br/> |
|[ReportTemplate](reporttemplate.md) <br/> |追跡を取得するレポートの種類を指定します。 この要素は必須です。  <br/> |
|[RecipientFilter](recipientfilter.md) <br/> |指定した追跡レポートで使用する受信者のアドレスを指定します。 この要素はオプションです。  <br/> |
|[MessageTrackingReportId](messagetrackingreportid.md) <br/> |**FindMessageTrackingReport**操作から取得された id 文字列を指定します。 この要素は必須です。  <br/> |
|[ReturnQueueEvents](returnqueueevents.md) <br/> |タスクを実行している人が特権を持つ役割を持っているかを指定します。 この要素はオプションです。  <br/> |
|[DiagnosticsLevel](diagnosticslevel.md) <br/> |追跡レポートを派生させるために使用されるタイミングとパフォーマンスの情報を指定します。 この要素はオプションです。  <br/> |
|[プロパティ (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |1 つまたは複数の追跡のプロパティの一覧を指定します。 この要素はオプションです。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

