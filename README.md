# Instructions

./hex0-seed ./src/hex0_x86_64.hex0 ./bin/hex0 # build hex0 from seed
./bin/hex0 ./src/kaem-minimal.hex0 ./bin/kaem-minimal # build kaem-minimal from hex0
./bin/kaem-minimal install.kaem # run install script

# Validation of seed:
cmp ./bin/hex0 hex0-seed # should return with no output (files equal)
./bin/hex0 ./src/hex0_x86_64.hex0 hex0.cmp # rebuild
cmp ./bin/hex0 hex0.cmp # should return with no output (files equal)
rm hex0.cmp
wc -c ./bin/hex0 # show file size
229 hex0

