---
title: Diagnostics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Diagnostics
api_type:
- schema
ms.assetid: fecea440-970a-49da-9796-534ca470cbd6
description: 診断の要素は、データ ・ センターのレポートに使用されるタイミングとパフォーマンスの情報を提供します。
ms.openlocfilehash: 2b9cac54a683967ec274b8681fb9a0c8a844205e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760028"
---
# <a name="diagnostics"></a>Diagnostics

**診断**の要素は、データ ・ センターのレポートに使用されるタイミングとパフォーマンスの情報を提供します。 
  
```XML
<Diagnostics>
   <String/>
</Diagnostics>

```

 **ArrayOfStringsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[String](string.md) <br/> |アイテム、連絡先、タスク、および会話で使用される文字列が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) <br/> |状態および 1 つの結果が含まれています[FindMessageTrackingReport の操作](findmessagetrackingreport-operation.md)を要求します。  <br/> |
|[GetMessageTrackingReportResponse](getmessagetrackingreportresponse.md) <br/> |[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)の応答が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

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

- [FindMessageTrackingReport 操作](findmessagetrackingreport-operation.md)
- [GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

