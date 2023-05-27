Error repro setup for this rails issue: https://github.com/rails/rails/issues/48318

The error can be seen by running rails and navigating to localhost:3000.

I needed to run rails with this:
```
RUBY_THREAD_VM_STACK_SIZE=10485760 ./bin/rails s
```
in order to avoid a `stack level too deep (SystemStackError)` error.

I've reproduced this with ruby version 3.2.2.
