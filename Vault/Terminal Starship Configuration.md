```
add_newline = false
format = """$hostname$directory $username $git_branch$git_status$character"""

[username]
style_user = "bold fg:135"
style_root = "bold red"
format = "[$user]($style)"
show_always = true

[hostname]
trim_at = ""
style = "fg:28"
format = "[$hostname]($style)/"

[directory]
truncate_to_repo = true
truncation_length = 2
truncation_symbol = ".../"
style = "fg:77"
format = "[$path]($style)[$read_only]($read_only_style)"

[character]
success_symbol = "[:](bold green)"
error_symbol = "[:](bold red)"

[git_commit]
only_detached = false

[git_branch]
symbol = ""
style = "fg:36"

[git_status]
style = "fg:36"

```
