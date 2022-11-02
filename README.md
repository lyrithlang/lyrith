# This is Lyrith.

Lyrith is a personal project to essentially mash together elements of other programming languages and concepts from talks I found interesting.

- **Highly performant** via Just-in-Time _and_ Ahead-of-Time compilation
- **Highly concurrent** via lightweight actor-model concurrent threads  
  _Inspired by Go, Elixir, Pony_
- **Robust** via fault tolerance and non-halting errors  
  _Inspired by Elixir, Zig_
- **Memory safe** via borrow checking and capability-based security  
  _Inspired by Rust and Pony_
- **Runtime debuggable** (in specific execution modes)
- **Simple** via no hidden control flow, memory allocations, preprocessing and macros  
  _Inspired by Zig_
- **Easy** to read and write, with syntatic roots in _Python_

## Roadmap

### Proof of Concept (LLVM via llvmlite)

- Compiler Frontend
  - [ ] ASTGen
  - [ ] LLVM IR CodeGen

- Featureset
  - [ ] Memory Safety
  - [ ] Capabilities-based Security
  - [ ] Actor-model Concurrency Threads
  - [ ] Fault Tolerance

### Working Demo (Self-Hosted Compiler)

- Compiler Frontend (Re-implementation)
  - [ ] In-house Packrat Parser
  - [ ] ASTGen
  - [ ] Lyric IR CodeGen

- Compiler Backend via Lyric
  - [ ] IR Optimisation Passes
  - [ ] Execution Environment
  - [ ] Faster-than-Light Just-in-Time Compilation
  - [ ] Ahead-of-Time Compilation
    - [ ] amd64 CodeGen
    - [ ] aarch64 CodeGen

- Compiler + Toolchain Featureset
  - [ ] Non-Halting Errors
  - [ ] Runtime Debugging via Introspection and Reflection
  - [ ] Hot Reloading

## Copyright and Licence

Copyright © 2022 Mark Joshwel. All rights reserved.

Lyrith has multiple licences, but is *not* dual-licenced. Please refer to the information below for more information. In the event where you need to quickly know what licence governs a code file, the text header will indicate so.

- `src/stdlib`, `src/builtins`  
  Unlicense Licenced

- `*`, `src/lyrith/**/*`  
  LGPL Licenced

The Lyrith is licenced under the [GNU Lesser General Public License (LGPL)](https://www.gnu.org/licenses/lgpl-3.0.en.html) version 3 or later, see the [LICENCE.LESSER](LICENCE.LESSER) file for the full text. As the LGPL is a set of additional permissions on top of the GNU General Public License (GPL) version 3 or later, see the [LICENCE.GPL](LICENCE.GPL) file for the GPL full text.

However, the Lyrith standard and `builtins` library are released into the public domain using [The Unlicense](https://unlicense.org/), see [LICENCE.UNLICENSE](LICENCE.UNLICENSE) for the full text.
