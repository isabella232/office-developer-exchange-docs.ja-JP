---
title: ConnectionFailureCause
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectionFailureCause
api_type:
- schema
ms.assetid: d2160c8a-015c-4964-b7f7-93478764a173
description: ConnectionFailureCause 要素は、電話から切断した理由を指定します。
ms.openlocfilehash: 6385641eaee140a114906703232974d51d5ce344
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529449"
---
# <a name="connectionfailurecause"></a>ConnectionFailureCause

**ConnectionFailureCause**要素は、電話から切断した理由を指定します。 
  
```xml
<ConnectionFailureCause>None or UserBusy or NoAnswer or Unavailable or Other</ConnectionFailureCause>
```

 **ConnectionFailureCauseType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[PhoneCallInformation](phonecallinformation.md) <br/> |通話の状態情報を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に、 **ConnectionFailureCause**要素に指定できる値を示します。 
  
**ConnectionFailureCause 要素の値**

|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |呼び出しの状態が切断されていないか、切断の理由が不明です。  <br/> |
|UserBusy  <br/> |呼び出し先の回線がビジー状態でした。  <br/> |
|NoAnswer  <br/> |呼び出し先は応答しませんでした。  <br/> |
|使用できない  <br/> |呼び出し先番号が使用できませんでした。  <br/> |
|その他  <br/> |他の切断の理由からキャッチします。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

