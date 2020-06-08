+++
title = "SET"
description = "set a value to a key"

[extra]
type = "keys"
+++

# **SET key value [EX seconds]**

Set a value to key. if key already holds a value its overwritten.

#### Options

- **EX** seconds -- Set the specified expire time, in seconds.

#### Return Value
Returns **OK** if set was successful.

#### Examples
``` repl
> SET name kofi
"Ok"
> GET name
"kofi"
> SET verfication.code "330732" EX 60
"Ok"
```