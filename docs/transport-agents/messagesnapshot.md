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
description: '最終更新日: 2015 年9月17日'
ms.openlocfilehash: 8a58444580c803efb7312df95d75d697bc42e8e0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461843"
---
# <a name="messagesnapshot"></a>messageSnapshot

**製品:** Exchange Server 2013
  
**messageSnapshot** 要素には、クライアント アクセスやメールボックス サーバーの役割がインストールされている Exchange サーバーでパイプライン トレース機能を使えるようにするかどうかを指定する属性が含まれています。 
  
- [構成](configuration.md)  
- [mexRuntime](mexruntime.md) 
- [管理](monitoring.md) 
- [messageSnapshot](messagesnapshot.md)
  
```XML
<messageSnapshot enabled="" />
```

**messageSnapshotType (ブール値)**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**enabled** <br/> |クライアントアクセスまたはメールボックスサーバーに対してパイプライントレース機能が有効になっているかどうかを示すブール値。 パイプライントレースが有効になっている場合、値は**true**になります。それ以外の場合、値は**false**になるか、要素が存在しないことを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[管理](monitoring.md) <br/> |トランスポート サービスがインストールされているエージェントを監視する方法とタイミングを定義する構成情報が含まれています。  <br/> |
   
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |このファイルには名前空間が定義されていません。  <br/> |
|スキーマ名  <br/> |注意事項なし。  <br/> |
|検証ファイル  <br/> |該当なし。  <br/> |
|空に設定可能  <br/> |不正解。  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange 2013 のエージェント構成ファイルの要素](agents-configuration-file-elements-for-exchange-2013.md)

