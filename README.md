# pdf_opener

## problems faced !
- file size 133.33 mb you can only push 100mb max!

### git lfs failed
You must have push access to verify locks error.

### split files?
#### To split files into even-sized, smaller chunks, and combine them back into a single file
##### To Split
split -b 100m 'somefile.ext' somefile.
##### -b tells the split command that you want to specify the 'byte' size 100m, or 100 megabytes is the size of the parts we wanted 'somefile.ext' is the file we want to split into parts somefile. tells the split command that all part files should begin with 'some file.'
#### To Join
cat somefile.?? > 'somefile.ext'


- still can't push! 
fixed warning by reducing size to 50mb

- still can't push!!
- increased post buffer using
> git config http.postBuffer 524288000



# thanks to 
- https://stackoverflow.com/a/15851500
- https://gist.github.com/sosukeinu/4665975
