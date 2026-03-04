# Instructions

# build hex0 from seed
./hex0-seed ./src/hex0.hex0 ./bin/hex0
# build kaem from hex0
./bin/hex0 ./src/kaem.hex0 ./bin/kaem
# run the installation process
./bin/kaem-minimal install.kaem # run install script

# Validation of seed:
cmp ./bin/hex0 hex0-seed # should return with no output (files equal)
./bin/hex0 ./src/hex0.hex0 hex0.cmp # rebuild
cmp ./bin/hex0 hex0.cmp # should return with no output (files equal)
rm hex0.cmp
wc -c ./bin/hex0 # show file size
229 hex0

