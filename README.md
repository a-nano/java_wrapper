# javaonsygwin

TAKAHASHI,Toru's java on sygwin program.
Clone [https://jaist.dl.osdn.jp/javaoncygwin/53264/java_wrapper]

## Usage

### 1
Set windows env path.
JAVA_HOME = install/jdk/dir

### 2
Modify encoding to cp932.

```
-exec "$PROGRAM" $ARGS
+exec "$PROGRAM" $ARGS 2>&1 | iconv -f cp932 -t utf-8
```

### 3
Make symlinks

```
cd install/java_wrapper/dir
java_wrapper createsymlinks
```

## Author
TAKAHASHI,Toru