---
title: MarkAsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MarkAsRead
api_type:
- schema
ms.assetid: 404842e1-fbdb-480d-a1d8-ba1ab2c9fb1e
description: MarkAsRead 要素は、メッセージを既読としてマークするかどうかを示します。
ms.openlocfilehash: b453ad73912e99b6fd3aed84b03a7d2fc2b6a294
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832355"
---
# <a name="markasread"></a>MarkAsRead

**MarkAsRead**要素は、メッセージを既読としてマークするかどうかを示します。 
  
```XML
<MarkAsRead>true | false</MarkAsRead>
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
|[アクション](actions.md) <br/> |条件が満たされるときに、メッセージに対して実行される使用可能なアクションのセットを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**True**の場合、テキスト値は、メッセージは開封としてマークする必要があることを示します。 **False**の値は、メッセージが既読としてマークされていない必要があることを示します。 
  
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

