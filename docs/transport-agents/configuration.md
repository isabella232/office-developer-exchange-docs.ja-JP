---
title: 構成
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- configuration
api_type:
- schema
ms.assetid: 6fc04e4d-657a-4999-9431-186ccb7832b5
description: '最終更新日: 2015 年 9 月 17 日'
ms.openlocfilehash: 342e52e879534b6a130d286d358138c6095e4563
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759229"
---
# <a name="configuration"></a>configuration
  
**に適用されます:** Exchange Server 2013
  
**構成**要素は、エージェント構成ファイルのルート要素です。 
  
- [構成](configuration.md) 
- [mexRuntime](mexruntime.md)
  
```XML
<configuration>
      <mexRuntime/>
</configuration>
```

**configurationType (複合型)**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[mexRuntime](mexruntime.md) <br/> |エージェントの監視に関する構成情報を定義する要素と、インストールされているエージェントの SMTP およびルーティングに関する構成情報を定義する要素を格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |このファイルには名前空間が定義されていません。  <br/> |
|スキーマ名  <br/> |該当なし。  <br/> |
|検証ファイル  <br/> |該当なし。  <br/> |
|空に設定可能  <br/> |False。  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange 2013 のエージェント構成ファイルの要素](agents-configuration-file-elements-for-exchange-2013.md)

