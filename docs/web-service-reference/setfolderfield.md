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
description: SetFolderField 要素は、UpdateFolder 操作でフォルダーの 1 つのプロパティの値を設定する更新プログラムを表します。
ms.openlocfilehash: ed5c055c697865d5eb728d269c6f4c7ce60f4b5c
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353288"
---
# <a name="setfolderfield"></a><span data-ttu-id="1c80c-103">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="1c80c-103">SetFolderField</span></span>

<span data-ttu-id="1c80c-104">**SetFolderField**要素は、UpdateFolder 操作でフォルダーの 1 つのプロパティの値を設定する更新プログラムを表します。</span><span class="sxs-lookup"><span data-stu-id="1c80c-104">The **SetFolderField** element represents an update that sets the value for a single property on a folder in an UpdateFolder operation.</span></span> 

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


<span data-ttu-id="1c80c-105">**SetFolderFieldType**</span><span class="sxs-lookup"><span data-stu-id="1c80c-105">**SetFolderFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1c80c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1c80c-106">Attributes and elements</span></span>

<span data-ttu-id="1c80c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1c80c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1c80c-108">属性</span><span class="sxs-lookup"><span data-stu-id="1c80c-108">Attributes</span></span>

<span data-ttu-id="1c80c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1c80c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1c80c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1c80c-110">Child elements</span></span>

|<span data-ttu-id="1c80c-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="1c80c-111">**Element**</span></span>|<span data-ttu-id="1c80c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1c80c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c80c-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="1c80c-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="1c80c-114">URI によって頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="1c80c-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="1c80c-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="1c80c-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="1c80c-116">辞書の個々 のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="1c80c-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="1c80c-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="1c80c-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="1c80c-118">拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="1c80c-118">Identifies extended MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="1c80c-119">Folder</span><span class="sxs-lookup"><span data-stu-id="1c80c-119">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="1c80c-120">更新するフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="1c80c-120">Identifies a folder to update.</span></span>  <br/> |
|[<span data-ttu-id="1c80c-121">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="1c80c-121">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="1c80c-122">主に予定表のアイテムを含むフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="1c80c-122">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="1c80c-123">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="1c80c-123">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="1c80c-124">メールボックスの連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="1c80c-124">Represents a Contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="1c80c-125">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="1c80c-125">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="1c80c-126">メールボックスに格納されている検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="1c80c-126">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="1c80c-127">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="1c80c-127">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="1c80c-128">メールボックスに含まれるタスク フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="1c80c-128">Represents a Tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1c80c-129">親要素</span><span class="sxs-lookup"><span data-stu-id="1c80c-129">Parent elements</span></span>

|<span data-ttu-id="1c80c-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="1c80c-130">**Element**</span></span>|<span data-ttu-id="1c80c-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="1c80c-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c80c-132">Updates (Folder)</span><span class="sxs-lookup"><span data-stu-id="1c80c-132">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="1c80c-133">定義する一連要素にはが含まれていて、このオプションを設定すると、フォルダーのプロパティへの変更を削除します。</span><span class="sxs-lookup"><span data-stu-id="1c80c-133">Contains a set of elements that defines append, set, and delete changes to folder properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1c80c-134">注釈</span><span class="sxs-lookup"><span data-stu-id="1c80c-134">Remarks</span></span>

<span data-ttu-id="1c80c-135">プロパティが存在する場合、プロパティの値が指定した値に設定します。</span><span class="sxs-lookup"><span data-stu-id="1c80c-135">If the property exists, the property value is set to the specified value.</span></span> <span data-ttu-id="1c80c-136">プロパティが存在しない場合は、指定の値を持つプロパティが作成されます。</span><span class="sxs-lookup"><span data-stu-id="1c80c-136">If the property does not exist, the property is created with the specified value.</span></span>
  
<span data-ttu-id="1c80c-137">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1c80c-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1c80c-138">要素情報</span><span class="sxs-lookup"><span data-stu-id="1c80c-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1c80c-139">名前空間</span><span class="sxs-lookup"><span data-stu-id="1c80c-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1c80c-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1c80c-140">Schema Name</span></span>  <br/> |<span data-ttu-id="1c80c-141">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="1c80c-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="1c80c-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1c80c-142">Validation File</span></span>  <br/> |<span data-ttu-id="1c80c-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1c80c-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1c80c-144">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1c80c-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="1c80c-145">False</span><span class="sxs-lookup"><span data-stu-id="1c80c-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1c80c-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="1c80c-146">See also</span></span>

- <span data-ttu-id="1c80c-147">
  [UpdateFolder 操作](updatefolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="1c80c-147">[UpdateFolder operation](updatefolder-operation.md)</span></span>
- [<span data-ttu-id="1c80c-148">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1c80c-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

