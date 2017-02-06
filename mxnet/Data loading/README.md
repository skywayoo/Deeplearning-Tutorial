# Create ImageIterator

### mx.io.ImageRecordIter()

* How to use own images to dataiter

> 1. change direction`cd mxnet/tools/`
> 2. create .lst file `python im2rec.py --list=True --recursive=True [list_file] [filepath] ` 
> 3. create .rec file `python im2rec.py --resize=256 --quality=90 --num-thread=4 [list_file] [filepath]`    

### mx.io.extract()
> extract the iterator data

> data = `mx.io.extract(data_iter)[1]`

> labels = `mx.io.extract(data_iter)[2]`

### mx.io.arrayiter()
### mx.io.CSVIter()
### mx.io.MNISTIter()


