## Technical Interview Task (45 minutes)

**Title:***Smart Text Grouping for Automated Document Tagging*

### 🧩 **Background:**

When processing documents, you need to extract keyword tags. These tags can be long, partially overlapping, or nested as substrings of one another. For more effective indexing, we want to group similar tags together.

Your task is to **group tags** where each group contains tags that are **substrings of one another**.

---

### ✅ **Task**

Implement a method:

```
public List<Set<String>> groupTags(List<String> tags)
```

Where:

* A group includes tags that are substrings of at least one other tag in the same group.
* Tags that don’t match any others can stay in their own group.

#### Example Input:
```
List<String> tags = List.of(
  "account", "accounting", "finance", "financial", "investment", "invest", "invested", "bank", "banking"
);
```

#### Expected Output:

<pre class="overflow-visible!" data-start="1088" data-end="1222"><div class="overflow-y-auto p-4" dir="ltr"><code class="whitespace-pre! language-java"><span><span>[
  [</span><span>"account"</span><span>, </span><span>"accounting"</span><span>],
  [</span><span>"finance"</span><span>, </span><span>"financial"</span><span>],
  [</span><span>"invest"</span><span>, </span><span>"investment"</span><span>, </span><span>"invested"</span><span>],
  [</span><span>"bank"</span><span>, </span><span>"banking"</span><span>]
]
</span></span></code></div></div></pre>

> *Note: You don’t need to sort tags or groups. Output order doesn’t matter.*

---

### 💡 Requirements

* Decompose your code into logical units — avoid one large method.
* Follow clean code practices: good naming, small functions, separation of concerns.
* Write **unit tests using JUnit 5**, covering all possible cases that you can come up with

---

## 📁 Project Skeleton

```
// File: src/main/java/com/example/taggrouper/TagGrouper.java
package com.example.taggrouper;

import java.util.*;

public class TagGrouper {

    /**
     * Groups tags that are substrings of each other.
     *
     * @param tags the input list of tags
     * @return a list of groups (sets), where each group contains related tags
     */
    public List<Set<String>> groupTags(List<String> tags) {
        // TODO: implement the algorithm
        return Collections.emptyList(); // placeholder
    }

    // You may add helper methods or classes here
}
```
---
