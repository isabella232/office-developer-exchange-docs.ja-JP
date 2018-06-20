---
title: messageSnapshot
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- messageSnapshot
api_type:
- schema
ms.assetid: f157e44c-b950-463f-b086-31d5da94b7ff
description: '最終更新日: 2015 年 9 月 17 日'
ms.openlocfilehash: 4b814def8eef8fb452d2e754c5f6787d644055f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759256"
---
# <a name="messagesnapshot"></a>messageSnapshot

**に適用されます:** Exchange Server 2013
  
**MessageSnapshot**要素には、クライアント アクセスまたはメールボックス サーバーの役割がインストールされている Exchange サーバーのパイプライン トレース機能が有効になっているかどうかを指定する属性が含まれています。 
  
- [構成](configuration.md)  
- [mexRuntime](mexruntime.md) 
- [監視](monitoring.md) 
- [messageSnapshot](messagesnapshot.md)
  
```XML
<messageSnapshot enabled="" />
```

**messageSnapshotType (ブール値)**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**有効になっています。** <br/> |クライアント アクセスまたはメールボックス サーバーのパイプライン トレース機能が有効になっているかどうかを示すブール値です。 値が**true**の場合、パイプライン トレースが有効になっています。それ以外の場合、値は**false**または、要素が存在しません。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[監視](monitoring.md) <br/> |トランスポート サービスがインストールされているエージェントを監視する方法とタイミングを定義する構成情報が含まれています。  <br/> |
   
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |このファイルには名前空間が定義されていません。  <br/> |
|スキーマ名  <br/> |該当なし。  <br/> |
|検証ファイル  <br/> |該当なし。  <br/> |
|空に設定可能  <br/> |False。  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange 2013 のエージェント構成ファイルの要素](agents-configuration-file-elements-for-exchange-2013.md)

