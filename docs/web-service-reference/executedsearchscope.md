---
title: ExecutedSearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExecutedSearchScope
api_type:
- schema
ms.assetid: 2de5f0ad-43f2-4d38-b520-06540066564e
description: ExecutedSearchScope 要素には、検索結果を得るために実行された検索の範囲が含まれています。
ms.openlocfilehash: ece9fdfc156cedad2a9fa181897145ae4eea20a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760367"
---
# <a name="executedsearchscope"></a>ExecutedSearchScope

**ExecutedSearchScope**要素には、検索結果を得るために実行された検索の範囲が含まれています。 
  
```xml
<ExecutedSearchScope/>
```

 **文字列型 (String)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) <br/> |状態および 1 つの結果が含まれています[FindMessageTrackingReport の操作](findmessagetrackingreport-operation.md)を要求します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は省略可能です。 この情報より効果的に結果をキャッシュするのには、クライアント アプリケーションによって使用されます。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[FindMessageTrackingReport 操作](findmessagetrackingreport-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

