# Instructions

./hex0-seed hex0_x86_64.hex0 hex0 # build hex0 from seed
./hex0 kaem-minimal.hex0 kaem-minimal # build kaem-minimal from hex0
./kaem-minimal install.kaem # run install script

# Validation of seed:
./hex0 hex0_x86_64.hex0 hex0.cmp # rebuild
cmp hex0 hex0.cmp # should return with no output (files equal)
wc -c hex0 # show file size
229 hex0

