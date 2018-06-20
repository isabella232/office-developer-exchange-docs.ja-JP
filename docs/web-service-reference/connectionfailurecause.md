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
description: ConnectionFailureCause 要素は、電話の呼び出しからの切断の理由を指定します。
ms.openlocfilehash: 54b4f5b89efdb42ef82dbef8f1af14a39c0ccc6a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759658"
---
# <a name="connectionfailurecause"></a>ConnectionFailureCause

**ConnectionFailureCause**要素は、電話の呼び出しからの切断の理由を指定します。 
  
```xml
<ConnectionFailureCause>None or UserBusy or NoAnswer or Unavailable or Other</ConnectionFailureCause>
```

 **ConnectionFailureCauseType**
## <a name="attributes-and-elements"></a>属性および要素

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

次の表は、 **ConnectionFailureCause**要素の値を一覧します。 
  
**ConnectionFailureCause 要素の値**

|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |呼び出しの状態が切り離されていないか、切断の理由が不明です。  <br/> |
|UserBusy  <br/> |呼ばれるパーティの回線がビジー状態でした。  <br/> |
|NoAnswer  <br/> |呼に応答しませんでした。  <br/> |
|使用できない  <br/> |呼び出し先の番号は使用できませんでした。  <br/> |
|その他  <br/> |切断の理由には、キャッチ オール。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

