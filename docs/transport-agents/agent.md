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
# <a name="agent"></a><span data-ttu-id="38e8c-103">エージェント</span><span class="sxs-lookup"><span data-stu-id="38e8c-103">agent</span></span>
  
<span data-ttu-id="38e8c-104">**に適用されます:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="38e8c-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="38e8c-105">**エージェント**の要素には、インストールされているエージェントの構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="38e8c-105">The **agent** element contains configuration information about an installed agent.</span></span> 
  
- [<span data-ttu-id="38e8c-106">構成</span><span class="sxs-lookup"><span data-stu-id="38e8c-106">configuration</span></span>](configuration.md) 
- [<span data-ttu-id="38e8c-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="38e8c-107">mexRuntime</span></span>](mexruntime.md)
- [<span data-ttu-id="38e8c-108">agentList</span><span class="sxs-lookup"><span data-stu-id="38e8c-108">agentList</span></span>](agentlist.md)
- [<span data-ttu-id="38e8c-109">エージェント</span><span class="sxs-lookup"><span data-stu-id="38e8c-109">agent</span></span>](agent.md)
  
```XML
<agent
        name=""
        baseType=""
        classFactory=""
        assemblyPath=""
        enabled="" />
</agent>
```

<span data-ttu-id="38e8c-110">**agentType (複合型)**</span><span class="sxs-lookup"><span data-stu-id="38e8c-110">**agentType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="38e8c-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="38e8c-111">Attributes and elements</span></span>

<span data-ttu-id="38e8c-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="38e8c-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38e8c-113">属性</span><span class="sxs-lookup"><span data-stu-id="38e8c-113">Attributes</span></span>

|<span data-ttu-id="38e8c-114">**属性**</span><span class="sxs-lookup"><span data-stu-id="38e8c-114">**Attribute**</span></span>|<span data-ttu-id="38e8c-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="38e8c-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="38e8c-116">**name**</span><span class="sxs-lookup"><span data-stu-id="38e8c-116">**name**</span></span> <br/> |<span data-ttu-id="38e8c-p101">エージェントのインストール時に指定された名前。この属性には、空でない文字列値が必要です (最大 64 文字)。</span><span class="sxs-lookup"><span data-stu-id="38e8c-p101">The name that was specified when the agent was installed. This attribute requires a nonempty string value that contains a maximum of 64 characters.</span></span>  <br/> |
|<span data-ttu-id="38e8c-119">**baseType**</span><span class="sxs-lookup"><span data-stu-id="38e8c-119">**baseType**</span></span> <br/> |<span data-ttu-id="38e8c-p102">エージェントの派生元クラスの完全な名前。名前空間も含みます。この属性には、少なくとも 1 文字以上の空でない文字列値が必要です。</span><span class="sxs-lookup"><span data-stu-id="38e8c-p102">The full name, including the namespace, of the class from which the agent derives. This attribute requires a nonempty string value that contains at least one character.</span></span>  <br/> |
|<span data-ttu-id="38e8c-122">**classFactory**</span><span class="sxs-lookup"><span data-stu-id="38e8c-122">**classFactory**</span></span> <br/> |<span data-ttu-id="38e8c-123">エージェントのインスタンスを作成するエージェントのファクトリを実装するクラスの名前空間を含む完全名です。</span><span class="sxs-lookup"><span data-stu-id="38e8c-123">The full name, including the namespace, of the class that implements the agent factory that creates instances of the agent.</span></span> <span data-ttu-id="38e8c-124">この属性には、エージェントのインスタンスを作成するエージェントのファクトリを実装するクラスの完全修飾名が含まれている必要があります。</span><span class="sxs-lookup"><span data-stu-id="38e8c-124">This attribute must contain the fully qualified name of the class that implements the agent factory that creates instances of the agent.</span></span> <span data-ttu-id="38e8c-125">このクラスは、 [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)または[RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)のいずれかのクラスから派生する必要があります。</span><span class="sxs-lookup"><span data-stu-id="38e8c-125">This class must derive from either the [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) or [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) class.</span></span>  <br/> |
|<span data-ttu-id="38e8c-126">**assemblyPath**</span><span class="sxs-lookup"><span data-stu-id="38e8c-126">**assemblyPath**</span></span> <br/> |<span data-ttu-id="38e8c-p104">エージェントのコードを含んでいるアセンブリの完全修飾パス。ファイル名も含みます。この属性には、少なくとも 1 文字以上の空でない文字列値が必要です。</span><span class="sxs-lookup"><span data-stu-id="38e8c-p104">The fully qualified path, including the file name, of the assembly that contains the code for the agent. This attribute requires a nonempty string value that contains at least one character.</span></span>  <br/> |
|<span data-ttu-id="38e8c-129">**有効になっています。**</span><span class="sxs-lookup"><span data-stu-id="38e8c-129">**enabled**</span></span> <br/> |<span data-ttu-id="38e8c-130">エージェントが有効になっているかどうかを示すブール値です。</span><span class="sxs-lookup"><span data-stu-id="38e8c-130">A Boolean value that indicates whether the agent is enabled.</span></span> <span data-ttu-id="38e8c-131">値が**true**の場合は、エージェントが有効になっています。それ以外の場合、値が**false**にします。</span><span class="sxs-lookup"><span data-stu-id="38e8c-131">The value is **true** if the agent is enabled; otherwise, the value is **false**.</span></span> <span data-ttu-id="38e8c-132">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="38e8c-132">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="38e8c-133">子要素</span><span class="sxs-lookup"><span data-stu-id="38e8c-133">Child elements</span></span>

<span data-ttu-id="38e8c-134">なし。</span><span class="sxs-lookup"><span data-stu-id="38e8c-134">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="38e8c-135">親要素</span><span class="sxs-lookup"><span data-stu-id="38e8c-135">Parent elements</span></span>

|<span data-ttu-id="38e8c-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="38e8c-136">**Element**</span></span>|<span data-ttu-id="38e8c-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="38e8c-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38e8c-138">agentList</span><span class="sxs-lookup"><span data-stu-id="38e8c-138">agentList</span></span>](agentlist.md) <br/> |<span data-ttu-id="38e8c-139">インストールされている各エージェントの**エージェント**の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="38e8c-139">Contains an **agent** element for each installed agent.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="38e8c-140">要素情報</span><span class="sxs-lookup"><span data-stu-id="38e8c-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38e8c-141">名前空間</span><span class="sxs-lookup"><span data-stu-id="38e8c-141">Namespace</span></span>  <br/> |<span data-ttu-id="38e8c-142">このファイルには名前空間が定義されていません。</span><span class="sxs-lookup"><span data-stu-id="38e8c-142">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="38e8c-143">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="38e8c-143">Schema Name</span></span>  <br/> |<span data-ttu-id="38e8c-144">該当なし。</span><span class="sxs-lookup"><span data-stu-id="38e8c-144">Not available.</span></span>  <br/> |
|<span data-ttu-id="38e8c-145">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="38e8c-145">Validation File</span></span>  <br/> |<span data-ttu-id="38e8c-146">該当なし。</span><span class="sxs-lookup"><span data-stu-id="38e8c-146">Not available.</span></span>  <br/> |
|<span data-ttu-id="38e8c-147">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="38e8c-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="38e8c-148">False。</span><span class="sxs-lookup"><span data-stu-id="38e8c-148">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="38e8c-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="38e8c-149">See also</span></span>

- [<span data-ttu-id="38e8c-150">Exchange 2013 のエージェント構成ファイルの要素</span><span class="sxs-lookup"><span data-stu-id="38e8c-150">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

