---
title: agentExecution
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agentExecution
api_type:
- schema
ms.assetid: 600c4690-941c-45af-a906-5528748d09cd
description: '最終更新日: 2015 年 9 月 17 日'
ms.openlocfilehash: 5848d52a68c8c3f747614015e49becb34bc4cfd8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759225"
---
# <a name="agentexecution"></a>agentExecution
  
**に適用されます:** Exchange Server 2013 
  
**AgentExecution**要素は、エージェントがイベント ログに書き込む前にイベントを終了するまで待機するか、クライアント アクセス、メールボックス サーバーをミリ秒単位で時間を定義します。 
  
- [構成](configuration.md)  
- [監視](monitoring.md)
- [agentExecution](agentexecution.md)
  
```XML
<agentExecution timeLimitInMilliseconds="" />
```

**agentExecutionType (複合型)**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**timeLimitInMilliseconds** <br/> |エージェントのイベントからの復帰をサーバーが待機する時間をミリ秒単位で指定する正の整数値。この時間を過ぎるとイベント ログに警告が書き込まれます。この値が小さすぎると、パフォーマンスが低下することがあります。この属性の推奨値は、5 分間に相当する 300,000 です。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[監視](monitoring.md) <br/> |インストールされているエージェントをフロント エンド トランスポート サービスまたはトランスポート サービスが監視する方法とタイミングを定義する構成情報を格納します。  <br/> |
   
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |このファイルには名前空間が定義されていません。  <br/> |
|スキーマ名  <br/> |該当なし。  <br/> |
|検証ファイル  <br/> |該当なし。  <br/> |
|空に設定可能  <br/> |False。  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange 2013 のエージェント構成ファイルの要素](agents-configuration-file-elements-for-exchange-2013.md)

