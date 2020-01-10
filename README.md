# My Notes - for the offical README to get started see README_Theirs.md

## Instructions

Install the tool as noted in the README_Theirs.md file, but don't try to generate any hash tables or use it yet.

We need to generate a hash database to look up phone numbers against. They push you towards a PostGresSQL DB, but we're going to use a SQLite database rather than PostGresQL as it's much easier to get the tool working and keeps it all neat.

cd hash2phone
python3 hashmap_gen_sqlite.py dbinit
python3 hashmap_gen_sqlite.py 4475XXXXXXXX
python3 hashmap_gen_sqlite.py 4477XXXXXXXX
python3 hashmap_gen_sqlite.py 4478XXXXXXXX
python3 hashmap_gen_sqlite.py 4479XXXXXXXX

We can now run ble_read_state to get the possible phone numbers when you connect to a network
python3 ble_read_state.py -c 



None of the other scripts seem to want to work, but this works nicely for demo purposes.
