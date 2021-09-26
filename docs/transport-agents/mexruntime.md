---
title: mexRuntime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- mexRuntime
api_type:
- schema
ms.assetid: eabb2f12-10a7-4ce2-ae4b-9c04010c765f
description: '最終更新日: 2015 年 9 月 17 日'
ms.openlocfilehash: c7ae630a01ac0339433a7c78859c06006efab4b5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546911"
---
# <a name="mexruntime"></a>mexRuntime
  
**製品:** Exchange Server 2013
  
**mexRuntime** 要素には、エージェントの監視に関する構成情報を定義する要素と、SMTP とインストールされている ルーティング エージェントに関する構成情報を定義する要素が含まれます。 
  
- [構成](configuration.md)  
- [mexRuntime](mexruntime.md)
  
```XML
<mexRuntime>
   <monitoring/>
   <agentList/>
</mexRuntime>
```

**mexRuntimeType (complexType)**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[監視](monitoring.md) <br/> |トランスポートがインストールされているエージェントを監視する方法とタイミングを定義する構成情報が含まれています。  <br/> |
|[agentList](agentlist.md) <br/> |インストールされている各エージェントの [agent](agent.md) 要素が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[configuration](configuration.md) <br/> |エージェント構成ファイルのルート要素です。  <br/> |
   
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |このファイルには名前空間が定義されていません。  <br/> |
|スキーマ名  <br/> |該当なし。  <br/> |
|検証ファイル  <br/> |該当なし。  <br/> |
|空に設定可能  <br/> |不正解。  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange 2013 のエージェント構成ファイルの要素](agents-configuration-file-elements-for-exchange-2013.md)

