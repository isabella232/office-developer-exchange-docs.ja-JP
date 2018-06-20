---
title: IsNDR
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsNDR
api_type:
- schema
ms.assetid: 194f5836-7793-463a-a090-4386d1c2487a
description: IsNDR 要素は、受信メッセージが配信不能レポート (Ndr) をする必要があるかどうかを示しますを適用する場合の条件または例外の順序で。
ms.openlocfilehash: 651590d055a0532c904dbf6c481dca2f899d673f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832056"
---
# <a name="isndr"></a>IsNDR

**IsNDR**要素は、受信メッセージが配信不能レポート (Ndr) をする必要があるかどうかを示しますを適用する場合の条件または例外の順序で。 
  
```XML
<IsNDR>true | false</IsNDR>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[条件](conditions.md) <br/> |条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。  <br/> |
|[Exceptions](exceptions.md) <br/> |受信トレイ ルールの使用可能なルールの例外条件をすべてを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**True**の場合、テキスト値は、メッセージは NDR を適用する場合の条件または例外の順序のである必要があることを示します。 **False**の値は、メッセージが NDR を適用する場合の条件または例外の順にする必要がありますできないことを示します。 
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

