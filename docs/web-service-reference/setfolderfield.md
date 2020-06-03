---
title: SetFolderField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetFolderField
api_type:
- schema
ms.assetid: 8c69db7b-54b5-4ae2-abca-4d6e0937a790
description: SetFolderField 要素は、UpdateFolder 操作のフォルダーの1つのプロパティの値を設定する更新を表します。
ms.openlocfilehash: ab75a3862801b9a7b3369d9a4116c653b461781c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530318"
---
# <a name="setfolderfield"></a><span data-ttu-id="a766a-103">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="a766a-103">SetFolderField</span></span>

<span data-ttu-id="a766a-104">**Setfolderfield**要素は、updatefolder 操作のフォルダーの1つのプロパティの値を設定する更新を表します。</span><span class="sxs-lookup"><span data-stu-id="a766a-104">The **SetFolderField** element represents an update that sets the value for a single property on a folder in an UpdateFolder operation.</span></span> 

```xml
<SetFolderField>
   <FieldURI/>
   <Folder/>
</SetFolderField>
```
  
```xml
<SetFolderField>
   <IndexedFieldURI/> 
   <SearchFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <FieldURI/> 
   <TasksFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <CalendarFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <SearchFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <Folder/> 
</SetFolderField>
```

```xml
<SetFolderField>
    <IndexedFieldURI/> 
    <TasksFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <FieldURI/> 
   <SearchFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <FieldURI/> 
   <CalendarFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <TasksFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <IndexedFieldURI/> 
   <CalendarFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <IndexedFieldURI/> 
   <Folder/>
</SetFolderField>
```

```xml
<SetFolderField>
    <FieldURI/> 
    <ContactsFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <ContactsFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <IndexedFieldURI/> 
   <ContactsFolder/> 
</SetFolderField>
```


<span data-ttu-id="a766a-105">**SetFolderFieldType**</span><span class="sxs-lookup"><span data-stu-id="a766a-105">**SetFolderFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a766a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a766a-106">Attributes and elements</span></span>

<span data-ttu-id="a766a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a766a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a766a-108">属性</span><span class="sxs-lookup"><span data-stu-id="a766a-108">Attributes</span></span>

<span data-ttu-id="a766a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a766a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a766a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a766a-110">Child elements</span></span>

|<span data-ttu-id="a766a-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="a766a-111">**Element**</span></span>|<span data-ttu-id="a766a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a766a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a766a-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="a766a-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="a766a-114">URI で頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="a766a-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="a766a-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="a766a-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="a766a-116">辞書の個々のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="a766a-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="a766a-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="a766a-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="a766a-118">拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="a766a-118">Identifies extended MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="a766a-119">Folder</span><span class="sxs-lookup"><span data-stu-id="a766a-119">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="a766a-120">更新するフォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="a766a-120">Identifies a folder to update.</span></span>  <br/> |
|[<span data-ttu-id="a766a-121">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="a766a-121">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="a766a-122">主に予定表アイテムを含むフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="a766a-122">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="a766a-123">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="a766a-123">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="a766a-124">メールボックス内の連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="a766a-124">Represents a Contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="a766a-125">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="a766a-125">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="a766a-126">メールボックスに含まれている検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="a766a-126">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="a766a-127">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="a766a-127">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="a766a-128">メールボックスに含まれる Tasks フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="a766a-128">Represents a Tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a766a-129">親要素</span><span class="sxs-lookup"><span data-stu-id="a766a-129">Parent elements</span></span>

|<span data-ttu-id="a766a-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="a766a-130">**Element**</span></span>|<span data-ttu-id="a766a-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="a766a-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a766a-132">Updates (フォルダー)</span><span class="sxs-lookup"><span data-stu-id="a766a-132">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="a766a-133">フォルダーのプロパティに対する追加、設定、および削除の変更を定義する一連の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a766a-133">Contains a set of elements that defines append, set, and delete changes to folder properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a766a-134">注釈</span><span class="sxs-lookup"><span data-stu-id="a766a-134">Remarks</span></span>

<span data-ttu-id="a766a-135">プロパティが存在する場合、プロパティ値は指定された値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="a766a-135">If the property exists, the property value is set to the specified value.</span></span> <span data-ttu-id="a766a-136">プロパティが存在しない場合は、指定された値を持つプロパティが作成されます。</span><span class="sxs-lookup"><span data-stu-id="a766a-136">If the property does not exist, the property is created with the specified value.</span></span>
  
<span data-ttu-id="a766a-137">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="a766a-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a766a-138">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a766a-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a766a-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="a766a-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a766a-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a766a-140">Schema Name</span></span>  <br/> |<span data-ttu-id="a766a-141">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a766a-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="a766a-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a766a-142">Validation File</span></span>  <br/> |<span data-ttu-id="a766a-143">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a766a-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a766a-144">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a766a-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="a766a-145">正しくない</span><span class="sxs-lookup"><span data-stu-id="a766a-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a766a-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="a766a-146">See also</span></span>

- [<span data-ttu-id="a766a-147">UpdateFolder 操作</span><span class="sxs-lookup"><span data-stu-id="a766a-147">UpdateFolder operation</span></span>](updatefolder-operation.md)
- [<span data-ttu-id="a766a-148">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a766a-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

