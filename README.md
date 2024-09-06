
```zig
const std = @import("std");

const User = struct {
    code: []const []const u8,
    os: []const u8,
    editor: []const u8,
};

pub fn main() !void {
    const maky = User{
        .code = &[_][]const u8{
            "Zig",
            "Go",
            "TypeScript",
            "JavaScript",
            "GraphQL",
            "Python",
            "Go",
            "Lua",
        },
        .os = "Mac OS",
        .editor = "NeoVim",
    };
    std.debug.print("Maky's details:\n", .{});
    std.debug.print("  Code: ", .{});
    for (franklin.code) |lang| {
        std.debug.print("{s}, ", .{lang});
    }
    std.debug.print("\n  OS: {s}\n", .{maky.os});
    std.debug.print("  Editor: {s}\n", .{maky.editor});
    std.debug.print("  Playlist: {s}\n", .{maky.playlist});
}
```

![glory](https://github.com/user-attachments/assets/c96412d9-c28c-4bd5-bcdb-fdbe2ec299e1)
