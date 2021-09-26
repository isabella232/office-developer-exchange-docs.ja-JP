---
title: ConnectionFailureCause
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConnectionFailureCause
api_type:
- schema
ms.assetid: d2160c8a-015c-4964-b7f7-93478764a173
description: ConnectionFailureCause 要素は、電話からの切断の理由を指定します。
ms.openlocfilehash: de2f06ae89577b0141b8555f98dba1671a228d45
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543535"
---
# <a name="connectionfailurecause"></a>ConnectionFailureCause

**ConnectionFailureCause 要素** は、電話からの切断の理由を指定します。 
  
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
|[PhoneCallInformation](phonecallinformation.md) <br/> |電話の状態情報を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に **、ConnectionFailureCause 要素で使用できる値を示** します。 
  
**ConnectionFailure 要素の値**

|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |通話状態が切断されていないか、切断理由が分かっていない。  <br/> |
|UserBusy  <br/> |呼び出されたパーティ行がビジー状態でした。  <br/> |
|NoAnswer  <br/> |呼び出されたパーティが応答しなかった。  <br/> |
|使用できない  <br/> |呼び出されたパーティ番号は使用できません。  <br/> |
|その他  <br/> |その他の切断の理由でキャッチオール。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

