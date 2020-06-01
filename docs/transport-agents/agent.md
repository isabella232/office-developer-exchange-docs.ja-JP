---
title: agent
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
description: '最終更新日: 2015 年9月17日'
ms.openlocfilehash: a810bb229015054e0f244773760235114655a982
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455682"
---
# <a name="agent"></a><span data-ttu-id="0769c-103">agent</span><span class="sxs-lookup"><span data-stu-id="0769c-103">agent</span></span>
  
<span data-ttu-id="0769c-104">**製品:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="0769c-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="0769c-105">**agent** 要素には、インストールされているエージェントの構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0769c-105">The **agent** element contains configuration information about an installed agent.</span></span> 
  
- [<span data-ttu-id="0769c-106">構成</span><span class="sxs-lookup"><span data-stu-id="0769c-106">configuration</span></span>](configuration.md) 
- [<span data-ttu-id="0769c-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="0769c-107">mexRuntime</span></span>](mexruntime.md)
- [<span data-ttu-id="0769c-108">agentList</span><span class="sxs-lookup"><span data-stu-id="0769c-108">agentList</span></span>](agentlist.md)
- [<span data-ttu-id="0769c-109">agent</span><span class="sxs-lookup"><span data-stu-id="0769c-109">agent</span></span>](agent.md)
  
```XML
<agent
        name=""
        baseType=""
        classFactory=""
        assemblyPath=""
        enabled="" />
</agent>
```

<span data-ttu-id="0769c-110">**agentType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="0769c-110">**agentType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0769c-111">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0769c-111">Attributes and elements</span></span>

<span data-ttu-id="0769c-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0769c-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0769c-113">属性</span><span class="sxs-lookup"><span data-stu-id="0769c-113">Attributes</span></span>

|<span data-ttu-id="0769c-114">**属性**</span><span class="sxs-lookup"><span data-stu-id="0769c-114">**Attribute**</span></span>|<span data-ttu-id="0769c-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="0769c-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0769c-116">**name**</span><span class="sxs-lookup"><span data-stu-id="0769c-116">**name**</span></span> <br/> |<span data-ttu-id="0769c-117">エージェントのインストール時に指定された名前。</span><span class="sxs-lookup"><span data-stu-id="0769c-117">The name that was specified when the agent was installed.</span></span> <span data-ttu-id="0769c-118">この属性には、空でない文字列値が必要です (最大 64 文字)。</span><span class="sxs-lookup"><span data-stu-id="0769c-118">This attribute requires a nonempty string value that contains a maximum of 64 characters.</span></span>  <br/> |
|<span data-ttu-id="0769c-119">**baseType**</span><span class="sxs-lookup"><span data-stu-id="0769c-119">**baseType**</span></span> <br/> |<span data-ttu-id="0769c-p102">エージェントの派生元クラスの完全な名前。名前空間も含みます。この属性には、少なくとも 1 文字以上の空でない文字列値が必要です。</span><span class="sxs-lookup"><span data-stu-id="0769c-p102">The full name, including the namespace, of the class from which the agent derives. This attribute requires a nonempty string value that contains at least one character.</span></span>  <br/> |
|<span data-ttu-id="0769c-122">**classFactory**</span><span class="sxs-lookup"><span data-stu-id="0769c-122">**classFactory**</span></span> <br/> |<span data-ttu-id="0769c-123">エージェントのインスタンスを作成するエージェントファクトリを実装するクラスの名前空間を含む完全な名前。</span><span class="sxs-lookup"><span data-stu-id="0769c-123">The full name, including the namespace, of the class that implements the agent factory that creates instances of the agent.</span></span> <span data-ttu-id="0769c-124">この属性には、エージェントのインスタンスを作成するエージェントファクトリを実装するクラスの完全修飾名を含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="0769c-124">This attribute must contain the fully qualified name of the class that implements the agent factory that creates instances of the agent.</span></span> <span data-ttu-id="0769c-125">このクラスは、 [Smtpreceiveagentfactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)または[routingagentfactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)クラスから派生する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0769c-125">This class must derive from either the [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) or [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) class.</span></span>  <br/> |
|<span data-ttu-id="0769c-126">**assemblyPath**</span><span class="sxs-lookup"><span data-stu-id="0769c-126">**assemblyPath**</span></span> <br/> |<span data-ttu-id="0769c-p104">エージェントのコードを含んでいるアセンブリの完全修飾パス。ファイル名も含みます。この属性には、少なくとも 1 文字以上の空でない文字列値が必要です。</span><span class="sxs-lookup"><span data-stu-id="0769c-p104">The fully qualified path, including the file name, of the assembly that contains the code for the agent. This attribute requires a nonempty string value that contains at least one character.</span></span>  <br/> |
|<span data-ttu-id="0769c-129">**enabled**</span><span class="sxs-lookup"><span data-stu-id="0769c-129">**enabled**</span></span> <br/> |<span data-ttu-id="0769c-130">エージェントが有効かどうかを示すブール値。</span><span class="sxs-lookup"><span data-stu-id="0769c-130">A Boolean value that indicates whether the agent is enabled.</span></span> <span data-ttu-id="0769c-131">エージェントが有効な場合の値は **true**、それ以外の場合の値は **false** です。</span><span class="sxs-lookup"><span data-stu-id="0769c-131">The value is **true** if the agent is enabled; otherwise, the value is **false**.</span></span> <span data-ttu-id="0769c-132">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="0769c-132">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0769c-133">子要素</span><span class="sxs-lookup"><span data-stu-id="0769c-133">Child elements</span></span>

<span data-ttu-id="0769c-134">なし。</span><span class="sxs-lookup"><span data-stu-id="0769c-134">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0769c-135">親要素</span><span class="sxs-lookup"><span data-stu-id="0769c-135">Parent elements</span></span>

|<span data-ttu-id="0769c-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="0769c-136">**Element**</span></span>|<span data-ttu-id="0769c-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="0769c-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0769c-138">agentList</span><span class="sxs-lookup"><span data-stu-id="0769c-138">agentList</span></span>](agentlist.md) <br/> |<span data-ttu-id="0769c-139">インストールされたエージェントごとに **agent** 要素を格納します。</span><span class="sxs-lookup"><span data-stu-id="0769c-139">Contains an **agent** element for each installed agent.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="0769c-140">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0769c-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0769c-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="0769c-141">Namespace</span></span>  <br/> |<span data-ttu-id="0769c-142">このファイルには名前空間が定義されていません。</span><span class="sxs-lookup"><span data-stu-id="0769c-142">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="0769c-143">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0769c-143">Schema Name</span></span>  <br/> |<span data-ttu-id="0769c-144">注意事項なし。</span><span class="sxs-lookup"><span data-stu-id="0769c-144">Not available.</span></span>  <br/> |
|<span data-ttu-id="0769c-145">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0769c-145">Validation File</span></span>  <br/> |<span data-ttu-id="0769c-146">該当なし。</span><span class="sxs-lookup"><span data-stu-id="0769c-146">Not available.</span></span>  <br/> |
|<span data-ttu-id="0769c-147">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0769c-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="0769c-148">不正解。</span><span class="sxs-lookup"><span data-stu-id="0769c-148">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0769c-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="0769c-149">See also</span></span>

- [<span data-ttu-id="0769c-150">Exchange 2013 のエージェント構成ファイルの要素</span><span class="sxs-lookup"><span data-stu-id="0769c-150">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

