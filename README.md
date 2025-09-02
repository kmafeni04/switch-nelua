# switch-nelua

Macro function to allow switching on not only numbers

## Requirements
- [nelua](https://nelua.io/)

## How to install
Copy `switch.nelua` into your project and require normally or add to your [nlpm](https://github.com/kmafeni04/nlpm) package dependencies
```lua
{
  name = "switch-nelua",
  repo = "https://github.com/kmafeni04/switch-nelua",
  version = "COMMIT-HASH-OR-TAG",
},
```

## Quick start

```lua
local y = 1
local res = _switch!(y, {
  [1] = "hello",
  _default = (do
    in "_default"
  end)
})
-- when y == 1
print(res) --> hello
-- when y == anything else
print(res) --> _default
```

## Reference

### _switch macro

```lua
## function _switch(expr, cases)
```

