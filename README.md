# Utility commands

## find grep

```bash
$ find $1 -name $2 -print | xargs grep $3
```

## ps grep

```bash
$ ps aux | grep $1 | grep -v grep
```

## port listen

```bash
$ sudo lsof -nP -i4TCP -sTCP:LISTEN
```

## stdout null

```bash
$ $* > /dev/null 2>&1 &
```
