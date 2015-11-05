Build Instruction
=================

1. Copy files from your build dir to jdk and jre subfolders according to layout in `files.txt`.
2. Delete duplicates from jdk package - there are files in `bin` folder that conflicts with jre (two packages should not contain same files).
3. Build packages:
   ```
   dpkg-deb --build tuxjdk-8-jdk_8.60-1
   dpkg-deb --build tuxjdk-8-jre_8.60-1
   ```

