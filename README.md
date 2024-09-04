
```zig
const std = @import("std");

const User = struct {
    code: []const []const u8,
    os: []const u8,
    editor: []const u8,
    playlist: []const u8,
};

pub fn main() !void {
    const franklin = User{
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
        .playlist = "https://open.spotify.com/playlist/5qS4k4o1Nv63BXYw6BC29w?si=8b0df14856ff4891",
    };
    std.debug.print("Franklin's details:\n", .{});
    std.debug.print("  Code: ", .{});
    for (franklin.code) |lang| {
        std.debug.print("{s}, ", .{lang});
    }
    std.debug.print("\n  OS: {s}\n", .{franklin.os});
    std.debug.print("  Editor: {s}\n", .{franklin.editor});
    std.debug.print("  Playlist: {s}\n", .{franklin.playlist});
}
```

![glory](https://github.com/user-attachments/assets/c96412d9-c28c-4bd5-bcdb-fdbe2ec299e1)
