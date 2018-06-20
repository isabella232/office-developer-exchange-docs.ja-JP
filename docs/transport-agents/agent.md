---
title: エージェント
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agent
api_type:
- schema
ms.assetid: 0bf744a5-9d79-4c82-8ea7-45fdb3f55300
description: '最終更新日: 2015 年 9 月 17 日'
ms.openlocfilehash: 3895095ed4e469cdb9fec489ba6b6e228779a9c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759228"
---
# <a name="agent"></a>エージェント
  
**に適用されます:** Exchange Server 2013
  
**エージェント**の要素には、インストールされているエージェントの構成情報が含まれています。 
  
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

**agentType (複合型)**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**name** <br/> |エージェントのインストール時に指定された名前。この属性には、空でない文字列値が必要です (最大 64 文字)。  <br/> |
|**baseType** <br/> |エージェントの派生元クラスの完全な名前。名前空間も含みます。この属性には、少なくとも 1 文字以上の空でない文字列値が必要です。  <br/> |
|**classFactory** <br/> |エージェントのインスタンスを作成するエージェントのファクトリを実装するクラスの名前空間を含む完全名です。 この属性には、エージェントのインスタンスを作成するエージェントのファクトリを実装するクラスの完全修飾名が含まれている必要があります。 このクラスは、 [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)または[RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)のいずれかのクラスから派生する必要があります。  <br/> |
|**assemblyPath** <br/> |エージェントのコードを含んでいるアセンブリの完全修飾パス。ファイル名も含みます。この属性には、少なくとも 1 文字以上の空でない文字列値が必要です。  <br/> |
|**有効になっています。** <br/> |エージェントが有効になっているかどうかを示すブール値です。 値が**true**の場合は、エージェントが有効になっています。それ以外の場合、値が**false**にします。 この属性は、必要があります。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[agentList](agentlist.md) <br/> |インストールされている各エージェントの**エージェント**の要素が含まれています。  <br/> |
   
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |このファイルには名前空間が定義されていません。  <br/> |
|スキーマ名  <br/> |該当なし。  <br/> |
|検証ファイル  <br/> |該当なし。  <br/> |
|空に設定可能  <br/> |False。  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange 2013 のエージェント構成ファイルの要素](agents-configuration-file-elements-for-exchange-2013.md)

