---
title: ViewPrivateItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ViewPrivateItems
api_type:
- schema
ms.assetid: 80b949ac-440c-4a01-b428-ebafb5b1b802
description: ViewPrivateItems 要素は、代理人のユーザーまたはクライアント アプリケーションが主体のメールボックスにプライベート アイテムを表示する権限を持つかどうかを示します。
ms.openlocfilehash: c35f24ae79e907424cb5cfb0efeec2307334ca12
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839994"
---
# <a name="viewprivateitems"></a>ViewPrivateItems

**ViewPrivateItems**要素は、代理人のユーザーまたはクライアント アプリケーションが主体のメールボックスにプライベート アイテムを表示する権限を持つかどうかを示します。 
  
```XML
<ViewPrivateItems>true | false</ViewPrivateItems>
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
|[DelegateUser](delegateuser.md) <br/> |1 つのデリゲートを追加するメールボックスの更新を識別します。  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。 この要素は、読み取り専用です。  <br/> |
   
## <a name="text-value"></a>テキスト値

**True**の場合、代理人またはクライアント アイテムを表示できますプライベート主体のメールボックス内を示します。 **False**の値は、プライベートなアイテムが、代理人またはクライアントに表示されていないことを示します。 
  
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



[AddDelegate 操作](adddelegate-operation.md)
  
[UpdateDelegate 操作](updatedelegate-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


[デリゲートを追加します。](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

