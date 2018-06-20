---
title: ルール
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Rules
api_type:
- schema
ms.assetid: 53f59054-8f68-4eaa-be9c-ccfc9383bcf2
description: ルール要素には、保護の規則の配列が含まれています。
ms.openlocfilehash: 5d511f977f3eb3273dc43f56356a059985b2a929
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833269"
---
# <a name="rules"></a>ルール

**ルール**要素には、保護の規則の配列が含まれています。 
  
```xml
<Rules>   <Rule/></Rules>
```

 **ArrayOfProtectionRulesType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[Rule](rule.md) <br/> |1 つの保護ルールが含まれています。 この要素に 0 回以上発生します。 この要素と保護のルールが定義されていない組織で 0 が発生します。 1 つ以上の時間は、組織が少なくとも 1 つのルールが定義されている場合に発生します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ProtectionRulesConfiguration](protectionrulesconfiguration.md) <br/> |保護ルールのサービスのサービスの構成が含まれています。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

