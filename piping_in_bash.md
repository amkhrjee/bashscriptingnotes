# Piping in bash 
`>` is used to **redirect output**.
```
    $ echo "hello" > file.txt
```
`<` is used to **redirect input**.
```
    $ cat < file.txt
```
Output:
```
    hello
```
`>>` is used to **append output to the end of the file**.
```
    $ echo "world!" >> file.txt
```
Output:
```
    hello
    world!
```
`<<` (called "here document") is a **file literal** or **input stream literal**.
```
    $ cat << EOF >> file.txt
```
Output:
```
    >
```
Here you can type whatever you want and it can be multi-line. It ends when you type EOF. (We used EOF in our example but you can use something else instead.)
```
    > linux
    > is
    > EOF
```
Output:
```
    hello
    world!
    linux
    is
```    

`<<<` (called "here string") is the **same as `<<`
but takes only one "word" (i.e., string)**.

```    $ cat <<< great! >> file.txt ```

Output:

```
    hello
    world!
    linux
    is
    great!
```
