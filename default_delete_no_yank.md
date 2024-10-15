```toml

[keys.normal]
d = ["delete_selection_noyank"]
A-d = ["delete_selection"]
S-A-up = ["extend_to_line_bounds", "yank", "open_below", "normal_mode", "replace_with_yanked", "collapse_selection"]
S-A-down = ["extend_to_line_bounds", "yank", "open_above", "normal_mode", "replace_with_yanked", "collapse_selection"]
A-down = ["extend_to_line_bounds", "delete_selection", "paste_after"]
A-up = ["extend_to_line_bounds", "delete_selection", "move_line_up", "paste_before"]

[keys.select]
d = ["delete_selection_noyank"]
A-d = ["delete_selection"]

[keys.insert]
S-A-up = ["extend_to_line_bounds", "yank", "open_below", "normal_mode", "replace_with_yanked", "collapse_selection"]
S-A-down = ["extend_to_line_bounds", "yank", "open_above", "normal_mode", "replace_with_yanked", "collapse_selection"]
A-down = ["extend_to_line_bounds", "delete_selection", "paste_after"]
A-up = ["extend_to_line_bounds", "delete_selection", "move_line_up", "paste_before"]

```
