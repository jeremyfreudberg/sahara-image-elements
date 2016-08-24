here's what the massopencloud module does:

1. it installs pig.
2. it sets environment variables properly for "ubuntu" and "hadoop" users.

eventually:
3. it will change resourcemanager type to fair scheduler.
   - this is so yarn/oozie can handle pig.
   - currently, must be done manually (through ng-template or otherwise)

it's just for vanilla plugin
