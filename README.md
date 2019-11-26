# ngx-profiler-module
An module that helps us tracking CPU, memory in nginx

# How it works

Format: csv.
Columns:
- process_id: process id
- process_name: process name
- time per 10 minutes: CPU percentage
Data will be save Daily.

# Config:
Directive:
### system_profiler
Syntax: `system_profiler on|off`
Context: http,server,location

Toggles system profiler feature.

### system_profiler_freq
Syntax: `system_profiler_freq time`
Context: http,server,location

How ofent system profiler collects data.
Default: 10m.

### system_profiler_path
Syntax: `system_profiler_path path`
Context: http, server, location

Set path to save data