## Technical Interview Task (30 minutes)

**Title:***Group Tags by Common Prefix*

### 🧩 **Background:**

When processing documents, you need to group keyword tags. For more effective indexing, we want to group similar tags together.

You need to group document tags that share the same prefix (first few characters).

---

### ✅ **Task**

Implement a method:

```
public List<Set<String>> groupTagsByPrefix(List<String> tags, int prefixLength)
```

Where:

* Tags that share the same first `prefixLength` characters belong to the same group.
* Tags that don’t share their prefix with any others stay in their own group.

#### Example Input:
```
List<String> tags = List.of(
    "account", "accounting", "plan", "planner", "planning", "invest", "investment", "bank", "banking"
);
int prefixLength = 4;
```

#### Expected Output:

```
[
  ["account", "accounting"],
  ["plan", "planner", "planning"],
  ["invest", "investment"],
  ["bank", "banking"]
]
```

---

### 💡 Requirements

* Decompose your code into logical units — avoid one large method.
* Follow clean code practices: good naming, small functions, separation of concerns.
* Write **unit tests using JUnit 5**, covering all possible cases that you can come up with

---

## 📁 Project Skeleton

```
package com.example.taggrouper;

import java.util.*;

public class TagGrouper {

    /**
     * Groups tags by their prefix of given length.
     *
     * @param tags the input list of tags
     * @param prefixLength the length of prefix to group by
     * @return a list of groups (sets), where each group contains tags with the same prefix
     */
    public List<Set<String>> groupTagsByPrefix(List<String> tags, int prefixLength) {
        // TODO: implement the algorithm
        return Collections.emptyList(); // placeholder
    }

    // You can add helper methods here
}

```
---
