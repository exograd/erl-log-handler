# Project
This repository contains a minimalist log handler for the
[logger](https://erlang.org/doc/man/logger.html) OTP application.

# Usage
Make sure to add the application as dependency in the Rebar3 configuration
file. After that, the formatter is configured as any other logger handler,
in the system configuration file.

Example:
```erlang
[{kernel,
  [{logger,
    [{handler, default, log_handler,
      #{level => debug,
        filter_default => log}}]},
   {logger_level, debug}]}].
```

See the [logger
documentation](https://erlang.org/doc/apps/kernel/logger_chapter.html) for
more information.

# Contact
If you find a bug or have any question, feel free to open a GitHub issue or to
contact me [by email](mailto:khaelin@gmail.com).

Please note that I do not currently review or accept any contribution.
