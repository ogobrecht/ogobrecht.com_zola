+++
title = "Console"
description = "Lightweight PL/SQL logging tool inspired by the JavaScript Console"
weight = 2
template = "page.html"

[taxonomies]
tags = ["Oracle", "PL/SQL", "Instrumentation", "Logger"]

[extra]
local_image = "/img/pete-nuij-m-AqW5QCxNQ-unsplash-square.jpeg"
+++

An instrumentation tool for Oracle developers focused on easy installation
and usage combined with nice features.

![Flying owl, symbol for a keen eye on the code](/img/pete-nuij-m-AqW5QCxNQ-unsplash.jpg)

#### [View Source](https://github.com/ogobrecht/console){.centered-text}

## Features

- Easy to Install
  - Works without a context
  - Has a single installation script (can be installed in APEX via "SQL
  Workshop > SQL Scripts")
- Easy to Use
  - Save to run in production without further configuration
  - Errors are always logged
  - You can change the default log level for all or specfic sessions from
    `error` to `warning`, `info`, `debug` and `trace`. As a best practice the
    last two should not be set for all sessions on production systems.
  - Specific sessions are identified by the client identifier. If a session
    has no client identifier, console is setting one for you.
  - Method names are inspired by the JavaScript Console
- Can help you to avoid cluttered error logs by only logging errors in your
  outermost package methods without loosing context details with the help of
  `console.error_save_stack` in the nested methods. This might be the most
  powerful feature for some people...
- No need to provide manually a scope for your log entries - console does
  this automatically for you. If needed, you can overwrite the default scope.
- Has an optional APEX error handling function to log also internal errors of
  the APEX engine
- Has an optional APEX plug-in to log JavaScript errors in your client
  frontends
- Is extensible. Log methods `error`, `warn`, `info`, `debug` and `trace` are
  all implemented as a procedure and a function returning the log ID. So you
  can easily implement additional functionality which references the log
  entries like an approval for certain errors or save additional information
  in a specific table.
- Can easily log method parameters with the help of `console.add_param` (chainable)
- Brings some useful helper functions with it
