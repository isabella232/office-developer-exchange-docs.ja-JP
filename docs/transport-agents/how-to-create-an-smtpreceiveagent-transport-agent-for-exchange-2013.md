---
title: Exchange 2013 用の SmtpReceiveAgent トランスポートエージェントを作成する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cdc7c462-74a7-49d6-95b2-155d783840e9
description: Exchange 2013 で使用する、カスタムの SmtpReceiveAgent トランスポートエージェントを作成する方法について説明します。
ms.openlocfilehash: 5ba021d02849ffc7e125029f0fd18ebf14c3f8da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459140"
---
# <a name="create-an-smtpreceiveagent-transport-agent-for-exchange-2013"></a><span data-ttu-id="b42dc-103">Exchange 2013 用の SmtpReceiveAgent トランスポートエージェントを作成する</span><span class="sxs-lookup"><span data-stu-id="b42dc-103">Create an SmtpReceiveAgent transport agent for Exchange 2013</span></span>

<span data-ttu-id="b42dc-104">Exchange 2013 で使用する、カスタムの SmtpReceiveAgent トランスポートエージェントを作成する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="b42dc-104">Find out how to create a custom SmtpReceiveAgent transport agent to use with Exchange 2013.</span></span>
  
<span data-ttu-id="b42dc-105">**製品:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="b42dc-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="b42dc-106">関連するコードスニペットとサンプルアプリ:</span><span class="sxs-lookup"><span data-stu-id="b42dc-106">Related code snippets and sample apps:</span></span>

- [<span data-ttu-id="b42dc-107">Exchange 2013: 本文変換トランスポートエージェントを構築する</span><span class="sxs-lookup"><span data-stu-id="b42dc-107">Exchange 2013: Build a body conversion transport agent</span></span>](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0)
  
<span data-ttu-id="b42dc-108">[Smtpreceiveagentfactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)および[smtpreceiveagent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)クラスを使用すると、メールボックスサーバー上のクライアントアクセスサーバーまたはトランスポートサービス上のフロントエンドトランスポートサービスの動作を拡張することができます。</span><span class="sxs-lookup"><span data-stu-id="b42dc-108">The [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) and [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) classes enable you to extend the behavior of the Front End Transport service on a Client Access Server or the Transport service on a Mailbox server.</span></span> <span data-ttu-id="b42dc-109">これらのクラスを使用して、組織に到着したメッセージに応答するように設計されたトランスポート エージェントを実装できます。</span><span class="sxs-lookup"><span data-stu-id="b42dc-109">You can use these classes to implement transport agents that are designed to respond to messages as they come into your organization.</span></span> 
  
<span data-ttu-id="b42dc-110">[Smtpreceiveagentfactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)および[smtpreceiveagent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)クラスには、次の表に示すイベントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b42dc-110">The [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) and [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) classes include the events listed in the following table.</span></span> 
  
<span data-ttu-id="b42dc-111">**表1SmtpReceiveAgent クラスのイベント**</span><span class="sxs-lookup"><span data-stu-id="b42dc-111">**Table 1. SmtpReceiveAgent class events**</span></span>

|<span data-ttu-id="b42dc-112">**イベント**</span><span class="sxs-lookup"><span data-stu-id="b42dc-112">**Event**</span></span>|<span data-ttu-id="b42dc-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="b42dc-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b42dc-114">OnAuthCommand</span><span class="sxs-lookup"><span data-stu-id="b42dc-114">OnAuthCommand</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnAuthCommand.aspx) <br/> |<span data-ttu-id="b42dc-115">どの種類の認証方法が使用されたかによって、メッセージ配信の試行を拒否または承認するエージェントなど、SMTP **AUTH** コマンドでのみ得られる情報を必要とするエージェントで使用します。</span><span class="sxs-lookup"><span data-stu-id="b42dc-115">Use when your agent requires information that is provided only in the SMTP **AUTH** command, such as an agent that accepts or rejects attempts to deliver a message based on the type of authentication method used.</span></span>  <br/> |
|[<span data-ttu-id="b42dc-116">OnConnect</span><span class="sxs-lookup"><span data-stu-id="b42dc-116">OnConnect</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnConnect.aspx) <br/> |<span data-ttu-id="b42dc-117">リモート SMTP サーバーのアドレスまたはドメインに基づいてアクションを実行するエージェントなど、フロント エンド トランスポート サービスへの SMTP による接続が開いているときにのみ得られる情報を必要とするエージェントで使用します。</span><span class="sxs-lookup"><span data-stu-id="b42dc-117">Use when your agent requires information that is provided only when a connection is opened via SMTP to the Front End Transport service, such as an agent that performs an action based on the address or domain of the remote SMTP server.</span></span>  <br/> |
|[<span data-ttu-id="b42dc-118">OnDataCommand</span><span class="sxs-lookup"><span data-stu-id="b42dc-118">OnDataCommand</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDataCommand.aspx) <br/> |<span data-ttu-id="b42dc-119">このイベントは、SMTP **DATA** コマンドで得られる情報を必要とするエージェントで使用します。</span><span class="sxs-lookup"><span data-stu-id="b42dc-119">Use this event when your agent requires information that is provided in the SMTP **DATA** command.</span></span>  <br/> |
|[<span data-ttu-id="b42dc-120">OnDisconnect</span><span class="sxs-lookup"><span data-stu-id="b42dc-120">OnDisconnect</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDisconnect.aspx) <br/> |<span data-ttu-id="b42dc-121">時間の計算を実行するために、切断時に得られる現在の時刻と日付などの情報を必要とするエージェントで使用します。</span><span class="sxs-lookup"><span data-stu-id="b42dc-121">Use when your agent requires information that is available at the time of disconnection, such as the current date and time, in order to perform time calculations.</span></span>  <br/> |
|[<span data-ttu-id="b42dc-122">OnEhloCommand</span><span class="sxs-lookup"><span data-stu-id="b42dc-122">OnEhloCommand</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEhloCommand.aspx) <br/> |<span data-ttu-id="b42dc-123">SMTP **EHLO** コマンドで得られる情報を必要とするエージェントで使用します。たとえば、**EHLO** コマンドで得られる ID に基づいて、エージェントによってメッセージを承認または拒否する場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="b42dc-123">Use when your agent requires information that is provided in the SMTP **EHLO** command; for example, if your agent accepts or rejects messages based on the identity provided in the **EHLO** command.</span></span>  <br/> |
|[<span data-ttu-id="b42dc-124">OnEndOfAuthentication</span><span class="sxs-lookup"><span data-stu-id="b42dc-124">OnEndOfAuthentication</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfAuthentication.aspx) <br/> |<span data-ttu-id="b42dc-125">リモート サーバーが認証プロセスを完了したときに得られる情報を必要とするエージェントで使用します。たとえば、リモートの SMTP サーバーやクライアントから得られる認証情報に基づいてメッセージにアクションを実行するエージェントで使用します。</span><span class="sxs-lookup"><span data-stu-id="b42dc-125">Use when your agent requires information that is available after the remote server completes the authentication process; for example, for an agent that performs an action on a message based on the authentication information provided by the remote SMTP server or client.</span></span>  <br/> |
|[<span data-ttu-id="b42dc-126">OnEndOfData</span><span class="sxs-lookup"><span data-stu-id="b42dc-126">OnEndOfData</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) <br/> |<span data-ttu-id="b42dc-p102">メッセージから得られるデータに基づいてアクションを実行する必要のあるエージェントで使用します。このイベントは、フロント エンド トランスポート サービスでは発生しません。このイベントをトランスポート エージェントで使用する必要がある場合は、そのエージェントをメールボックス サーバーにインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b42dc-p102">Use when your agent must perform an action based on data that is available in the message. This event will not fire on the Front End Transport service. If your transport agent has to use this event, you have to install it on a Mailbox server.</span></span>  <br/> |
|[<span data-ttu-id="b42dc-130">OnEndOfHeaders</span><span class="sxs-lookup"><span data-stu-id="b42dc-130">OnEndOfHeaders</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) <br/> |<span data-ttu-id="b42dc-131">送信したメッセージのヘッダーから得られる情報に基づいてアクションを実行する必要のあるエージェントで使用します。</span><span class="sxs-lookup"><span data-stu-id="b42dc-131">Use when your agent must perform an action based on information that is available in the headers of the submitted message.</span></span>  <br/> |
   
## <a name="creating-a-custom-smtpreceiveagent-transport-agent"></a><span data-ttu-id="b42dc-132">カスタム SmtpReceiveAgent トランスポート エージェントの作成</span><span class="sxs-lookup"><span data-stu-id="b42dc-132">Creating a custom SmtpReceiveAgent transport agent</span></span>

<span data-ttu-id="b42dc-133">次に示す手順では、カスタムの SmtpReceiveAgent トランスポート エージェントを作成する方法について説明しています。</span><span class="sxs-lookup"><span data-stu-id="b42dc-133">The following procedure describes how to create a custom SmtpReceiveAgent transport agent.</span></span> 
  
### <a name="to-create-the-transport-agent"></a><span data-ttu-id="b42dc-134">トランスポート エージェントを作成するには</span><span class="sxs-lookup"><span data-stu-id="b42dc-134">To create the transport agent</span></span>

1. <span data-ttu-id="b42dc-135">名前空間に参照を追加します。</span><span class="sxs-lookup"><span data-stu-id="b42dc-135">Add references to the namespaces.</span></span>
    
   ```cs
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Smtp;
      using Microsoft.Exchange.Data.Transport.Email;
      using Microsoft.Exchange.Data.TextConverters;
  
   ```

   <span data-ttu-id="b42dc-136">これらの名前空間は、Exchange 2013 サーバーで見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="b42dc-136">You can find these namespaces on your Exchange 2013 server.</span></span> <span data-ttu-id="b42dc-137">これらの名前空間への参照を追加すると、 [Smtpreceiveagent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)メンバーだけでなく、Exchange 2013 で使用されている他のクラスにもアクセスできるようになります。[本文変換トランスポートエージェント](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0)サンプルを作成します。</span><span class="sxs-lookup"><span data-stu-id="b42dc-137">When you add a reference to these namespaces, you will have access to the [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) members as well as other classes used in the [Exchange 2013: Build a body conversion transport agent](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) sample.</span></span> 
    
2. <span data-ttu-id="b42dc-138">[Smtpreceiveagentfactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)クラスの派生クラスを実装します。</span><span class="sxs-lookup"><span data-stu-id="b42dc-138">Implement the derived class for the [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) class.</span></span> 
    
   ```cs
      public class BodyConversionFactory : SmtpReceiveAgentFactory
      {
          /// <summary>
          /// Create a new BodyConversion
          /// </summary>
          /// <param name="server">Exchange server</param>
          /// <returns>A new BodyConversion</returns>
          public override SmtpReceiveAgent CreateAgent(SmtpServer server)
          {
              return new BodyConversion();
          }
      }
  
   ```

   <span data-ttu-id="b42dc-139">このコードでは、派生クラスのインスタンスを作成し、**CreateAgent** メソッドをオーバーライドして、新しいカスタム エージェントのインスタンスを作成するようにします。</span><span class="sxs-lookup"><span data-stu-id="b42dc-139">This code will instantiate the derived class and override the **CreateAgent** method to create an instance of your new custom agent.</span></span> 
    
3. <span data-ttu-id="b42dc-140">エージェントを定義します。</span><span class="sxs-lookup"><span data-stu-id="b42dc-140">Define your agent.</span></span>
    
   ```cs
     public class BodyConversion : SmtpReceiveAgent
      {
          // Your custom code goes here
          /// <summary>
          /// The constructor registers an end of data event handler.
          /// </summary>
          public BodyConversion()
          {
              Debug.WriteLine("[BodyConversion] Agent constructor");
              this.OnEndOfData += new EndOfDataEventHandler(this.OnEndOfDataHandler);
          }
      }
  
   ```

   <span data-ttu-id="b42dc-141">独自のエージェント クラスを定義すると、カスタムの機能を追加できるようになります。</span><span class="sxs-lookup"><span data-stu-id="b42dc-141">After you define your agent class, you can add your custom functionality.</span></span> <span data-ttu-id="b42dc-142">この例では、 [Onendofdata](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx)イベントがカスタムイベントハンドラーにリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="b42dc-142">In this example, the [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) event is redirected to your custom event handler.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="b42dc-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="b42dc-143">See also</span></span>

- [<span data-ttu-id="b42dc-144">Exchange 2013 におけるトランスポート エージェントの概念</span><span class="sxs-lookup"><span data-stu-id="b42dc-144">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)    
- [<span data-ttu-id="b42dc-145">Exchange 2013 のトランスポート エージェントのリファレンス</span><span class="sxs-lookup"><span data-stu-id="b42dc-145">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)    
- [<span data-ttu-id="b42dc-146">SmtpReceiveAgentFactory</span><span class="sxs-lookup"><span data-stu-id="b42dc-146">SmtpReceiveAgentFactory</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)    
- [<span data-ttu-id="b42dc-147">SmtpReceiveAgent</span><span class="sxs-lookup"><span data-stu-id="b42dc-147">SmtpReceiveAgent</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
    

