---
title: messageSnapshot
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- messageSnapshot
api_type:
- schema
ms.assetid: f157e44c-b950-463f-b086-31d5da94b7ff
description: '最終更新日: 2015 年 9 月 17 日'
ms.openlocfilehash: 2ac38dd3f50b5d9d070262f3daffb72b02df5d82
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525457"
---
# <a name="messagesnapshot"></a>messageSnapshot

**製品:** Exchange Server 2013
  
**messageSnapshot** 要素には、クライアント アクセスやメールボックス サーバーの役割がインストールされている Exchange サーバーでパイプライン トレース機能を使えるようにするかどうかを指定する属性が含まれています。 
  
- [構成](configuration.md)  
- [mexRuntime](mexruntime.md) 
- [監視](monitoring.md) 
- [messageSnapshot](messagesnapshot.md)
  
```XML
<messageSnapshot enabled="" />
```

**messageSnapshotType (Boolean)**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**enabled** <br/> |クライアント アクセスやメールボックス サーバーのパイプライン トレース機能を使えるようするかどうかを指定するブール値。この値は、パイプライン トレース機能が使える場合には **true**。それ以外の場合やこの要素が存在しない場合には **false** です。<br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[監視](monitoring.md) <br/> |トランスポート サービスがインストールされているエージェントを監視する方法とタイミングを定義する構成情報が含まれています。  <br/> |
   
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |このファイルには名前空間が定義されていません。  <br/> |
|スキーマ名  <br/> |該当なし。  <br/> |
|検証ファイル  <br/> |該当なし。  <br/> |
|空に設定可能  <br/> |不正解。  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange 2013 のエージェント構成ファイルの要素](agents-configuration-file-elements-for-exchange-2013.md)

