## brat-doc

*Work in Progress*

Scans special comments in Brat and Lua code to generate some documentation.

Doesn't do anything fancy.

## Format

### Lua

    -- Object: <object> [instance]
    -- Call: <object>.<method> [<args>]
    -- Returns: <object>
    --
    -- <description>
    --
    -- Example:
    --
    -- <example>


Only the `Object:` line is required.

Example:

    -- Object: string instance
    -- Call: string.reverse!
    -- Returns: string
    --
    -- Reverses a string.
    --
    -- Example:
    --
    -- "parts".reverse!


### Brat

    # Object: <object> [instance]
    # Call: <object>.<method> [<args>]
    # Returns: <object>
    #
    # <description>
    #
    # Example:
    #
    # <example>

Example:

    # Object: file
    # Call: file.read file_name
    # Returns: string
    #
    # Reads in contents of file into a string.
