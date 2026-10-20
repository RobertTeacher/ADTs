# Cambridge 9618 — Unit 19 Visualizer

A GitHub Pages-ready visual revision site for Cambridge International A Level Computer Science 9618 Unit 19.

## Included

- Searching & Sorting
  - Linear search
  - Binary search
  - Bubble sort
  - Insertion sort
  - Recursive binary search
  - Recursive insertion sort
- Stack
  - Push / Pop
  - explicit TopPointer convention
- Circular Queue
  - Enqueue / Dequeue
  - HeadPointer / TailPointer / NumberItems
  - wrap-around
- Linked List
  - pointer traversal pattern
  - insert at front
  - remove by value
  - free-list management
- Binary Search Tree
  - AddNode
  - recursive SearchValue
  - Pre-order traversal
  - In-order traversal
  - Post-order traversal
  - call stack / unwinding
- Recursion Lab
  - base case
  - general case
  - call stack
  - unwinding
  - recursive linear search
- Dictionary and Graph concepts
  - dictionary key-value operations
  - graph features
  - BFS/DFS animation is clearly labelled enrichment
- Big O reference table
- Examiner-informed Paper 4 tips

## GitHub Pages

Upload all HTML files in this folder to the same repository directory and enable GitHub Pages.

The entry point is:

`index.html`

Example URL:

`https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/`

## Canvas LMS

After GitHub Pages is live, paste the following into the Canvas HTML editor:

```html
<div style="width:100%;border:1px solid #d8d8d8;box-sizing:border-box;overflow:hidden;">
  <iframe
    src="https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/"
    title="Cambridge 9618 Unit 19 Visualizer"
    style="display:block;width:100%;height:1450px;border:none;"
    width="100%"
    height="1450"
    loading="lazy"
    frameborder="0">
  </iframe>
</div>
```

Increase the iframe height if required by your Canvas theme.

## Important conventions

These are explicit conventions for this visualizer:

- Stack: `TopPointer` points to the next free position.
- Circular queue: `HeadPointer` points to the next item to remove; `TailPointer` points to the next free position; `NumberItems` distinguishes full from empty.
- Linked list: `[Data, NextPointer]`, `FirstNode`, `FirstEmpty`.
- Binary tree: `[LeftPointer, Data, RightPointer]`, `RootPointer`, `FreeNode`.

In an examination, the convention stated in the question always takes priority.

## Big O cautions

- Optimised bubble sort has best-case O(n) only if early termination is actually implemented.
- Binary-search-tree search/insert is average O(log n) but worst O(n) when the tree becomes highly unbalanced.
- Recursive algorithms may have the same time complexity as iterative versions but use additional call-stack memory.
- Dictionary complexity depends on its concrete implementation.

## Examiner-report basis

The exam-tip page paraphrases recurring issues reported in Cambridge Principal Examiner Reports, especially:

- June 2025 Paper 4: queue full/empty checks, Head/Tail misuse, missing circular wrap-around, stack pointer conventions, inappropriate use of append, binary-search boundary updates, return-value handling, exact data types, recursive/tree pointer handling, and evidence-document presentation.
- June 2023 Paper 4: preserve the structure/functionality of a supplied sorting algorithm and copy required source data accurately.

The site paraphrases these findings rather than reproducing report text.
