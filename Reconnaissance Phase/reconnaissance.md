## Exploitation (!)

### Connecting to the server (*)

Here is some boilerplate code for connecting to a docker-based challenge:

```python
if __name__ == "__main__":
    r = remote("0.0.0.0", 1337)
    pwn()
```
