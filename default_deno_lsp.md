```toml

[language]]

name = "markdown"
scope = "source.markdown"
roots = []
file-types = [ 'txt' ]


[[language]]

name = "javascript"
shebangs = ["deno"]
roots = ["deno.json", "deno.jsonc"]
file-types = ["js"]
language-servers = ["deno-lsp"]
auto-format = true
indent = { tab-width = 4, unit = "    " }


[[language]]

name = "typescript"
shebangs = ["deno"]
roots = ["deno.json", "deno.jsonc"]
file-types = ["ts"]
language-servers = ["deno-lsp"]
auto-format = true
indent = { tab-width = 4, unit = "    " }

[[language]]

name = "jsx"
shebangs = ["deno"]
roots = ["deno.json", "deno.jsonc"]
file-types = ["jsx"]
language-servers = ["deno-lsp"]
auto-format = true
indent = { tab-width = 4, unit = "    " }


[[language]]

name = "tsx"
shebangs = ["deno"]
roots = ["deno.json", "deno.jsonc"]
file-types = ["tsx"]
language-servers = ["deno-lsp"]
auto-format = true
indent = { tab-width = 4, unit = "    " }


[language-server.deno-lsp]
command = "deno"
args = ["lsp"]
environment = { NO_COLOR = "1" }

[language-server.deno-lsp.config.deno]
enable = true
# Uncomment to enable completion of unstable features of Deno
# unstable = true
# Uncomment to cache dependencies on save
# cacheOnSave = true
# Enable completion of importing from registries
# Enable completion of function calls
suggest = { completeFunctionCalls = false, imports = { hosts = { "https://deno.land" = true } } }
# suggest = { imports = { hosts = { "https://deno.land" = true, "https://crux.land" = true, "https://x.nest.land" = true } } }
# Uncomment to enable inlay hints
inlayHints.parameterNames.enabled = "all"
inlayHints.parameterTypes.enabled = true
inlayHints.variableTypes.enabled = true
# inlayHints.propertyDeclarationTypes.enabled  = true
# inlayHints.functionLikeReturnTypes.enabled = true
# inlayHints.enumMemberValues.enabled = true

```