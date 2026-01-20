# YAML syntax for Github Actions

## Variation 1 --> inline list ✅

```yaml
on: [push, pull_request, 'workflow_dispatch']
branches: [main, develop, 'feature/**', '!test/**']
types: [opened, labeled]
```

## Variation 2  --> block list ✅ and 💯

```yaml
branches:
      - main
      - develop
      - 'feature/**'
```

## Variation 3 -- nested list ❌ ( YAML ✅ )

```yaml
branches:
  - main
  - [develop, release]
```

## Variation 4 -- inline list with quotes ✅

```yaml

branches: ["main", "develop", "release/**"]
```

