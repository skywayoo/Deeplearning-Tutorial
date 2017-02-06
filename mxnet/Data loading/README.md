#Data loading

### Create ImageIterator

* mx.io.ImageRecordIter()

> 1. change direction`cd mxnet/tools/`
> 2. create .lst file `python im2rec.py --list=True --recursive=True [list_file] [filepath] ` 
> 3. create .rec file(name the same as .lst)  `python im2rec.py --resize=256 --quality=90 --num-thread=4 [list_file] [filepath]`    

* mx.io.arrayiter()
* mx.io.CSVIter()
* mx.io.MNISTIter()
* mx.io.extract()

### Using the Iterator data 

* mx.io.extract()
>``


