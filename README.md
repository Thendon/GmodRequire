
  Require

  How to use:
  - use: Require( <i>pathToFile</i> )
  - example: Require( "classes/core/printer")
  - note: 
      - do NOT add any prefixes like cl_, sv_, sh_ or the .lua file ending.
      - Scince all files are included only one time it is recommended to save the return into alocal variable

  What it does:
  -   all found files get combined and included ONCE<br />
  -   if the file was required before, the same pointer gets returned<br />
  -   scans in lua and gamemode folder by default<br />
  -   no prefix is handled like sh_<br />

  How it works:
  -   meta-table magic
