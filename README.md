
  Require

  How to use:
  -   use: Require( <pathToFile> )
      example: Require( "classes/core/printer")
      note:   do NOT add any prefixes like cl_, sv_, sh_
              or the .lua file ending.
              Scince all files are included only one time
              it is recommended to save the return into a
              local variable

  What it does:
  -   all found files get combined and included ONCE
  -   if the file was required before, the same pointer gets returned
  -   scans in lua and gamemode folder by default
  -   no prefix is handled like sh_

  How it works:
  -   meta-table magic
