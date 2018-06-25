---
title: mexRuntime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- mexRuntime
api_type:
- schema
ms.assetid: eabb2f12-10a7-4ce2-ae4b-9c04010c765f
description: '最終更新日: 2015 年 9 月 17 日'
ms.openlocfilehash: 4a34eedfc16d64cbfa67003ed23cf6eba2bb4bad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759259"
---
# <a name="mexruntime"></a>mexRuntime
  
**に適用されます:** Exchange Server 2013
  
**MexRuntime**要素には、監視エージェントの構成情報および SMTP およびインストールされているルーティング エージェントの構成情報を定義する要素が含まれています。 
  
- [構成](configuration.md)  
- [mexRuntime](mexruntime.md)
  
```XML
<mexRuntime>
   <monitoring/>
   <agentList/>
</mexRuntime>
```

**mexRuntimeType (複合型)**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[監視](monitoring.md) <br/> |トランスポートがインストールされているエージェントを監視する方法とタイミングを定義する構成情報が含まれています。  <br/> |
|[agentList](agentlist.md) <br/> |インストールされている各エージェントの[エージェント](agent.md)の要素が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[構成](configuration.md) <br/> |エージェント構成ファイルのルート要素です。  <br/> |
   
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |このファイルには名前空間が定義されていません。  <br/> |
|スキーマ名  <br/> |該当なし。  <br/> |
|検証ファイル  <br/> |該当なし。  <br/> |
|空に設定可能  <br/> |False。  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange 2013 のエージェント構成ファイルの要素](agents-configuration-file-elements-for-exchange-2013.md)

