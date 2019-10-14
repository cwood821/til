# Use arrays in bash scripts

Bash supports single-dimension arrays. There are several ways to declare arrays, one such way is:

```bash
myarr=( zero one two three four )

# Index into arrays with this syntax
echo ${myarr[0]}
```

Loop over an array with a for loop:

```bash
for i in "${myarr[@]}"
do
   echo "$i"
done
```

Remember: [Bash variables are untyped](http://www.tldp.org/LDP/abs/html/untyped.html#BVUNTYPED). Read more and see examples in the [Advanced Bash Scripting Guide](http://www.tldp.org/LDP/abs/html/arrays.html).
