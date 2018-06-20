---
title: プロパティ (ArrayOfTrackingPropertiesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Properties
api_type:
- schema
ms.assetid: 175566d2-fd62-45a2-8518-2827912cec88
description: プロパティ要素には、1 つまたは複数の追跡のプロパティの一覧が含まれています。
ms.openlocfilehash: 079d2d2c101fdeb7f26d65798048c3c6c59f3e94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832897"
---
# <a name="properties-arrayoftrackingpropertiestype"></a>プロパティ (ArrayOfTrackingPropertiesType)

**プロパティ**要素には、1 つまたは複数の追跡のプロパティの一覧が含まれています。 
  
- [FindMessageTrackingReport](findmessagetrackingreport.md)
  
- [プロパティ (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md)
  
```xml
<Properties>
   <TrackingPropertyType/>
</Properties>
```

**ArrayOfTrackingPropertiesType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[TrackingPropertyType](trackingpropertytype.md) <br/> |名前と値文字列のペアを使用してレポートを追跡するメッセージのプロパティを作成するを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindMessageTrackingReport](findmessagetrackingreport.md) <br/> |検索するメッセージの種類の条件を指定します。  <br/> |
|[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) <br/> |状態および 1 つの結果が含まれています[FindMessageTrackingReport の操作](findmessagetrackingreport-operation.md)を要求します。  <br/> |
|[GetMessageTrackingReport](getmessagetrackingreport.md) <br/> |レポートを指定した ID の追跡を取得するために[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)の要求が含まれています  <br/> |
|[GetMessageTrackingReportResponse](getmessagetrackingreportresponse.md) <br/> |1 つの結果が含まれています[GetMessageTrackingReport の操作](getmessagetrackingreport-operation.md)を要求します。  <br/> |
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> |受信者の 1 つのイベントの情報が含まれています。  <br/> |
|[MessageTrackingReport](messagetrackingreport.md) <br/> |[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)で返される 1 つのメッセージが含まれています。  <br/> |
|[MessageTrackingSearchResult](messagetrackingsearchresult.md) <br/> |[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md)要素の 1 つのメッセージの結果が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [FindMessageTrackingReport 操作](findmessagetrackingreport-operation.md)
- [GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

