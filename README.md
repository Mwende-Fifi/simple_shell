# Simple Shell Program

This is a simple shell program that allows users to execute commands with or without arguments. It displays a prompt, waits for user input, executes the command, and then displays the prompt again for the next command.

## Features

- Displays a user-friendly prompt to input commands.
- Executes commands, both with and without arguments.
- Handles errors and notifies the user in case of an invalid command or executable not found.
- Gracefully handles the "end of file" condition (Ctrl+D).

## Getting Started

To run this shell program, follow these steps:

1. Clone this repository to your local machine.

```bash
git clone https://github.com/Mwende-Fifi/simple_shell
cd simple_shell
```

2. Compile the shell program.

```bash
gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh
```

3. Run the shell.

```bash
./hsh
```

## Usage

Once you have launched the shell, you can start typing commands. The shell supports simple commands, which are single words without any semicolons, pipes, redirections, or advanced features.

### Example Commands:

1. **Executing a Command:**

   ```
   > ls
   ```

   This will execute the `ls` command and display the directory contents.

2. **Command with Arguments:**

   ```
   > echo Hello, world!
   ```

   This will execute the `echo` command with the argument "Hello, world!" and display the output.

3. **Handling Errors:**

   If you enter an invalid command or the executable is not found:

   ```
   > foobar
   Command not found: foobar
   ```

   The shell will print an error message and display the prompt again for the next command.

4. **End of File Condition:**

   To signal the end of input, press `Ctrl+D`. The shell will gracefully exit.

## Limitations

This simple shell program has some limitations:

- It supports only single-word commands, so complex commands with arguments won't work.
- It does not support advanced features like pipes, semicolons, or file redirections.
- Command lines can have arguments, but they must be space-separated and placed after the command itself.

## Contribution

Contributions to this project are welcome! If you find any issues or have improvements to suggest, please feel free to open an issue or create a pull request.
