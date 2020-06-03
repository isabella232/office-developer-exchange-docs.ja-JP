---
title: Status (MemberStatusType)
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
description: Status 要素は、サーバー上の配布リストのメンバーの状態に関する情報を提供します。
ms.openlocfilehash: bfa0c349d6af51c1b2238c9749d2656541d31906
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465465"
---
# <a name="status-memberstatustype"></a>Status (MemberStatusType)

**Status**要素は、サーバー上の配布リストのメンバーの状態に関する情報を提供します。 
  
```
<Status>Unrecognized or Normal or Demoted</Status>
```

 **MemberStatusType**
## <a name="attributes-and-elements"></a>属性と要素

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

次の表に、 **Status**要素に指定できる値を示します。 
  
**Status 要素の値**

|**値**|**説明**|
|:-----|:-----|
|認識できない  <br/> |メンバー情報が無効であるか、認識されません。  <br/> |
|標準  <br/> |配布リスト内のメンバー情報は、参照されているオブジェクトと同期しています。  <br/> |
|差し戻し  <br/> |参照されるオブジェクトは使用できません。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

