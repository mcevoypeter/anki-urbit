# Urbit Resources

### [`hoon/`](hoon)
The contents of [`hoon/tjic`](hoon/tjic) were written by Travis J.I. Corcoran. I
stumbled across them thanks to [this
tweet](https://twitter.com/MorlockP/status/1502367967476174859?ref_src=twsrc%5Etfw%7Ctwcamp%5Etweetembed%7Ctwterm%5E1502367967476174859%7Ctwgr%5E%7Ctwcon%5Es1_c10&ref_url=https%3A%2F%2Fpublish.twitter.com%2F%3Fquery%3Dhttps3A2F2Ftwitter.com2FMorlockP2Fstatus2F1502367967476174859widget%3DTweet).

### [`papers/`](papers)

 Year | Title                                                                                                                    | Author
------|:-------------------------------------------------------------------------------------------------------------------------|:-----------------------
 1966 | [The Next 700 Programming Languages](papers/next-700-1966-landin.pdf)                                                    | Landin
 1989 | [Tcl: An Embeddable Command Language](papers/tcl-usenix-1989-ousterhout.pdf)                                             | Ousterhout
 1991 | [The Design and Implementation of a Log-Structured File System](papers/lfs-1991-rosenblum-ousterhout.pdf)                | Rosenblum & Ousterhout
 1996 | [An On-the-fly Bytecode Compiler for Tcl](papers/tcl-bytecode-compiler-1996-lewis.pdf)                                   | Lewis
 2011 | [Kafka: a Distributed Messaging System for Log Processing](papers/kafka-2011-kreps-et-al.pdf)                            | Kreps et al
 2014 | [In Search of an Understandable Consensus Algorithm (Extended Version)](papers/raft-extended-2014-ongaro-ousterhout.pdf) | Ongaro & Ousterhout
 2015 | [The Cuneiform Tablets of 2015](papers/cuneiform-2015-nguyen-kay.pdf)                                                    | Nguyen & Kay
 2016 | [Sulong - Execution of LLVM-Based Languages on the JVM](papers/sulong-2016-rigger-et-al.pdf)                             | Rigger et al
 2016 | [Urbit: A Solid-State Interpreter](papers/urbit-2016-yarvin-et-al.pdf)                                                   | Yarvin et al
 2017 | [The Case for Writing a Kernel in Rust](papers/levy-et-al-2017-rust-kernel.pdf)                                          | Levy et al
 2018 | [Build Systems à la Carte](papers/build-systems-2018-mokhov-et-al.pdf)                                                   | Mokhov et al
 2018 | [Poster: Log Pruning in Distributed Event-sourced Systems](papers/poster-log-pruning-2018-erb-et-al.pdf)                 | Erb et al
 2020 | [DBOS: A Proposal for a Data-Centric Operating System](papers/dbos-proposal-2020-cafarella-et-al.pdf)                    | The DBOS Committee
 2021 | [DBOS: A DBMS-oriented Operating System](papers/dbos-2021-skiadopoulos-et-al.pdf)                                        | Skiadopoulos et al
 2022 | [A Progress Report on DBOS: A Database-oriented Operating System](papers/dbos-progress-report-2022-li-et-al.pdf)         | Li et al

### C Style

#### Variable names

##### Three-letter representation

 Concept         | Three-letter representation
:--------------- |:----------------------------
 block           | `blk`
 buffer          | `buf`, `byt`
 component       | `cop`
 count           | `cnt`
 current         | `cur`
 data            | `dat`
 directory       | `dir`
 epoch           | `epo`, `poc`
 event           | `eve`, `evt`
 file            | `fil`
 file descriptor | `fid`
 first           | `fir`
 free            | `fre`
 function        | `fun`
 ID              | `ide`
 image           | `img`
 index           | `idx`
 last            | `las`
 length          | `len`
 list            | `lis`
 log             | `log`
 name            | `nam`
 north           | `nor`
 next            | `nex`
 page            | `pag`
 parent          | `par`
 patch           | `pat`
 pool            | `pol`
 previous        | `pre`
 queue           | `que`
 size            | `siz`
 south           | `sou`
 start           | `sar`
 token           | `tok`
 vector          | `vec`

##### One-letter type suffix

Type        | Type suffix
:-----------|:------------

##### Two-lettter type suffix

Type        | Type suffix
:-----------|:------------

##### Local variables

All local variable names should fit the following pattern: `<three_letter_representation>_<type_suffix>`

##### Global variables

All global variable names (including statically-scoped global variables) should fit the following pattern: `<three_letter_representation>_<three_letter_representation>_<type_suffix>`.

 duct | call stack (list of wire)
 move | pair of duct and rest of move
 pass | kind of like function call
 give | kind of like function return
 note | task tagged by vane
 wire | arvo path
