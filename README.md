## Technical Interview Task (45 minutes)

**Title:***Smart Text Grouping for Automated Document Tagging*

### 🧩 **Background:**

When processing documents, you need to extract keyword tags. These tags can be long, partially overlapping, or nested as substrings of one another. For more effective indexing, we want to group similar tags together.

Your task is to **group tags** where each group contains tags that are **substrings of one another**.

---

### ✅ **Task**

Implement a method:

<code class="whitespace-pre! language-java"><span><span>public</span><span> List<Set<String>> </span><span>groupTags</span><span>(List<String> tags)</span><span>
</span></span></code></div></div></pre>

Where:

* A group includes tags that are substrings of at least one other tag in the same group.
* Tags that don’t match any others can stay in their own group.

#### Example Input:

<pre class="overflow-visible!" data-start="916" data-end="1064"><div class="contain-inline-size rounded-2xl relative bg-token-sidebar-surface-primary"><div class="overflow-y-auto p-4" dir="ltr"><code class="whitespace-pre! language-java"><span><span>List<String> tags = List.of(
  </span><span>"account"</span><span>, </span><span>"accounting"</span><span>, </span><span>"finance"</span><span>, </span><span>"financial"</span><span>, </span><span>"investment"</span><span>, </span><span>"invest"</span><span>, </span><span>"invested"</span><span>, </span><span>"bank"</span><span>, </span><span>"banking"</span><span>
);
</span></span></code></div></div></pre>

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

<pre class="overflow-visible!" data-start="1655" data-end="2222"><div class="contain-inline-size rounded-2xl relative bg-token-sidebar-surface-primary"><div class="overflow-y-auto p-4" dir="ltr"><code class="whitespace-pre! language-java"><span><span>// File: src/main/java/com/example/taggrouper/TagGrouper.java</span><span>
</span><span>package</span><span> com.example.taggrouper;

</span><span>import</span><span> java.util.*;

</span><span>public</span><span> </span><span>class</span><span> </span><span>TagGrouper</span><span> {

    /**
     * Groups tags that are substrings of each other.
     *
     * </span><span>@param</span><span> tags the input list of tags
     * </span><span>@return</span><span> a list of groups (sets), where each group contains related tags
     */
    </span><span>public</span><span> List<Set<String>> </span><span>groupTags</span><span>(List<String> tags)</span><span> {
        </span><span>// TODO:</span><span> implement the algorithm
    }

    </span><span>// You may add helper methods or classes here</span><span>
}
</span></span></code></div></div></pre>

---
