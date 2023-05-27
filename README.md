I needed to run rails with this:
```
RUBY_THREAD_VM_STACK_SIZE=10485760
```
in order to avoid a `stack level too deep (SystemStackError)` error.

