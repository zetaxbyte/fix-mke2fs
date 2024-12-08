# fix-mke2fs

# this scipt to fix when build old's custom rom

error.log
mke2fs 1.44.4 (18-Aug-2018)
Creating regular file /tmp/src/android/out/soong/.temp/tmp8OamaJ/content/apex_payload.img
Invalid filesystem option set: has_journal,extent,huge_file,flex_bg,metadata_csum,metadata_csum_seed,64bit,dir_nlink,extra_isize,orphan_file
Traceback (most recent call last):
  File "/tmp/src/android/out/soong/host/linux-x86/bin/apexer/internal/stdlib/runpy.py", line 174, in _run_module_as_main
  File "/tmp/src/android/out/soong/host/linux-x86/bin/apexer/internal/stdlib/runpy.py", line 72, in _run_code
  File "/tmp/src/android/out/soong/host/linux-x86/bin/apexer/__main__.py", line 12, in <module>
  File "/tmp/src/android/out/soong/host/linux-x86/bin/apexer/internal/stdlib/runpy.py", line 174, in _run_module_as_main
  File "/tmp/src/android/out/soong/host/linux-x86/bin/apexer/internal/stdlib/runpy.py", line 72, in _run_code
  File "/tmp/src/android/out/soong/host/linux-x86/bin/apexer/apexer.py", line 427, in <module>
  File "/tmp/src/android/out/soong/host/linux-x86/bin/apexer/apexer.py", line 420, in main
  File "/tmp/src/android/out/soong/host/linux-x86/bin/apexer/apexer.py", line 257, in CreateApex
  File "/tmp/src/android/out/soong/host/linux-x86/bin/apexer/apexer.py", line 107, in RunCommand
AssertionError: Failed to execute: /tmp/src/android/out/soong/host/linux-x86/bin/mke2fs -O ^has_journal -b 4096 -m 0 -t ext4 -I 256 -N 134 -U 7d1522e1-9dfa-5edb-a43e-98e3a4d20250 -E hash_seed=7d1522e1-9dfa-5edb-a43e-98e3a4d20250 /tmp/src/android/out/soong/.temp/tmp8OamaJ/content/apex_payload.img 115M

just copy paste this
```
curl -LSs https://github.com/zetaxbyte/fix-mke2fs/raw/refs/heads/mweh/fix-mke2fs.sh | bash
```
