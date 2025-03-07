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
local Hawk = an4rch() -- Function inside a variable
local skibid = false -- Returns false
local Players: Players = game:GetService('Players') -- gets the players service
```

## Tables
Tables in Lua are powerful data structures that can be used as arrays, dictionaries, objects, functions and more.
```lua
-- Creating a basic table
local table = {
    tee = 'test',        -- Key-value pair (dictionary style)
    funcs = {            -- Nested table
        an4rch = an4rch()
    },
    "first",             -- Array-style element (index 1)
    "second",            -- Array-style element (index 2)
    123                  -- Array-style element (index 3)
}
-- Accessing table elements
print(table.tee)         -- Outputs: test
print(table["tee"])      -- Alternative way to access, outputs: test
print(table[1])          -- Outputs: first (array-style access)
-- Iterates through a table with pairs() (for dictionaries)
for i,v in pairs(table) do
    print(i,v)
end
-- Iterates through array portion with ipairs() (for arrays)
for i,v in ipairs(table) do
    print(i,v)
end
-- Table manipulation
table.newKey = "new value"   -- Add new key-value pair
table[4] = "fourth"          -- Add to array portion
table.tee = nil              -- Removes a key
-- Table functions
print(#table)                -- Length of array portion
table.insert(table, "fifth") -- Add to end of array portion
table.remove(table, 1)       -- Remove first array element
table.concat({"a", "b", "c"}, "-") -- Join array elements (outputs: a-b-c)
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

## Operator Comparison
- `==` Equal to

  ```lua
  print(5 == 5) -- Returns true
  print(5 == 6) -- Returns false
  ```
- `<` Less than

  ```lua
  print(3 < 5) -- Returns true
  print(5 < 3) -- Returns false
  ```
- `>` Greater than

  ```lua
  print(5 > 3) -- Returns true
  print(3 > 5) -- Returns false
  ```
- `<=` Less than or equal to

  ```lua
  print(3 <= 3) -- Returns true
  print(4 <= 3) -- Returns false
  ```
- `>=` Greater than or equal to

  ```lua
  print(3 >= 3) -- Returns true
  print(2 >= 3) -- Returns false
  ```
- `~=` Not equal to

  ```lua
  print(5 ~= 6) -- Returns true
  print(5 ~= 5) -- Returns false
  ```
## String Functions
```lua
-- string.split() divides a string by separator
local text = "apple,banana,orange"
local fruits = string.split(text, ",")  -- Returns {"apple", "banana", "orange"}

-- string.pack() and string.unpack() for binary data
local packed = string.pack("ii", 123, 456)    -- Packs numbers into binary
local num1, num2 = string.unpack("ii", packed) -- Unpacks back to numbers

-- tostring() turns the result into a string
local math = math.random(1,999)
print(tostring(math))
```