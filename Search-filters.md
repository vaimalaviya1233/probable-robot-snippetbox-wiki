## Search filters

### Simple search
- Query: `component`
- Result: All snippets with word "component" in either title or description

---

### Search with language filter (`lang:`)
- Single language
  - Query: `function lang:typescript`
  - Result: All snippets with word "function" in either title or description and "typescript" as a language

- Multiple languages
  - Query: `function lang:typescript,python`
  - Result: All snippets with word "function" in either title or description and "typescript" or "python" as a language

- Only languages
  - Query: `lang:php,go`
  - Result: All snippets with "php" or "go" as a language

---

### Search with tags filter (`tags:`)
- Single tag
  - Query: `component tags:card`
  - Result: All snippets with word "component" in either title or description and "card" tag

- Multiple tags
  - Query: `component tags:card,react`
  - Result: All snippets with word "component" in either title or description and "card" or "react" tag

- Only tags
  - Query: `tags:react,vue,angular`
  - Result: All snippets with "react", "vue" or "angular" tag

---

Multiple filters can be used at once: `card lang:typescript tags:react,vue` is a valid query