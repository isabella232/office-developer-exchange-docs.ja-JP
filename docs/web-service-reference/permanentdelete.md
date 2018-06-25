---
title: PermanentDelete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermanentDelete
api_type:
- schema
ms.assetid: 1a0e0f46-1472-4eb7-bb54-f193a2603587
description: PermanentDelete 要素は、メッセージを完全に削除され、削除済みアイテム フォルダーに保存されませんにするかどうかを示します。
ms.openlocfilehash: 40cf80e054bb70a3f6d687e8d4361f1d4331a7f8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832724"
---
# <a name="permanentdelete"></a>PermanentDelete

**PermanentDelete**要素は、メッセージを完全に削除され、削除済みアイテム フォルダーに保存されませんにするかどうかを示します。 
  
```XML
<PermanentDelete>true | false</PermanentDelete>
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

**True**の場合、テキスト値は完全に削除するメッセージをマークする必要があることを示します。 **False**の値は、メッセージが完全に削除するのにはマークされていない必要があることを示します。 
  
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

