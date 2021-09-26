---
title: Properties (ArrayOfTrackingPropertiesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Properties
api_type:
- schema
ms.assetid: 175566d2-fd62-45a2-8518-2827912cec88
description: Properties 要素には、1 つ以上の追跡プロパティの一覧が含まれる。
ms.openlocfilehash: 8232b94effe3aae5b07be12bdaf1b5e85331938f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542982"
---
# <a name="properties-arrayoftrackingpropertiestype"></a>Properties (ArrayOfTrackingPropertiesType)

**Properties 要素には**、1 つ以上の追跡プロパティの一覧が含まれる。 
  
- [FindMessageTrackingReport](findmessagetrackingreport.md)
  
- [Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md)
  
```xml
<Properties>
   <TrackingPropertyType/>
</Properties>
```

**ArrayOfTrackingPropertiesType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[TrackingPropertyType](trackingpropertytype.md) <br/> |メッセージ追跡レポートのプロパティの作成に使用される文字列の名前と値のペアを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindMessageTrackingReport](findmessagetrackingreport.md) <br/> |検索するメッセージの種類の条件を指定します。  <br/> |
|[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) <br/> |1 つの [FindMessageTrackingReport](findmessagetrackingreport-operation.md) 操作要求の状態と結果を格納します。  <br/> |
|[GetMessageTrackingReport](getmessagetrackingreport.md) <br/> |指定した ID の完全なメッセージ追跡レポートを取得する [GetMessageTrackingReport](getmessagetrackingreport-operation.md) 操作の要求を格納します。  <br/> |
|[GetMessageTrackingReportResponse](getmessagetrackingreportresponse.md) <br/> |1 つの [GetMessageTrackingReport 操作要求の結果を格納](getmessagetrackingreport-operation.md) します。  <br/> |
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> |受信者の 1 つのイベントの情報を格納します。  <br/> |
|[MessageTrackingReport](messagetrackingreport.md) <br/> |[GetMessageTrackingReport](getmessagetrackingreport-operation.md)操作で返される 1 つのメッセージを格納します。  <br/> |
|[MessageTrackingSearchResult](messagetrackingsearchresult.md) <br/> |[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md)要素の 1 つのメッセージ結果を含む。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web Services をホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [FindMessageTrackingReport 操作](findmessagetrackingreport-operation.md)
- [GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

