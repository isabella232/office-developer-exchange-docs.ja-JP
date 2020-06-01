---
title: ダン
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
description: Diagnostics 要素は、データセンターでのレポートに使用されるタイミングとパフォーマンスに関する情報を提供します。
ms.openlocfilehash: 9eb46ef7ceb877372aff9b029190af8c8d8115cd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467838"
---
# <a name="diagnostics"></a>ダン

**Diagnostics**要素は、データセンターでのレポートに使用されるタイミングとパフォーマンスに関する情報を提供します。 
  
```XML
<Diagnostics>
   <String/>
</Diagnostics>

```

 **ArrayOfStringsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[String](string.md) <br/> |アイテム、連絡先、タスク、会話で使用される文字列が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) <br/> |単一の[Findmessagetrackingreport 操作](findmessagetrackingreport-operation.md)要求の状態と結果を格納します。  <br/> |
|[GetMessageTrackingReportResponse](getmessagetrackingreportresponse.md) <br/> |[Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)に対する応答を格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [FindMessageTrackingReport 操作](findmessagetrackingreport-operation.md)
- [GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

