# ISO 639 Standard
"Code for individual languages and language groups."

## Usage
Example:
```Zig
const std = @import("std");
const Iso639 = @import("iso639");

pub fn main() void {
    const language_name = "Polish";
    const language = Iso639.Language.initNameUtf8(language_name);
    std.log.info("Language code '{s}' is associated with the language '{s}'.", .{
        @tagName(language.?),
        language_name,
    });
}
```
