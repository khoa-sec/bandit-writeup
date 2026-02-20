# Bandit Level 12 → 13

## Goal

Find the password.

## Solution

The password is stored in the file data.txt which contains multiple layers of compression and encoding. Use xxd to reverse the hex dump, then repeatedly identify the file type, rename, and decompress it until the password is revealed.

Command used:

mktemp -d
cd /tmp/tmp.xxxxxxxxxx
cp ~/data.txt .

xxd -r data.txt > filek

file filek

mv filek filek.gz
gzip -d filek.gz

mv filek filek.bz2
bzip2 -d filek.bz2

mv filek filek.tar
tar -xf filek.tar

file data5.bin
mv data5.bin data5.bin.tar
tar -xf data5.bin.tar

file data6.bin
mv data6.bin data6.bin.bz2
bzip2 -d data6.bin.bz2

file data6.bin
mv data6.bin data6.bin.tar
tar -xf data6.bin.tar

file data8.bin
mv data8.bin data8.bin.gz
gzip -d data8.bin.gz

file data8.bin
cat data8.bin 

## Result

Password found.
