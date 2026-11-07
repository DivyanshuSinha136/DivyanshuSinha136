<div align="center">

<img src="./assets/banner.svg" alt="Divyanshu Sinha, systems and programming-language engineer" width="100%">

<br>

[![GitHub followers](https://img.shields.io/github/followers/DivyanshuSinha136?style=flat-square&logo=github&logoColor=white&color=34d399&labelColor=0d1117)](https://github.com/DivyanshuSinha136)
[![PyPI](https://img.shields.io/badge/PyPI-pythonaibrain-34d399?style=flat-square&logo=pypi&logoColor=white&labelColor=0d1117)](https://pypi.org/user/DivyanshuSinha/)
[![KingCobra](https://img.shields.io/badge/Language-KingCobra-34d399?style=flat-square&logo=github&logoColor=white&labelColor=0d1117)](https://github.com/DivyanshuSinha136/KingCobra)
[![PSF Member](https://img.shields.io/badge/Python%20Software%20Foundation-Member-34d399?style=flat-square&logo=python&logoColor=white&labelColor=0d1117)](https://www.python.org/psf/)
[![Email](https://img.shields.io/badge/Email-divyanshu.sinha631%40gmail.com-34d399?style=flat-square&logo=gmail&logoColor=white&labelColor=0d1117)](mailto:divyanshu.sinha631@gmail.com)

**[About](#about)** &nbsp;·&nbsp; **[KingCobra](#kingcobra)** &nbsp;·&nbsp; **[Projects](#projects)** &nbsp;·&nbsp; **[Tech stack](#tech-stack)** &nbsp;·&nbsp; **[GitHub analytics](#github-analytics)** &nbsp;·&nbsp; **[Contact](#contact)**

</div>

<img src="./assets/divider.svg" width="100%" alt="">

<h2 id="about"><img src="./assets/icons/user.svg" width="26" align="absmiddle" alt=""> About</h2>

I build software from first principles: **AI systems, programming languages, assemblers and operating systems**. I started with Python and moved down the stack to C, C++, Assembly and bare-metal x86 machine code. I also ship secure web applications and security tooling.

|  |  |
|:--|:--|
| **Name** | Divyanshu Sinha |
| **Age** | 18 |
| **Region** | India |
| **Email** | [divyanshu.sinha631@gmail.com](mailto:divyanshu.sinha631@gmail.com) |
| **Focus** | Programming languages, operating systems, AI backends, security software |
| **Creator of** | `pythonaibrain` · `pythonaibrain-client` · `TigerASM` · `KingCobra` · `CDNEE` · `Aetherix` · `Peacock OS` |

**Highlights**

- Earned the [Quickdraw achievement](https://github.com/users/DivyanshuSinha136/achievements/quickdraw) on GitHub.
- Built AI systems from scratch: rule-based engines, Python AI backends and an Assembly-based AI.
- Published Python packages on PyPI: [`pythonaibrain`](https://pypi.org/project/pythonaibrain/) and [`pythonaibrain-client`](https://pypi.org/project/pythonaibrain-client/).
- Designed three languages and tools in the same space: KingCobra, CDNEE and the TigerASM assembler.
- Developed games and simulation engines (3D assets, train simulations) and an interactive Class 12 Physics GUI.
- Skilled in ethical hacking, security software and encryption systems.
- Built secure web applications with OTP verification, encryption and real-time features.

<img src="./assets/divider.svg" width="100%" alt="">

<h2 id="kingcobra"><img src="./assets/icons/terminal.svg" width="26" align="absmiddle" alt=""> KingCobra</h2>

<a href="https://github.com/DivyanshuSinha136/KingCobra"><img src="./assets/kingcobra-banner.svg" alt="KingCobra, a native general-purpose systems programming language" width="100%"></a>

<div align="center">

[![Repository](https://img.shields.io/badge/Repository-DivyanshuSinha136%2FKingCobra-34d399?style=for-the-badge&logo=github&logoColor=white&labelColor=0d1117)](https://github.com/DivyanshuSinha136/KingCobra)
[![Releases](https://img.shields.io/github/v/release/DivyanshuSinha136/KingCobra?style=for-the-badge&color=34d399&labelColor=0d1117&label=Release)](https://github.com/DivyanshuSinha136/KingCobra/releases)
[![License](https://img.shields.io/badge/License-MIT-34d399?style=for-the-badge&labelColor=0d1117)](https://github.com/DivyanshuSinha136/KingCobra/blob/HEAD/LICENSE)

</div>

> [!NOTE]
> **KingCobra is my flagship project.** It is an independent, actively developed programming language with its own syntax, runtime, JIT, compiler and standard library. Source files use the **`.kc`** extension. It is a native systems language with scripting-language ergonomics, not a Python dialect, and it has no relation to other languages named "Cobra".

**What it is.** KingCobra has a small, readable syntax and a REPL, but it also gives you explicit memory, checked C-style pointers, a real FFI, raw machine code and a bare-metal compiler target. The language, runtime, JIT and every standard-library module are plain **C11** with **no third-party build-time dependencies**.

```kingcobra
struct Point { x: int, y: int }
impl Point { fn len2(self) -> int { return self.x * self.x + self.y * self.y; } }

fn main() {
    let nums = [5, 3, 8, 1, 9];
    let [first, ...rest] = nums;
    print(f"first={first}", Point { x: 3, y: 4 }.len2(), nums[1..3]);

    try { throw error("rejected"); } catch (e) { print(e.message); }
}
```

<h3><img src="./assets/icons/star.svg" width="20" align="absmiddle" alt=""> Key capabilities</h3>

| Area | What you get |
|:--|:--|
| **Easy like a script** | `let`/`var`, f-strings, slicing, destructuring, `match`, `try`/`catch`, a REPL and `help()` with `///` doc comments |
| **Native underneath** | Exact 64-bit integers, a closure JIT to x86-64 machine code, a real `extern` FFI, `rhex` and `unsafe` for raw machine code |
| **Explicit memory, no GC** | `free` on every heap value, use-after-free and double free are errors, `defer` runs during unwinding, `--leaks` finds what you forgot |
| **Checked pointers** | C-style pointers and buffers with bounds and lifetime checking |
| **Real tooling** | Built-in `test` and `check`, a static type checker, errors with source excerpts and "did you mean", a terminal IDE and a debugger |
| **Bare metal** | `kcc` compiles to standalone executables and to a freestanding kernel; **KCOS**, an OS written in KingCobra, boots in QEMU |
| **Portable** | Linux and Windows (macOS builds with `make`) on x86-64, ARM64, ARMhf and RISC-V |

<h3><img src="./assets/icons/layers.svg" width="20" align="absmiddle" alt=""> Toolchain architecture</h3>

<div align="center">
<img src="./assets/toolchain.svg" alt="KingCobra toolchain: source files go through the front end into the interpreter, JIT or kcc compiler" width="100%">
</div>

<h3><img src="./assets/icons/package.svg" width="20" align="absmiddle" alt=""> Standard library: 21 native modules</h3>

| Category | Modules |
|:--|:--|
| **Systems and hardware** | `std.acpi` · `std.mmio` · `std.mmu` · `std.memory` · `std.rhex` · `std.system` |
| **I/O and data** | `std.io` · `std.fbin` · `std.csv` · `std.json` · `std.regx` |
| **Networking** | `std.network` · `std.http` (HTTP and TLS) |
| **Compute and AI** | `std.vector` · `std.nn` · `std.nlp` |
| **Media and interfaces** | `std.gui` · `std.game` · `std.ascii_screen` · `std.music_note` · `std.tts` |

<h3><img src="./assets/icons/code.svg" width="20" align="absmiddle" alt=""> Quick start</h3>

Requires a C11 compiler and `make`.

```bash
git clone https://github.com/DivyanshuSinha136/KingCobra.git
cd KingCobra

make                               # builds ./kingcobra
./kingcobra run examples/hello.kc  # run a program
./kingcobra repl                   # interactive REPL
make test                          # run every example end to end
```

[Documentation](https://github.com/DivyanshuSinha136/KingCobra/tree/HEAD/docs) &nbsp;·&nbsp; [Releases](https://github.com/DivyanshuSinha136/KingCobra/releases) &nbsp;·&nbsp; [Issues](https://github.com/DivyanshuSinha136/KingCobra/issues) &nbsp;·&nbsp; [Contributing](https://github.com/DivyanshuSinha136/KingCobra/blob/HEAD/CONTRIBUTING.md)

<img src="./assets/divider.svg" width="100%" alt="">

<h2 id="projects"><img src="./assets/icons/cpu.svg" width="26" align="absmiddle" alt=""> Key projects</h2>

| Project | Category |
|:--|:--|
| [KingCobra](#kingcobra-project) | Programming language |
| [CDNEE](#cdnee) | Programming language |
| [TigerASM](#tigerasm) | Assembler |
| [Peacock OS](#peacock-os) | Operating system |
| [pythonaibrain](#pythonaibrain) | AI backend |
| [pythonaibrain-client](#pythonaibrain-client) | Client library |
| [Aetherix](#aetherix) | Open-source project |

<h3 id="pythonaibrain"><a href="https://pypi.org/project/pythonaibrain/">pythonaibrain</a></h3>

An AI backend with advanced contextual understanding, self-learning capabilities, and integration-ready APIs.

<h3 id="pythonaibrain-client"><a href="https://pypi.org/project/pythonaibrain-client/">pythonaibrain-client</a></h3>

Client library to easily interact with `pythonaibrain` servers and APIs.

<h3 id="tigerasm"><a href="https://github.com/DivyanshuSinha136/TigerASM">TigerASM</a></h3>

Custom assembler for learning low-level programming, system design, and assembly code execution.

<h3 id="kingcobra-project"><a href="https://github.com/DivyanshuSinha136/KingCobra">KingCobra Programming Language</a></h3>

Native, general-purpose systems language with a Python-like feel, custom syntax, `.kc` source files, a JIT, the `kcc` compiler, a static type checker and a terminal IDE. See the [full KingCobra section](#kingcobra) above.

<h3 id="cdnee"><a href="https://divyanshusinha136.github.io/CDNEE-Docs/">CDNEE Programming Language</a></h3>

CDNEE (Control Dynamic Native Execution Engine) is a high-level assembly-oriented programming language designed for direct access to native machine-code execution without the complexity of traditional assemblers or low-level compilers. It sits at a unique intersection: readable, structured syntax on the surface, bare-metal native performance underneath.

Programs are written in `.cdnee` source files and run through the CDNEE runtime, which compiles and executes x86-64 machine code on the fly using a built-in JIT engine backed by NASM. You can drop into raw assembly, benchmark it, patch it at runtime, inspect its disassembly, snapshot its memory, and call foreign libraries, all from a single coherent source file.

[![Docs](https://img.shields.io/badge/Official%20Docs-CDNEE-34d399?style=flat-square&labelColor=0d1117)](https://divyanshusinha136.github.io/CDNEE-Docs/)
[![Releases](https://img.shields.io/badge/Official%20Releases-GitHub-34d399?style=flat-square&logo=github&logoColor=white&labelColor=0d1117)](https://github.com/DivyanshuSinha136/CDNEE/releases)

<h3 id="peacock-os">Peacock OS</h3>

Experimental lightweight operating system focused on performance, security, and system programming learning.

<h3 id="aetherix"><a href="https://github.com/DivyanshuSinha136/Aetherix">Aetherix</a></h3>

Open-source project by me. See the [repository](https://github.com/DivyanshuSinha136/Aetherix) for details.

<img src="./assets/divider.svg" width="100%" alt="">

<h2 id="tech-stack"><img src="./assets/icons/layers.svg" width="26" align="absmiddle" alt=""> Tech stack</h2>

<div align="center">

<img src="https://skillicons.dev/icons?i=py,c,cpp,js,html,css,lua,go,flask,sqlite,firebase,git,linux,vscode&theme=dark&perline=14" alt="Python, C, C++, JavaScript, HTML, CSS, Lua, Go, Flask, SQLite, Firebase, Git, Linux, VS Code">

</div>

| Layer | Technologies |
|:--|:--|
| **Languages** | Python · C · C++ · JavaScript · HTML · CSS · Assembly (x86 machine code) · Lua · Go |
| **Frameworks and tools** | Flask · CustomTkinter · Socket.IO · SQLite · Firebase · MinGW-w64 · Turbo C++ |
| **Domains** | AI and NLP · operating systems and systems programming · language and assembler design · game and simulation engines · web applications · security software and ethical hacking |

<img src="./assets/divider.svg" width="100%" alt="">

<h2 id="github-analytics"><img src="./assets/icons/chart.svg" width="26" align="absmiddle" alt=""> GitHub analytics</h2>

<div align="center">

<img height="180" alt="GitHub stats" src="https://github-readme-stats.vercel.app/api?username=DivyanshuSinha136&show_icons=true&hide_border=true&bg_color=0d1117&title_color=34d399&icon_color=34d399&text_color=c9d1d9&ring_color=34d399&rank_icon=github&include_all_commits=true" />
<img height="180" alt="Most used languages" src="https://github-readme-stats.vercel.app/api/top-langs/?username=DivyanshuSinha136&layout=donut&hide_border=true&bg_color=0d1117&title_color=34d399&text_color=c9d1d9&langs_count=8" />

<br><br>

<img alt="Contribution streak" src="https://streak-stats.demolab.com?user=DivyanshuSinha136&hide_border=true&background=0D1117&ring=34D399&fire=34D399&currStreakLabel=34D399&currStreakNum=C9D1D9&sideLabels=C9D1D9&sideNums=C9D1D9&dates=8B949E&stroke=30363D" />

<br><br>

<img alt="Contribution activity graph" width="100%" src="https://github-readme-activity-graph.vercel.app/graph?username=DivyanshuSinha136&bg_color=0d1117&color=34d399&line=34d399&point=ffffff&area=true&area_color=34d399&hide_border=true&custom_title=Contribution%20activity" />

</div>

<img src="./assets/divider.svg" width="100%" alt="">

<h2 id="recognition"><img src="./assets/icons/award.svg" width="26" align="absmiddle" alt=""> Memberships and recognition</h2>

| Program | What it provides |
|:--|:--|
| **Python Software Foundation (PSF)** | Official Python community membership |
| **Google Developer Program and Firebase Studio Developer Community** | Developer tooling and cloud services |
| **Google Cloud × NVIDIA Community** | NIM API and LLM access |
| **GDG on Campus** | Hackathons, labs and workshops |
| **NVIDIA Developer Program** | AI model testing and GPU-backed inference |

<img src="./assets/divider.svg" width="100%" alt="">

<h2 id="contact"><img src="./assets/icons/mail.svg" width="26" align="absmiddle" alt=""> Contact</h2>

<div align="center">

[![Email](https://img.shields.io/badge/Email-divyanshu.sinha631%40gmail.com-34d399?style=for-the-badge&logo=gmail&logoColor=white&labelColor=0d1117)](mailto:divyanshu.sinha631@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-DivyanshuSinha136-34d399?style=for-the-badge&logo=github&logoColor=white&labelColor=0d1117)](https://github.com/DivyanshuSinha136)
[![PyPI](https://img.shields.io/badge/PyPI-DivyanshuSinha-34d399?style=for-the-badge&logo=pypi&logoColor=white&labelColor=0d1117)](https://pypi.org/user/DivyanshuSinha/)

<sub>Divyanshu Sinha · India</sub>

*"Dream big, code bigger. The only limit is your imagination."*

</div>
