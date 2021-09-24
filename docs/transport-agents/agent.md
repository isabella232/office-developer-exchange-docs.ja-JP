---
title: agent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- agent
api_type:
- schema
ms.assetid: 0bf744a5-9d79-4c82-8ea7-45fdb3f55300
description: '最終更新日: 2015 年 9 月 17 日'
ms.openlocfilehash: 8bcfdd9bffd4c7a15af40528fd431a99c7868637
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520969"
---
# <a name="agent"></a>agent
  
**製品:** Exchange Server 2013
  
**agent** 要素には、インストールされているエージェントの構成情報が含まれています。 
  
- [構成](configuration.md) 
- [mexRuntime](mexruntime.md)
- [agentList](agentlist.md)
- [エージェント](agent.md)
  
```XML
<agent
        name=""
        baseType=""
        classFactory=""
        assemblyPath=""
        enabled="" />
</agent>
```

**agentType (complexType)**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**name** <br/> |エージェントのインストール時に指定された名前。この属性には、空でない文字列値が必要です (最大 64 文字)。  <br/> |
|**baseType** <br/> |エージェントの派生元クラスの完全な名前。名前空間も含みます。この属性には、少なくとも 1 文字以上の空でない文字列値が必要です。  <br/> |
|**classFactory** <br/> |エージェントのインスタンスを作成するエージェント ファクトリを実装するクラスの名前空間を含む完全な名前。 この属性には、エージェントのインスタンスを作成するエージェント ファクトリを実装するクラスの完全修飾名が含まれている必要があります。 このクラスは [、SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) クラスまたは [RoutingAgentFactory クラスから派生する必要](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) があります。  <br/> |
|**assemblyPath** <br/> |エージェントのコードを含んでいるアセンブリの完全修飾パス。ファイル名も含みます。この属性には、少なくとも 1 文字以上の空でない文字列値が必要です。  <br/> |
|**enabled** <br/> |エージェントが有効かどうかを示すブール値。エージェントが有効な場合の値は **true**、それ以外の場合の値は **false** です。この属性は必須です。<br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[agentList](agentlist.md) <br/> |インストールされたエージェントごとに **agent** 要素を格納します。  <br/> |
   
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |このファイルには名前空間が定義されていません。  <br/> |
|スキーマ名  <br/> |該当なし。  <br/> |
|検証ファイル  <br/> |該当なし。  <br/> |
|空に設定可能  <br/> |不正解。  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange 2013 のエージェント構成ファイルの要素](agents-configuration-file-elements-for-exchange-2013.md)

