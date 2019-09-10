### cactus
---
https://github.com/eudicots/Cactus

```py
// Cactus/skeleton/plugins
// blog.disabled.py
// coffeescrit.disabled.py
// gitcommitid.disabled.py
// haml.disabled.py
// page_context.py
// sass.disabled.py
// scss.disabled.py
// sprites.disabled.py

// static_optimizers.py
from cactus.contrib.external.closure import ClosureJSOptimizer
from cactus.contrib.external.yui import YUICSSOptimizer

def preBuild(site):
  """
  """
  optimize = site.config.get("optimize", [])
  
  if "js" in optimize:
    site.external_manager.register_optimizer(ClosureJSOptimizer)
    
  if "css" in optimize:
    site.external_manager.register_optimizer(YUICSSOptimizer)

```

```
```

```
```

