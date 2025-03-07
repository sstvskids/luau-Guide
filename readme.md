> [!IMPORTANT]
> This guide may not have every function, take caution

# luaU for idiots/skids
Explains luaU for exploits in a user-friendly way!

## Printing/Comments
There are 3 types of print. (error, warn and print)
```lua
print('test')
warn('yo')
error('real') -- Error has a second argument called level, however it's not necessary! This is a comment also.
--[[ this also works ]]
```

## Functions
Functions help in situations (e.g api) and clean code!
```lua
local function an4rch()
    print('an4rchist for life!!')
end
an4rch()
```

## Variables, Booleans, Services
Booleans are (true or false). Variables require two arguments. (name, (string, function or service or boolean))
```lua
local Skibidi = 'string' -- This is a string ''.
local Hawk = an4rch() -- A function
local skibid = false -- Returns false
local Players: Players = game:GetService('Players') -- gets the players service
```

# Operators
- `+` Addition (adds two values together)

  ```lua
  local sum = 5 + 3 -- Returns 8
  ```
- `-` Subtraction (subtracts second value from first)

  ```lua
  local difference = 10 - 4 -- Returns 6
  ```
- `*` Multiplication (multiplies two values)

  ```lua
  local product = 6 * 2 -- Returns 12
  ```
- `/` Division (divides first value by second)

  ```lua
  local quotient = 15 / 3 -- Returns 5
  ```
- `^` Exponentiation (raises first value to power of second)

  ```lua
  local power = 2 ^ 3 -- Returns 8
  ```
- `%` Modulus (returns remainder after division)

  ```lua
  local remainder = 10 % 3 -- Returns 1
  ```