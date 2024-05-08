<a name="readme-top"></a>

<!-- PROJECT SUMMARY -->
<div align="center">

  <h3 align="center">pipex</h3>

  <p align="center">
    Summary:
    This project is about discovering about a UNIX mechanism: pipes.
  </p>
  <br>
</div>

<!-- TABLE OF CONTENTS -->

- [About The Project](#about-the-project)
- [Usage](#usage)
- [Sources](#sources)

<!-- ABOUT THE PROJECT -->
## About The Project

This was also the first time that I had to use `fork()` and thus I had learned to bit about processes, threads and pipes.

This project was really helpful to discover a concept that would be central for minishell, another 42 cursus project.
Personnaly, it was easier to discover the pipes on a smaller scale and then applying what I learned on this project to minishell.

This is all coded in C.

The bonus are the handling of multiples pipes and a first introduction to here_doc and redirections.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- USAGE -->
## Usage

After compiling the program through the Makefile you can use the executable: `pipex`.

The program can be launched using the following syntax: `./pipex file1 cmd1 cmd2 file2`.

Here `file1` and `file2` are file names, `cmd1` and `cmd2` are shell commands with their parameters.

The idea was that launching a command like this is the equivalent of launching a normal shell command like `< file1 cmd1 | cmd2 > file2` in the terminal.

For the multiples pipes bonus, you can test them with the following commands: `./pipex file1 cmd1 cmd2 cmd3 ... cmdn file2` will have the same result as `< file1 cmd1 | cmd2 | cmd3 ... | cmdn > file2`.

For the redirections and here_doc, it's like this: `./pipex here_doc LIMITER cmd cmd1 file` for the a shell command like `cmd << LIMITER | cmd1 >> file`.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- SOURCES -->
## Sources

* https://www.youtube.com/playlist?list=PLfqABt5AS4FkW5mOn2Tn9ZZLLDwA3kZUY
* Videos in french:
  * https://www.youtube.com/watch?v=k8bGYB2gl-A
  * https://www.youtube.com/watch?v=Gat7z23A7mg

<p align="right">(<a href="#readme-top">back to top</a>)</p>