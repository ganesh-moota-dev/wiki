# Adding Comments

Comments in Bash scripting are used to provide explanations or annotations for the code, making it easier to understand and maintain. Here’s how you can use comments in Bash:

* **Single-line comments**: Begin with a `#` symbol. Everything following the `#` on that line is treated as a comment and ignored during execution.

```bash
# This is a single-line comment
echo "Hello, World!" # This is also a comment
```

* **Multi-line comments**: Bash doesn’t have a direct way to create multi-line comments like some other programming languages. However, you can use a `:` (colon) with a redirection operator `<<` and a delimiter to create a block of text that won’t be executed.

```bash
: <<'END_COMMENT'
This is a multi-line comment.
It can span multiple lines.
END_COMMENT
```

Remember, comments are essential for documenting the purpose and logic of your code, especially when working on complex scripts or collaborating with others. They can also be used to temporarily disable code during debugging.
