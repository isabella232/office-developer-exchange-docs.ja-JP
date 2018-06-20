---
title: 状態 (MemberStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Status
api_type:
- schema
ms.assetid: 4f8a860b-0a48-4a0d-9a7a-69a0304aa747
description: 状態の要素は、サーバー上の配布リストのメンバーの状態に関する情報を提供します。
ms.openlocfilehash: ef062433c80f0cca413c33012e1164b17e226faf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833580"
---
# <a name="status-memberstatustype"></a>状態 (MemberStatusType)

**状態**の要素は、サーバー上の配布リストのメンバーの状態に関する情報を提供します。 
  
```
<Status>Unrecognized or Normal or Demoted</Status>
```

 **MemberStatusType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[メンバー](member-ex15websvcsotherref.md) <br/> |配布リストのメンバーを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**状態**の要素の値を次の表に一覧します。 
  
**要素のステータス値**

|**値**|**説明**|
|:-----|:-----|
|認識されません。  <br/> |メンバー情報は、無効なまたは認識されません。  <br/> |
|Normal  <br/> |配布リストのメンバー情報は、参照されるオブジェクトとの同期します。  <br/> |
|降格  <br/> |参照先のオブジェクトでは使用できません。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

